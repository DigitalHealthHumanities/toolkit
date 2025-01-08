---
permalink: /about
---
{% include heading.html %}
# About the Advancing Digital Health Humanities Institute

Add some stuff!

# Meet Our Team

{% for individual in site.about %}
{% if individual.association == "lead" %}
<a href="{{ site.baseurl }}{{ individual.permalink }}">{{ individual.name }}</a><br>
{{ individual.title }}
{% endif %}
{% endfor %}

## Consultants

{% for consultant in site.about %}
{% if consultant.association == "consultant" %}
<a href="{{ site.baseurl }}{{ consultant.permalink }}">{{ consultant.name }}</a><br>
{{ consultant.affiliation }}
{% endif %}
{% endfor %}

## Instructors and Presenters

{% for instructor in site.about %}
{% if instructor.association == "instructor" %}
<a href="{{ site.baseurl }}{{ instructor.permalink }}">{{ instructor.name }}</a><br>
{{ instructor.title }}{{ instructor.affiliation }}
{% endif %}
{% endfor %}

## Awardees

{% for awardee in site.about %}
{% if awardee.association == "awardee" %}
<a href="{{ site.baseurl }}{{ awardee.permalink }}">{{ awardee.name }}</a><br>
{{ awardee.affiliation }}
{% endif %}
{% endfor %}

{% include footer.html %}