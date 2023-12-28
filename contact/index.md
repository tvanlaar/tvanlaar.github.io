---
title: Contact
nav:
  order: 6
  tooltip: Email, address, and location
---

# {% include icon.html icon="fa-regular fa-envelope" %}Contact

Don't hesitate to reach out!

{%
  include button.html
  type="email"
  text="tvanlaar@csustan.edu"
  link="tvanlaar@csustan.edu"
%}
{%
  include button.html
  type="phone"
  text="(209) 667-3695"
  link="+1-209-667-3695"
%}
{%
  include button.html
  type="address"
  tooltip="Our location on Google Maps for easy navigation"
  link="https://maps.app.goo.gl/d4GG2KXfTB3aoRLZ6"
%}

{% include section.html %}

{% capture col1 %}

{%
  include figure.html
  image="images/naraghi.jpg"
  caption="Naraghi Hall of Science <br><span>&copy; Brad Peatross<span>"
%}

{% endcapture %}

{% capture col2 %}

{%
  include figure.html
  image="images/photo.jpg"
  caption="Lorem ipsum"
%}

{% endcapture %}

{% include cols.html col1=col1 col2=col2 %}

{% include section.html dark=true %}

<iframe src="https://docs.google.com/forms/d/e/1FAIpQLSfer90Pr4p8lnh1Ua1MXuj_e9UH4UFCfxcArATQrYs8b_OytQ/viewform?embedded=true" width="640" height="1036" frameborder="0" marginheight="0" marginwidth="0">Loading…</iframe>

{% include section.html %}

{% capture col1 %}
Lorem ipsum dolor sit amet  
consectetur adipiscing elit  
sed do eiusmod tempor
{% endcapture %}

{% capture col2 %}
Lorem ipsum dolor sit amet  
consectetur adipiscing elit  
sed do eiusmod tempor
{% endcapture %}

{% capture col3 %}
Lorem ipsum dolor sit amet  
consectetur adipiscing elit  
sed do eiusmod tempor
{% endcapture %}

{% include cols.html col1=col1 col2=col2 col3=col3 %}
