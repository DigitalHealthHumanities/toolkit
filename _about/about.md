---
layout: default
permalink: /about
title: About the Advancing Digital Health Humanities Institute
---
# {{ page.title }}

Coming Soon!

## Meet Our Team
<div class="mt-3 mb-3">
    {% for individual in site.about %}
        {% if individual.association == "lead" %}
            {% include bio-card.html person=individual %}
        {% endif %}
    {% endfor %}
</div>

### Consultants
<div class="mt-3 mb-3">
    {% for consultant in site.about %}
        {% if consultant.association == "consultant" %}
            {% include bio-card.html person=consultant %}
        {% endif %}
    {% endfor %}
</div>

### Instructors and Presenters
<div class="mt-3 mb-3">
    {% for instructor in site.about %}
        {% if instructor.association == "instructor" %}
            {% include bio-card.html person=instructor %}   
        {% endif %}
    {% endfor %}
</div>

### Awardees
<div class="mt-3 mb-3">
    {% for awardee in site.about %}
        {% if awardee.association == "awardee" %}
            {% include bio-card.html person=awardee %}
        {% endif %}
    {% endfor %}
</div>
