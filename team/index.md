---
title: Team
nav:
  order: 4
  tooltip: About our team
---

# {% include icon.html icon="fa-solid fa-users" %}Team

The best part of science is getting to work with talented folks who bring new ideas and perspectives. 

{% include section.html %}

## Current Members

{% include list.html data="members" component="portrait" filters="role: pi" %}
{% include list.html data="members" component="portrait" filters="role: ms" %}
{% include list.html data="members" component="portrait" filters="role: undergrad" %}
{% include list.html data="members" component="portrait" filters="role: mascot" %}

{% include section.html background="images/background.jpg" dark=true %}



{% include section.html %}

## Alumni
{% capture content %}

{% include list.html  data="members"  component="portrait"  filters="group: alum" %}

{% endcapture %}

{% include grid.html style="square" content=content %}
