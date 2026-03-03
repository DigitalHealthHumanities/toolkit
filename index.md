---
type: page
---
{% include head.html %}

{% include heading.html %}

<div class="dhht-container d-flex flex-column">
    <h1>{{ site.title }}</h1>
    <p>{{ site.description }}</p>
    <h2>Lessons</h2>
    <div class="row">
        {% for sectionloop in site.lessons %}
        {% if sectionloop.layout == "lessongroup" %}
        <div class="col-md-4 mb-3">
            <div class="card dhht-card text-center h-100">
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
        <!-- <li><a href="{{ site.baseurl }}{{ sectionloop.permalink }}">{{ sectionloop.title }}</a></li>
        a href="{{ site.baseurl }}/lessons"> -->
        {% endif %}
        {% endfor %}
    </div>
    <h2>Digital Health Humanities White Paper</h2>
    {% for item in site.data.headings %}
        {% if item.title == "White Paper" %}
            <p><a href="{{ site.baseurl }}{{ item.permalink }}">{{ item.title }}</a></p>
        {% endif %}
    {% endfor %}
</div>



{% include footer.html %}
