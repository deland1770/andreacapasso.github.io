---
layout: default
title: 2D Crystal Fab
---


<!-- AUTOMATIC LATEST NEWS SECTION -->
<h2 style="text-align:left; margin-top:30px;">Latest News</h2>
<hr style="margin-bottom:20px;">

<div style="max-width:1000px; margin:0 auto;">
  {% for item in site.data.news limit:3 %}
  <div style="display:flex; align-items:center; gap:30px; margin-bottom:30px; border-bottom:1px solid #eee; padding-bottom:20px;">
    <!-- Text -->
    <div style="flex:3; min-width:0;">
      <h3 style="margin-top:0; margin-bottom:8px;">{{ item.title }}</h3>
      <p style="text-align: justify; margin-bottom:8px;">{{ item.description }}</p>
      <p style="font-size:14px; color:#777; margin:0;">{{ item.date }}</p>
    </div>
    <!-- Image -->
    {% if item.image %}
    <div style="flex:1; max-width:200px; height:150px; overflow:hidden;">
      <a href="{{ item.link | default: '#' }}" target="_blank">
        <img src="{{ item.image }}" alt="{{ item.title }}" style="width:100%; height:100%; object-fit:cover; border-radius:4px;">
      </a>
    </div>
    {% endif %}

  </div>
  {% endfor %}
</div>





