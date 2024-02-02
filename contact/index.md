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
  image="images/warrior.jpg"
  caption="Warrior Nation"
%}

{% endcapture %}

{% include cols.html col1=col1 col2=col2 %}

