---
type: page
---
{% include head.html %}

{% include heading.html %}

<div class="dhht-container d-flex flex-column">
    <h1>{{ site.title }}</h1>
    <p>{{ site.description }}</p>
    <p>Read the White Paper <a href="{{ site.baseurl }}/white-paper">here</a></p>
    <h2>Lessons</h2>
    <div class="row mt-2 mb-3">
    <!-- Pull lessongroups and generate cards -->
        {% assign lessongroups = site.lessons | where: "layout", "lessongroup" %}
        {% for sectionloop in lessongroups %}
        <div class="col-md-4 mb-3">
            <div class="card dhht-card border-dark text-center h-100">
                <div class="card-header pt-3">
                    <a href="{{ site.baseurl }}{{ sectionloop.permalink }}">
                        <h5 class="card-title">{{ sectionloop.title }}</h5>
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

{% include footer.html %}
