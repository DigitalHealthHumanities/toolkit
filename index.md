---
type: page
---
{% include head.html %}

{% include heading.html %}

<div class="dhht-container d-flex flex-column">
    <h1>{{ site.title }}</h1>
    <h2><a href="{{ site.baseurl }}/lessons">Lessons</a></h2>
    <ul>
        {% for sectionloop in site.lessons %}
        {% if sectionloop.layout == "lessongroup" %}
        <li><a href="{{ site.baseurl }}{{ sectionloop.permalink }}">{{ sectionloop.title }}</a></li>
        {% endif %}
        {% endfor %}
    </ul>
    <h2>Digital Health Humanities White Paper</h2>
    {% for item in site.data.headings %}
        {% if item.title == "White Paper" %}
            <a href="{{ site.baseurl }}{{ item.permalink }}">{{ item.title }}</a>
        {% endif %}
    {% endfor %}
</div>



{% include footer.html %}
