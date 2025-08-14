---
layout: about
title: About PICSAI 2025
permalink: /
subtitle: Probability, Information, Combinatorics, and AI Symposium, 27 of September to 4 of October, 2025</a>. Alanya, Turkey.
edition: picsai2025

news: false
selected_papers: false
social: false

# display_categories: [participant]
speaker_horizontal: false
organizer_horizontal: true
---


<p>The second edition of the Probability, Information, Combinatorics, and AI Symposium welcomes researchers and practitioners to Alanya, Turkey this September for a focused exploration of the interplay between these foundational fields. This symposium will provide a platform for the dissemination of cutting-edge research and the fostering of interdisciplinary collaboration through a series of invited talks by leading experts in their respective fields. </p>

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
            <p>This track will delve into the theoretical underpinnings and practical applications of artificial intelligence, with a focus on learning theory, quantum algorithms, and language models.</p>
        </li>
        <li>
            <h4>Arts Track:</h4> 
            <p>This track will explore the fascinating intersection of AI and the arts, examining how machine learning and computational creativity are reshaping artistic expression.</p>
        </li>
    </ul>
</div>


<h2>Venue</h2>
<p>The symposium will be held in the town of Alanya, its beautiful beaches, rich history, and vibrant local culture.</p>

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        <h3 style="text-align:center;"></h3>
        {% include figure.liquid loading="eager" path="assets/img/tower_alanya.jpg" title="Ruins Paestum" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        <h3 style="text-align:center;"></h3>
        {% include figure.liquid loading="eager" path="assets/img/port_alanya.jpg" title="Beach Paestum" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

See the [schedule](/2025/schedule) for details.

<!-- Speakers -->
<br>
<h1><b>Speakers and Participants</b></h1>

We are thrilled to have the following researchers and artists joining us for the event.

<div class="speakers">
  {% assign 2025_speakers = site.speakers | where_exp: "item", "item.editions contains 'picsai2025'" %}
  {% assign sorted_speakers = 2025_speakers | sort: "importance" %}
  <div class="d-flex flex-wrap">
    {% for speaker in sorted_speakers %}
      <div class="p-2 flex-grow-0 flex-basis-0" style="flex-basis: 25%;">
        {%- include speakers.liquid %}
      </div>
    {% endfor %}
  </div>
</div>

<br>
<h1><b>Contact</b></h1>

You can reach us by email at [``picsai.workshop@gmail.com``](mailto:picsai.workshop@gmail.com).
