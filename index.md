---
type: page
title: Digital Health Humanities Toolkit
---
{% include head.html %}

<div class="dhht-container d-flex flex-column">
    <h1>{{ site.title }}</h1>
    <p>{{ site.description }}</p>
    <p>Read the <a href="{{ site.baseurl }}/white-paper">White Paper</a></p>
    <h2>Lessons</h2>
    <div class="row mt-2 mb-3">
    <!-- Pull lessongroups and generate cards -->
        {% assign lessongroups = site.lessons | where: "layout", "lessongroup" %}
        {% for sectionloop in lessongroups %}
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
        {% endfor %}
    </div>
</div>
