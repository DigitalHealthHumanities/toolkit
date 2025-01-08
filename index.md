---
type: page
---
{% include heading.html %}

<h1><a href="{{ site.baseurl }}/lessons">Lessons</a></h1>
{% for sectionloop in site.lessons %}
{% if sectionloop.layout == "lessongroup" %}
<a href="{{ site.baseurl }}{{ sectionloop.permalink }}">{{ sectionloop.title }}</a>
{% endif %}
{% endfor %}

<h1>Digital Health Humanities White Paper</h1>
{% for item in site.data.headings %}
{% if item.title == "White Paper" %}
<a href="{{ site.baseurl }}{{ item.permalink }}">{{ item.title }}</a>
{% endif %}
{% endfor %}



{% include footer.html %}