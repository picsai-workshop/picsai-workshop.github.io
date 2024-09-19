---
layout: about
title: About
permalink: /
subtitle: Probability, Information, Combinatorics, and AI Symposium, Monday-Saturday, 22-28 of September 2024</a>. Paestum, Italy.

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

# display_categories: [participant]
speaker_horizontal: false
organizer_horizontal: true
---


<p>The Probability, Information, Combinatorics, and AI Symposium
welcomes researchers and practitioners to Paestum, Italy this
September for a focused exploration of the interplay between these
foundational fields. This symposium will provide a platform for
the dissemination of cutting-edge research and the fostering of
interdisciplinary collaboration through a series of invited talks
by leading experts in their respective fields. </p>

<br>
<br>

<h2>Symposium Highlights</h2>

<br>
<br>

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
---

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        <h3 style="text-align:center;"></h3>
        {% include figure.liquid loading="eager" path="assets/img/panel_watercolor.jpg" title="Talks image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        <h3 style="text-align:center;"></h3>
        {% include figure.liquid loading="eager" path="assets/img/ideas_watercolor.jpg" title="Ideas image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        <h3 style="text-align:center;"></h3>
        {% include figure.liquid loading="eager" path="assets/img/posters_watercolor.jpg" title="Posters image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

See the [schedule](/schedule) for details.

<!-- Speakers -->
<br>
<h1><b>Speakers and Participants</b></h1>

We are thrilled to have the following researchers and artists joining us for the event.

<div class="speakers">
{% if site.enable_speaker_categories and page.display_categories %}
  {% for category in page.display_categories %}
  <a id="{{ category }}" href=".#{{ category }}">
    <h2 class="category">{{ category }}</h2>
  </a>
  {% assign categorized_speakers = site.speakers | where: "category", category %}
  {% assign sorted_speakers = categorized_speakers | sort: "importance" %}
  {% if page.speaker_horizontal %}
  <div class="container">
    {% for speaker in sorted_speakers %}
      {% if forloop.index0 % 4 == 0 %}
        <div class="row row-cols-4"> {% endif %} 
          {% include speakers_horizontal.liquid %}
      {% if forloop.index % 4 == 0 or forloop.last %}
        </div> {% endif %}
    {% endfor %}
  </div>
  {% else %}
  <div class="d-flex flex-wrap"> 
    {% for speaker in sorted_speakers %}
      <div class="p-2 flex-grow-1 flex-basis-0" style="flex-basis: 25%;"> {%- include speakers.liquid %}</div>
    {% endfor %}
  </div>
  {% endif %}
  {% endfor %}

{% else %}

{% assign sorted_speakers = site.speakers | sort: "secondname" %}

  {% if page.speaker_horizontal %}

  <div class="container">
    {% for speaker in sorted_speakers %}
      {% if forloop.index0 % 4 == 0 %}
        <div class="row row-cols-4"> {% endif %}
        {% include speakers_horizontal.liquid %}
      {% if forloop.index % 4 == 0 or forloop.last %}
        </div> {% endif %}
    {% endfor %}
  </div>

{% else %}
  <div class="d-flex flex-wrap">
    {% for speaker in sorted_speakers %}
      <div class="p-2 flex-grow-0 flex-basis-0" style="flex-basis: 25%;">
        {%- include speakers.liquid %}
      </div>
    {% endfor %}
  </div>
{% endif %}
{% endif %}
</div>

<br>
<h1><b>Contact</b></h1>

You can reach us by email at [``picsai.workshop@gmail.com``](mailto:picsai.workshop@gmail.com).
