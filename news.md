---
layout: default
title: News
---

<h1 style="text-align:center; margin-top:40px;">News</h1>
<hr>

<div style="max-width:900px; margin:0 auto;">

{% for post in site.posts %}
  <div style="display:flex; align-items:flex-start; margin-bottom:40px; border-bottom:1px solid #ddd; padding-bottom:20px;">

    <div style="flex:1; padding-right:20px;">
      <h2 style="margin:0 0 10px 0;">
        <a href="{{ post.url | relative_url }}" style="text-decoration:none; color:#000;">
          {{ post.title }}
        </a>
      </h2>

      <p style="margin:0 0 10px 0; color:#444;">
        {{ post.excerpt | strip_html | truncate: 300 }}
      </p>

      <p style="font-size:14px; color:#777; margin:0;">
        Andrea Capasso &nbsp;|&nbsp;
        {{ post.date | date: "%B %d, %Y" }}
      </p>
    </div>

    {% if post.image %}
    <div style="width:150px; height:150px; overflow:hidden; flex-shrink:0;">
      <img src="{{ post.image }}" alt="thumbnail"
           style="width:100%; height:100%; object-fit:cover; border-radius:4px;">
    </div>
    {% endif %}

  </div>
{% endfor %}

</div>
