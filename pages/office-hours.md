---
layout: default
title: Office Hours
has_children: false
nav_order: 4
permalink: /office-hours/
---

{% assign variables = site.data[site.data_folder].variables %}
{% assign course_calendar = site.data[site.data_folder].course_calendar %}

## Contact Info

**Instructor** <br/> {{ variables.instructor.name }} - [{{ variables.instructor.email }}](mailto:{{ variables.instructor.email }})

**Teaching Assistants (TAs)**  
{% for ta in variables.teaching_assistants %}  
&nbsp;&nbsp;&nbsp;&nbsp;{{ ta.name }} - [{{ ta.email }}](mailto:{{ ta.email }})  
{% endfor %}

**Instructional Assistants (IAs)**  
{% for ia in variables.instructional_assistants %}  
&nbsp;&nbsp;&nbsp;&nbsp;{{ ia.name }} - [{{ ia.email }}](mailto:{{ ia.email }})  
{% endfor %}

<!-- {: .fs-3 } -->

# Office Hours

Office hours are a great place to personally interact. Beyond projects and course material, we are interested in your goals, career endeavors, and what you want to gain from COGS 9. Data Science is a rapidly changing field and there is always a lot to discuss!

<table style="table-layout: fixed; text-align: center; width: 100%;">
    <thead>
        <tr class="header">
            <th style="width: 40%;"> Staff </th>
            <th style="width: 30%;"> Day & Time </th>
            <th style="width: 30%;"> Location </th>
        </tr>
    </thead>
    <tbody>
        <!-- Instructor's Office Hours -->
        {% for oh in variables.instructor.office_hours %}
        <tr>
            <td> {{ variables.instructor.name }} </td>
            <td> {{ oh.day }} {{ oh.time }} </td>
            <td> {{ oh.location }} </td>
        </tr>
        {% endfor %}

        <!-- Teaching Assistants' Office Hours -->
        {% for ta in variables.teaching_assistants %}
            {% for oh in ta.office_hours %}
            <tr>
                <td> {{ ta.name }} </td>
                <td> {{ oh.day }} {{ oh.time }} </td>
                <td> {{ oh.location }} </td>
            </tr>
            {% endfor %}
        {% endfor %}

        <!-- Instructional Assistants' Office Hours -->
        {% for ia in variables.instructional_assistants %}
            {% for oh in ia.office_hours %}
            <tr>
                <td> {{ ia.name }} </td>
                <td> {{ oh.day }} {{ oh.time }} </td>
                <td> {{ oh.location }} </td>
            </tr>
            {% endfor %}
        {% endfor %}
    </tbody>
</table>

Zoom Links:
**[Dominic Burrows](https://ucsd.zoom.us/j/8134812385)**
**[Zhining](https://ucsd.zoom.us/j/6406707430?pwd=MnE3ek16UFVRRDZOL3FLekpUaGI0QT09)**
**[Qisen](https://ucsd.zoom.us/j/9154753966)**
**[Nicole](https://ucsd.zoom.us/j/95232938841)**
**[Ryan](https://ucsd.zoom.us/j/99152339794)**
**[Derek](https://ucsd.zoom.us/j/8992245079?omn=93563584893)**
**[Jiawei](https://uchealth.zoom.us/j/84325316380)**






{: .note .fs-3 }
If you are unable to join or are having other issues, please reach out before or after class (I try to get to class a few minutes early and can stay for a few minutes after, although I do teach a class right after this one so can't stay too long) or in the discussion sections.
