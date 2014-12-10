---
title: 'Chichester street reflection'
layout: photo
option:
  - map-meta
category: photo
date: 2014-11-27 20:20
updated: 2014-11-28 03:07
drafted: 2014-03-23 12:34
unique-id: 2014-03-23:chichester-street-reflection
description: 'After the rain in Chichester, on a brief trip to England.'
image:
  - src: 2014-03-23-chichester-street-reflection-olivermakes-ccbync.jpg
    alt: 'Reflections from a puddle where a street meets a sidewalk'
    caption: 'After the rain in Chichester, West Sussex'
    date: 2014-03-23
    camera: 'Apple iPhone 5S'
    lens: 'iPhone f/2.2'
    focal: '4.12mm'
    aperture: 'f/2.2'
    shutter: '1/120'
    iso: 50
    location: 'Central Chichester, UK'
    latitude: 50.8387
    longitude: -0.7782
    zoom: 16
    description: 'VSCOcam m5 preset'
    aspect: '3:2'

---

<figure class="wide">
  <input type="radio" role="radio" name="shift0" class="shift-back" id="shift-back0">
  <input type="radio" role="radio" name="shift0" class="shift-overlay" id="shift-overlay0">
  <input type="radio" role="radio" name="shift0" class="shift-map" id="shift-map0">
  <div class="container" id="i0">
    <img
      src="{{ site.image-url }}/{{ page.image[0].src }}" 
      sizes="{{ site.wide-sizes }}"
      srcset="{% for srcset1440 in site.srcset1440 %}{{ site.image-url }}/{{ site.srcset1440[forloop.index0] }}/{{ page.image[0].src }} {{ site.srcset1440[forloop.index0] }}w{% if forloop.last == false %}, {% endif %}{% endfor %}"
       alt="{{ page.image[0].alt }}"
    >
    <label for="shift-back0" class="shift-back-label"><span class="inner">↼ back to photo</span></label>
    <label for="shift-overlay0" class="shift-overlay-label"></label>
    <div class="photo-meta overlay">
      {% if page.image[0].camera contains "iPhone 5S" %}
      {% include icon-iphone5s.html %}
      {% elsif page.image[0].camera contains "X-E2" %}
      {% include icon-fxe2.html %}
      {% endif %}
      <ul class="camera-details">
        <li>Camera: {{ page.image[0].camera }}</li>
        <li>Lens: {{ page.image[0].lens }} at {{ page.image[0].focal }}</li>
        <li>Exposure: {{ page.image[0].aperture }} | {{ page.image[0].shutter }} s | ISO {{ page.image[0].iso }}</li>
        <li>Date: {{ page.image[0].date }}</li>
        <li>Location: {{ page.image[0].location }}</li>
      </ul>
      <label for="shift-map0" class="shift-map-label">View map{% include icon-location.html %}</label>
    </div>
  </div>
  <figcaption>{{ page.image[0].caption | markdownify }}</figcaption>
</figure>