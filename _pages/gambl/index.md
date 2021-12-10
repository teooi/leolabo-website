
---
layout: page
title: GAMBL
permalink: /gambl/
toggle: on
rank: 9
---

<div style="margin-bottom: 50px;">
    <img class="float-right" width="50%" src="{{ 'projects/wordcloud.png' | prepend: site.images_dir | prepend: site.baseurl }}" />
</div>
<div class="lab-wrapper">
    <ul class="lab-list">
    <!-- Current PIs -->
    {% for member in site.data.team %}
        {% if member.is_current and member.is_pi %}
            {% if member.name and member.bio %}
                {% include member.html %}
            {% endif %}
        {% endif %}
    {% endfor %}
    <!-- Current non-PIs -->
    {% for member in site.data.team %}
        {% if member.is_current and member.is_pi == false %}
            {% if member.name and member.bio %}
                {% include member.html %}
            {% endif %}
        {% endif %}
    {% endfor %}
    <!-- Non-current (alumni) -->
    {% assign alumni_size = site.data.team | size %}
    {% if alumni_size > 0 %}
        <h1 class="post-title">Alumni</h1>
        {% for member in site.data.team %}
            {% if member.is_current == false %}
                {% if member.name and member.bio %}
                    {% include member.html %}
                {% endif %}
            {% endif %}
        {% endfor %}
    {% endif %}
    </ul>
</div>
