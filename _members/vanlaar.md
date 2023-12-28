---
name: Dr. Tricia Van Laar
image: images/photo.jpg
role: pi
aliases:
  - TA Van Laar
  - T Van Laar
  - Van Laar
  - Tricia Van Laar
  - Tricia A Van Laar
  - Tricia A. Van Laar
  - T. A. Van Laar
  - T. Van Laar
links:
  orcid: 0000-0002-4654-8501
---

Hi! I am Dr. Van Laar and this is my website.

## All papers featuring Dr. Van Laar:

{% capture content %}

{% include list.html data="citations" component="citation" filters="author: Tricia A. Van Laar" %}

{% endcapture %}

{% include grid.html content=content %}
