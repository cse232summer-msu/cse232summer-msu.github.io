---
layout: page
title: Staff
description: A listing of all the course staff members.
---

# Staff

Contact information and office hours for the course staff.

---

## Course Instructor

{% assign instructors = site.staffers | where: 'role', 'Course Instructor' %}

{% for staffer in instructors %}
{{ staffer }}
{% endfor %}

---

## Teaching Assistants

{% assign teaching_assistants = site.staffers | where: 'role', 'Teaching Assistant' %}
{% assign num_teaching_assistants = teaching_assistants | size %}
{% if num_teaching_assistants != 0 %}

{% for staffer in teaching_assistants %}
{{ staffer }}
{% endfor %}
{% endif %}

---

## Undergraduate Learning Assistants

{% assign undergraduate_learning_assistants = site.staffers | where: 'role', 'Undergraduate Learning Assistant' %}
{% assign num_undergraduate_learning_assistants = undergraduate_learning_assistants | size %}
{% if num_undergraduate_learning_assistants != 0 %}

{% for staffer in undergraduate_learning_assistants %}
{{ staffer }}
{% endfor %}
{% endif %}