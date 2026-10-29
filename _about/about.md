---
layout: default
permalink: /about
title: About the Advancing Digital Health Humanities Institute
---
# {{ page.title }}

The Advancing Digital Health Humanities Institute (ADHHI), hosted by the University of California, San Francisco (UCSF) and funded through the National Endowment for the Humanities Institutes for Advanced Topics in the Digital Humanities, gathers a cross-disciplinary cohort of scholars, community organizers, and practicing physicians to participate in a two-year program designed to introduce and orient researchers with humanistic and computational methods used by the digital health humanities.

## Meet Our Team

### Leads
<div class="mb-3">
    {% for individual in site.about %}
        {% if individual.association == "lead" %}
            {% include bio-card.html person=individual %}
        {% endif %}
    {% endfor %}
</div>

### Consultants
<div class="mb-3">
    {% for consultant in site.about %}
        {% if consultant.association == "consultant" %}
            {% include bio-card.html person=consultant %}
        {% endif %}
    {% endfor %}
</div>

### Instructors and Presenters
<div class="mb-3">
    {% for instructor in site.about %}
        {% if instructor.association == "instructor" %}
            {% include bio-card.html person=instructor %}   
        {% endif %}
    {% endfor %}
</div>

### Awardees
<div class="mb-3">
    {% for awardee in site.about %}
        {% if awardee.association == "awardee" %}
            {% include bio-card.html person=awardee %}
        {% endif %}
    {% endfor %}
</div>
