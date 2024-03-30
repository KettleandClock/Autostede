---
title: Parts List
author: Richard Chompff
date: 2024-03-14
category: Jekyll
layout: post
---

<div>
{% for row in site.data.parts_list %}
    {% for pair in row %}
        {% if forloop.first %}
            <h2>{{ pair[1] }}</h2>
        {% else %}
            <b>{{ pair[0] }}:</b> {{ pair[1] }}<br>
        {% endif %}
    {% endfor %}
{% endfor %}
</div>
