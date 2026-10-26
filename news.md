---
layout: default
title: News
---

<h1 style="text-align:center; margin-top:40px;">News</h1>
<hr style="margin-bottom:40px;">

<div style="max-width:1700px; margin:0 auto;">

  {% for item in site.data.news %}
  <div style="display:flex; align-items:center; gap:40px; margin-bottom:40px; border-bottom:1px solid #ddd; padding-bottom:20px;">
    <!-- Text -->
    <div style="flex:3; min-width:0;">
      <h2>{{ item.title }}</h2>
      <p style="text-align: justify;">
        {{ item.description }}
      </p>
      <p style="font-size:14px; color:#777;">
        {{ item.date }}
      </p>
    </div>
<!-- Image -->
    {% if item.image %}
    <div style="flex:1; max-width:200px; height:200px; overflow:hidden;">
      <a href="{{ item.link }}" target="_blank">
        <img src="{{ item.image }}" style="width:100%; height:100%; object-fit:cover;">
      </a>
    </div>
    {% endif %}

  </div>
  {% endfor %}

</div>
