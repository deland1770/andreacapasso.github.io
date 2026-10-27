---
layout: default
title: News
---

<h1 style="text-align:center; margin-top:40px;">News</h1>
<hr style="margin-bottom:40px;">

<div class="news-container">

<style>
/* Main Container */
.news-container {
  max-width: 1100px;
  width: 100%;
  margin: 0 auto;
  padding: 0 15px;
  box-sizing: border-box;
}

/* Individual News Card */
.news-item {
  display: flex;
  align-items: center;
  gap: 30px;
  margin-bottom: 40px;
  border-bottom: 1px solid #ddd;
  padding-bottom: 25px;
}

/* Text Section */
.news-text {
  flex: 3;
  min-width: 0;
}

.news-text h2 {
  margin-top: 0;
  margin-bottom: 12px;
}

.news-text p {
  text-align: justify;
  text-justify: inter-word;
  margin-bottom: 10px;
}

.news-date {
  font-size: 14px;
  color: #777;
  margin: 0;
}

/* Image Wrapper for Desktop - Natural aspect ratio without vertical cropping */
.news-image-wrapper {
  flex: 1;
  max-width: 250px;
  width: 100%;
  height: auto;
  border-radius: 6px;
  overflow: hidden;
}

.news-image-wrapper img {
  width: 100%;
  height: auto;
  max-height: 220px;
  object-fit: contain; /* Displays full image without cropping top/bottom */
  display: block;
  border-radius: 6px;
}

/* MOBILE RESPONSIVE STYLES */
@media (max-width: 768px) {
  .news-item {
    flex-direction: column-reverse; /* Image on top, text below */
    align-items: stretch;
    gap: 15px;
  }

  .news-image-wrapper {
    max-width: 100%;
    margin-bottom: 10px;
  }

  .news-image-wrapper img {
    max-height: 280px;
    object-fit: cover; /* Fills full banner width cleanly on mobile */
  }
}
</style>

  {% for item in site.data.news %}
  <div class="news-item">
    
    <!-- Text Content -->
  <div class="news-text">
      <h2>{{ item.title }}</h2>
      <p>{{ item.description }}</p>
      <p class="news-date">{{ item.date }}</p>
    </div>

    <!-- Image -->
  {% if item.image %}
    <div class="news-image-wrapper">
      <a href="{{ item.link | default: '#' }}" target="_blank">
        <img src="{{ item.image }}" alt="{{ item.title }}">
      </a>
    </div>
    {% endif %}

  </div>
  {% endfor %}

</div>
