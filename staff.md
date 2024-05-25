---
layout: page
title: Staff
has_children: false
nav_order: 9
description: A listing of all the course staff members.
---

# Staff

<!-- Contact information for the course staff. -->

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

<!-- ---

## Help Room Schedule and Hours

Monday | 6:00pm to 8:00pm (EST)
Tuesday | 6:00pm to 8:00pm (EST)
Wednesday | 6:00pm to 8:00pm (EST)
Thursday | 6:00pm to 8:00pm (EST)
Friday | 6:00pm to 8:00pm (EST)
Saturday | No help room
Sunday | No help room

[Zoom link](https://msu.zoom.us/j/97204068191)

* Meeting ID: 972 0406 8191
* Passcode: 250641 -->