---
title: Stedepedia
author: Richard Chompff
date: 2024-03-14
category: Jekyll
layout: post
---

{% for row in site.data.stedepedia %}
    {% for pair in row %}
        {% if forloop.first %}
            ### {{ pair[1] }}
        {% else %}
            **{{ pair[0] }}:** {{ pair[1] }}
        {% endif %}
    {% endfor %}
{% endfor %}
