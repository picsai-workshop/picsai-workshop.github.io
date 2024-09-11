---
layout: about
title: About
permalink: /
subtitle: AI, Probability, Information, and Combinatorics Symposium, Monday-Saturday, 22-28 of September 2024</a>. Paestum, Italy.

# profile:
#   align: right
#   image: prof_pic.jpg
#   image_circular: false # crops the image to make it circular
#   more_info: >
#     <p>555 your office number</p>
#     <p>123 your address street</p>
#     <p>Your City, State 12345</p>

news: false # includes a list of news items
selected_papers: false # includes a list of papers marked as "selected={true}"
social: false # includes social icons at the bottom of the page

display_categories: [lecturer, panelist]
speaker_horizontal: false
organizer_horizontal: true
---

<p>The AI, Probability, Information, and Combinatorics Symposium
welcomes researchers and practitioners to Paestum, Italy this
September for a focused exploration of the interplay between these
foundational fields. This symposium will provide a platform for
the dissemination of cutting-edge research and the fostering of
interdisciplinary collaboration through a series of invited talks
by leading experts in their respective fields. </p>

<h2>Symposium Highlights</h2>

<div class="track">
    <h3>Dual Tracks:</h3>
    <ul>
        <li>
            <h4>AI Track:</h4>
            <p>This track will delve into the theoretical
            underpinnings and practical applications of artificial
            intelligence, with a focus on learning theory, quantum
            algorithms, and language models.</p>
        </li>
        <li>
            <h4>Arts Track:</h4> 
            <p>This track will explore the fascinating
            intersection of AI and the arts, examining how machine
            learning and computational creativity are reshaping
            artistic expression.</p>
        </li>
    </ul>
</div>


<h2>Venue</h2>
<p>The symposium will be held in the historic town of Paestum,
Italy, renowned for its ancient Greek temples and stunning coastal
setting.</p>

---
<h2 style="text-align:center;">Highlights</h2>
---

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        <h3 style="text-align:center;">A panel to discuss the current state of RL</h3>
        {% include figure.liquid loading="eager" path="assets/img/panel_watercolor.jpg" title="Talks image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        <h3 style="text-align:center;">Idea track: send your problems</h3>
        {% include figure.liquid loading="eager" path="assets/img/ideas_watercolor.jpg" title="Ideas image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        <h3 style="text-align:center;">Research track: send your solutions</h3>
        {% include figure.liquid loading="eager" path="assets/img/posters_watercolor.jpg" title="Posters image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

See the [schedule](/schedule) for details.

<!-- Speakers -->
<br>
<h1><b>Speakers</b></h1>

We are thrilled to have the following researchers joining us for the event.

<div class="speakers">
{% if site.enable_speaker_categories and page.display_categories %}
  <!-- Display categorized speakers -->
  {% for category in page.display_categories %}
  <a id="{{ category }}" href=".#{{ category }}">
    <h2 class="category">{{ category }}</h2>
  </a>
  {% assign categorized_speakers = site.speakers | where: "category", category %}
  {% assign sorted_speakers = categorized_speakers | sort: "importance" %}
  <!-- Generate cards for each speaker -->
  {% if page.speaker_horizontal %}
  <div class="container">
    <div class="row row-cols-2">
    {% for speaker in sorted_speakers %}
      {% include speakers_horizontal.liquid %}
    {% endfor %}
    </div>
  </div>
  {% else %}
  <div class="d-flex justify-content-between">
    {% for speaker in sorted_speakers %}
      <div class="p-2">{% include speakers.liquid %}</div>
    {% endfor %}
  </div>
  {% endif %}
  {% endfor %}

{% else %}

<!-- Display speakers without categories -->

{% assign sorted_speakers = site.speakers | sort: "importance" %}

  <!-- Generate cards for each speaker -->

{% if page.speaker_horizontal %}

  <div class="container">
    <div class="row row-cols-2">
    {% for speaker in sorted_speakers %}
      {% include speakers_horizontal.liquid %}
    {% endfor %}
    </div>
  </div>
  {% else %}
  <div class="grid">
    {% for speaker in sorted_speakers %}
      {% include speakers.liquid %}
    {% endfor %}
  </div>
  {% endif %}
{% endif %}
</div>

<!-- <br> -->
<!-- <h1><b>Sponsors</b></h1> -->

<!-- Thanks to our sponsors for supporting the workshop. -->

<!-- <div class="row"> -->
<!--     <div class="col-sm mt-3 mt-md-0"> -->
<!--         {% include figure.liquid loading="eager" path="assets/img/GR_logo_horizontal.png" width="220" title="GR logo" class="img-fluid rounded z-depth-1" %} -->
<!--     </div> -->
<!-- </div> -->

<br>
<h1><b>Contact</b></h1>

You can reach us by email at [``picsai.workshop@gmail.com``](mailto:picsai.workshop@gmail.com).
