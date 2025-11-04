---
title: Team
nav:
  order: 4
  tooltip: About our team
---

# {% include icon.html icon="fa-solid fa-users" %}Team

The best part of science is getting to work with talented folks who bring new ideas and perspectives. 

{% include section.html %}

{%- comment -%}
Normalize site.data.members to an array of member objects even if the data file is a hash.
{%- endcomment -%}
{% assign members_all = site.data.members %}
{% if members_all and members_all.first and members_all.first[1] %}
  {%- comment -%} members_all is a hash (array of [key, value] pairs); convert to array of values {%- endcomment -%}
  {% assign tmp = "" | split: "" %}
  {% for pair in members_all %}
    {% assign tmp = tmp | concat: [pair[1]] %}
  {% endfor %}
  {% assign members_all = tmp %}
{% endif %}

{%- comment -%}
Build "current" (case-insensitive; works if group is a string or an array)
{%- endcomment -%}
{% assign current = members_all | where_exp: "d", "d.group and ( (d.group contains 'current') or (d.group | downcase) == 'current' )" %}

{%- comment -%}
Split by role (case-insensitive)
{%- endcomment -%}
{% assign current_pi         = current | where_exp: "d", "d.role and (d.role | downcase) == 'pi'" %}
{% assign current_ms         = current | where_exp: "d", "d.role and (d.role | downcase) == 'ms'" %}
{% assign current_undergrad  = current | where_exp: "d", "d.role and (d.role | downcase) == 'undergrad'" %}
{% assign current_mascot     = current | where_exp: "d", "d.role and (d.role | downcase) == 'mascot'" %}

{%- comment -%}
Debug (optional): uncomment to verify counts
<!-- debug: all={{ members_all | size }}, current={{ current | size }}, pi={{ current_pi | size }}, ms={{ current_ms | size }}, ug={{ current_undergrad | size }}, mascot={{ current_mascot | size }} -->
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
