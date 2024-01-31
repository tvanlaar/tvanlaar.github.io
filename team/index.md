---
title: Team
nav:
  order: 4
  tooltip: About our team
---

# {% include icon.html icon="fa-solid fa-users" %}Team

The best part of science is getting to work with talented folks who bring new ideas and perspectives. 

{% include section.html %}

{% include list.html data="members" component="portrait" filters="role: pi" %}
{% include list.html data="members" component="portrait" filters="role: ms" %}

{% include section.html background="images/background.jpg" dark=true %}



{% include section.html %}

{% capture content %}


{% endcapture %}

{% include grid.html style="square" content=content %}
