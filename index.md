---
---

# Dr. Van Laar's Website

Here's where you can find information on my teaching and research...and other stuff I am interested in!
<br>
<br>
We are not currently recruiting any MS students, but interested undergraduates should email Dr. Van Laar with a CV and statement of why they'd like to join the group.

{% include section.html %}

## Highlights

{% capture text %}

If you're not able to access one of our publications, please email Dr. Van Laar (tvanlaar@csustan.edu) with the subject "Publication Request".

{%
  include button.html
  link="publications"
  text="See our publications"
  icon="fa-solid fa-arrow-right"
  flip=true
  style="bare"
%}

{% endcapture %}

{%
  include feature.html
  image="https://www.frontiersin.org/files/Articles/1027399/fevo-10-1027399-HTML/image_m/fevo-10-1027399-g002.jpg"
  link="publications"
  title="Our Publications"
  text=text
%}

{% capture text %}

Learn more about the research we're doing in the lab.

{%
  include button.html
  link="research"
  text="Browse our projects"
  icon="fa-solid fa-arrow-right"
  flip=true
  style="bare"
%}

{% endcapture %}

{%
  include feature.html
  image="images/siskin.jpg"
  link="projects"
  title="Our Projects"
  flip=true
  style="bare"
  text=text
%}

{% capture text %}

Exciting news about the lab!

{%
  include button.html
  link="news"
  text="Read the news"
  icon="fa-solid fa-arrow-right"
  flip=true
  style="bare"
%}

{% endcapture %}

{%
  include feature.html
  image="images/news.jpg"
  link="news"
  title="News"
  text=text
%}

{% capture text %}

The people who make the magic happen.

{%
  include button.html
  link="team"
  text="Meet our team"
  icon="fa-solid fa-arrow-right"
  flip=true
  style="bare"
%}

{% endcapture %}

{%
  include feature.html
  image="images/barney.jpg"
  link="team"
  title="Our Team"
  text=text
  flip=true
%}
