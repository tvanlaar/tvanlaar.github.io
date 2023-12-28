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
  link="[https://www.google.com/maps](https://www.google.com/maps/place/Naraghi+Hall+of+Science,+1+University+Cir,+Turlock,+CA+95382/@37.5231622,-120.8577629,17z/data=!3m1!4b1!4m6!3m5!1s0x8091071c023abbb1:0x495623f43bcd21f3!8m2!3d37.5231622!4d-120.855188!16s%2Fg%2F11g_r_4x_?entry=ttu)"
%}

{% include section.html %}

{% capture col1 %}

{%
  include figure.html
  image="images/photo.jpg"
  caption="Lorem ipsum"
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
