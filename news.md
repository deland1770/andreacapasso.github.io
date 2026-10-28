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

/* Clickable Link Wrapper */
.news-link-wrapper {
  text-decoration: none !important;
  color: inherit !important;
  display: block;
  margin-bottom: 30px;
}

/* Individual News Card */
.news-item {
  display: flex;
  align-items: center;
  gap: 30px;
  border-bottom: 1px solid #ddd;
  padding: 15px 15px 25px 15px;
  border-radius: 8px;
  transition: all 0.25s ease-in-out;
  cursor: pointer; /* Pointer cursor indicates clickability */
}

/* HOVER EFFECTS */
.news-link-wrapper:hover .news-item {
  background-color: #fafafa; /* Subtle background tint */
  transform: translateY(-3px); /* Lifts the card slightly */
  box-shadow: 0 6px 16px rgba(0, 0, 0, 0.08); /* Soft drop shadow */
}

/* Text Section */
.news-text {
  flex: 3;
  min-width: 0;
}

.news-text h2 {
  margin-top: 0;
  margin-bottom: 12px;
  color: #222;
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

/* Image Wrapper */
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
  object-fit: contain;
  display: block;
  border-radius: 6px;
  transition: transform 0.3s ease;
}

/* Zoom effect on image on card hover */
.news-link-wrapper:hover .news-image-wrapper img {
  transform: scale(1.03);
}

/* MOBILE RESPONSIVE STYLES */
@media (max-width: 768px) {
  .news-item {
    flex-direction: column-reverse;
    align-items: stretch;
    gap: 15px;
    padding: 10px;
  }

  .news-image-wrapper {
    max-width: 100%;
    margin-bottom: 10px;
  }

  .news-image-wrapper img {
    max-height: 280px;
    object-fit: cover;
  }
}
</style>

  {% for item in site.data.news %}
  <a href="{{ item.link | default: '#' }}" target="_blank" class="news-link-wrapper">
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
        <img src="{{ item.image }}" alt="{{ item.title }}">
      </div>
      {% endif %}

  </div>
  </a>
  {% endfor %}

</div>
