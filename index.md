---
layout: default
title: Digital Health Humanities Toolkit
---
<h1>{{ site.title }}</h1>
<div class="backsplash">
    <img src="assets/img/ADHHI/ADHHI_Draft7_Web.jpg" class="img-fluid banner-img mx-auto d-block" alt="Connected photographs of medical practitioners, researchers, and painting in front of lines of code."/>
</div>

<p>{{ site.description }}</p>

<p>Read the <a href="{{ site.baseurl }}/white-paper">White Paper</a></p>

{% assign sublessons = site.lessons | where: "layout", "sublesson" %}
{% assign introlessons = sublessons | where: "group", "intro" %}

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
                    <p class="card-text">{{ sectionloop.description }}</p>
                </div>
            </div>
        </div>
        {% endunless %}
    {% endfor %}
</div>
