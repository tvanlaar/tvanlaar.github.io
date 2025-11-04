---
title: Team
nav:
  order: 4
  tooltip: About our team
---

# {% include icon.html icon="fa-solid fa-users" %}Team

The best part of science is getting to work with talented folks who bring new ideas and perspectives. 

{% include section.html %}

{% assign current = site.data.members | where: "group", "current" %}
{% assign current_pi = current | where: "role", "pi" %}
{% assign current_ms = current | where: "role", "ms" %}
{% assign current_undergrad = current | where: "role", "undergrad" %}
{% assign current_mascot = current | where: "role", "mascot" %}

## Current Members
{% include list.html records=current_pi component="portrait" %}
{% include list.html records=current_ms component="portrait" %}
{% include list.html records=current_undergrad component="portrait" %}
{% include list.html records=current_mascot component="portrait" %}

{% include section.html background="images/background.jpg" dark=true %}

{% include section.html %}

## Alumni
{% capture content %}

{% include list.html  data="members"  component="portrait"  filters="group: alum" %}

{% endcapture %}

{% include grid.html style="square" content=content %}
