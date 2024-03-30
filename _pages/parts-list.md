---
title: Parts List
author: Richard Chompff
date: 2024-03-14
category: Jekyll
layout: post
---
# Styles

<div class="table-wrapper" markdown="block">

|Style|Bonus|Malus|
|:-:|:-:|:-:|
|Scrap|Power|Precision|
|Bulky|Power|Handling|
|Sleek|Handling|Power|
|Primal|Handling|Precision|
|Energy|Precision|Handling|
|Refined|Precision|Power|

</div>

# Frames
<div>
{% for row in site.data.Frames %}
    {% for pair in row %}
        {% if forloop.first %}
            <h2>{{ pair[1] }}</h2>
        {% else %}
            <b>{{ pair[0] }}:</b> {{ pair[1] }}<br>
        {% endif %}
    {% endfor %}
{% endfor %}
</div>
# Modules
<div>
{% for row in site.data.Modules %}
    {% for pair in row %}
        {% if forloop.first %}
            <h2>{{ pair[1] }}</h2>
        {% else %}
            <b>{{ pair[0] }}:</b> {{ pair[1] }}<br>
        {% endif %}
    {% endfor %}
{% endfor %}
</div>
