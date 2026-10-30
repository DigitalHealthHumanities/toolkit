---
layout: homepage
title: Digital Health Humanities Toolkit
---
<h1>{{ site.title }}</h1>

<p>{{ site.description }}</p>

<p>Read the <a href="https://escholarship.org/uc/item/9kt9c6hd">White Paper</a></p>

{% assign sublessons = site.lessons | where: "layout", "sublesson" %}
{% assign introlessons = sublessons | where: "crashcourse", "yes" %}

<!-- Pull Crash Course Lessons and Generate Cards -->
<h2>Digital Humanities Crash Course</h2>
<div class="row mt-2 mb-3">
    {% for lesson in introlessons %}
        <div class="col-md-4 mb-3">
            <div id="intro-course-header" class="card dhht-card border-dark text-center h-100">
                <div class="card-header intro pt-3">
                    <a href="{{ site.baseurl }}{{ lesson.permalink }}">
                        <h3 class="card-title">{{ lesson.title }}</h3>
                    </a>
                </div>
                <div class="card-body">
                    <p class="card-text">{{ lesson.abstract }}</p>
                    <ol>{% assign objs = lesson.learningobjectives | split: ';' %}{% for oblist in objs %}<li align="left">{{ oblist }}</li>{% endfor %}</ol>
                </div>
            </div>
        </div>
    {% endfor %}
</div>

<h2>Lessons</h2>
<div class="row mt-3 mb-3">
<!-- Pull non Crash Course lessongroups and generate cards -->
    {% assign lessongroups = site.lessons | where: "layout", "lessongroup" %}
    {% for sectionloop in lessongroups %}
        {% unless sectionloop.title == "Digital Humanities Crash Course" %}
        <div class="col-md-4 mb-3">
            <div class="card dhht-card border-dark text-center h-100">
                <div class="card-header pt-3">
                    <a href="{{ site.baseurl }}{{ sectionloop.permalink }}">
                        <h3 class="card-title">{{ sectionloop.title }}</h3>
                    </a>
                </div>
                <div class="card-body">
                <h2>Lessons</h2>
                {% for individuallessons in site.lessons %}{% if individuallessons.layout == "sublesson" %}{% if individuallessons.group == sectionloop.group %}{% if individuallessons.firstlesson == "true" %}
                    <p class="card-text"><a href="{{ site.baseurl }}{{ individuallessons.permalink }}">{{ individuallessons.lessontitle }}</a></p>{% endif %}{% endif %}{% endif %}{% endfor %}
                </div>
            </div>
        </div>
        {% endunless %}
    {% endfor %}
</div>
