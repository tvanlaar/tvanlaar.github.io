---
title: Team
nav:
  order: 4
  tooltip: About our team
---

# {% include icon.html icon="fa-solid fa-users" %}Team

The best part of science is getting to work with talented folks who bring new ideas and perspectives. 

{% include section.html %}

{%- comment -%} Use the MEMBERS COLLECTION, not data {%- endcomment -%}
{% assign current = site.members | where: "group", "current" %}

{%- comment -%} Role buckets (case-insensitive, in case of mixed casing) {%- endcomment -%}
{% assign current_pi         = current | where_exp: "d", "d.role and d.role | downcase == 'pi'" %}
{% assign current_ms         = current | where_exp: "d", "d.role and d.role | downcase == 'ms'" %}
{% assign current_undergrad  = current | where_exp: "d", "d.role and d.role | downcase == 'undergrad'" %}
{% assign current_mascot     = current | where_exp: "d", "d.role and d.role | downcase == 'mascot'" %}

{%- comment -%}
<!-- debug: all={{ site.members | size }}, current={{ current | size }}, pi={{ current_pi | size }}, ms={{ current_ms | size }}, ug={{ current_undergrad | size }}, mascot={{ current_mascot | size }} -->
{%- endcomment -%}

## Current Members
{% include list_records.html records=current_pi component="portrait" %}
{% include list_records.html records=current_ms component="portrait" %}
{% include list_records.html records=current_undergrad component="portrait" %}
{% include list_records.html records=current_mascot component="portrait" %}

{% include section.html background="images/background.jpg" dark=true %}

{% include section.html %}

## Alumni
{% capture content %}
{% include list.html data="members" component="portrait" filters="group: alum" %}
{% endcapture %}
{% include grid.html style="square" content=content %}
