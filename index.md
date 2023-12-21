---
---

# Dr. Van Laar's Website

Here's where you can find information on my teaching and research...and other stuff I am interested in!
<br>
<br>
We are currently recruiting one MS Biology student to begin in the Fall of 2024. This is an NSF-funded project in collaboration with Dr. Slade at Fresno State. The student will ne doing metagenomics on samples from 4 species of cardueline finches. No bioinformatics experience is necessary. Please contact Dr. Van Laar prior to applying for the program.

{% include section.html %}

## Highlights

{% capture text %}

If you're not able to access one of our publications, please email Dr. Van Laar (tvanlaar@csustan.edu) with the subject "Publication Request".

{%
  include button.html
  link="research"
  text="See our publications"
  icon="fa-solid fa-arrow-right"
  flip=true
  style="bare"
%}

{% endcapture %}

{%
  include feature.html
  image="images/photo.jpg"
  link="research"
  title="Our Publications"
  text=text
%}

{% capture text %}

Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.

{%
  include button.html
  link="projects"
  text="Browse our projects"
  icon="fa-solid fa-arrow-right"
  flip=true
  style="bare"
%}

{% endcapture %}

{%
  include feature.html
  image="images/photo.jpg"
  link="projects"
  title="Our Projects"
  flip=true
  style="bare"
  text=text
%}

{% capture text %}

Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.

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
  image="images/photo.jpg"
  link="team"
  title="Our Team"
  text=text
%}
