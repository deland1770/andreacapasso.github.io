---
layout: default
title: 2D Crystal Fab
---

<style>
/* Parent container to place items side-by-side on desktop, stacked on mobile */
.welcome-section {
  display: flex;
  flex-wrap: wrap; /* Allows wrapping on small screens */
  align-items: center;
  gap: 30px;
  max-width: 1000px;
  margin: 30px auto;
  width: 100%;
}

/* Left side: Slideshow Container */
.slideshow-container {
  flex: 1 1 300px;
  width: 100%;
  max-width: 500px;
  height: 340px;
  position: relative;
  overflow: hidden;
  border-radius: 8px;
  box-shadow: 0 4px 12px rgba(0,0,0,0.1);
  margin: 0 auto;
  background-color: #fafafa;
  transition: transform 0.25s ease-in-out, box-shadow 0.25s ease-in-out;
  cursor: pointer; /* Indicates clickability */
}

/* HOVER EFFECT ON SLIDESHOW (Matching News Page Style) */
.slideshow-container:hover {
  transform: translateY(-3px); /* Lifts the slideshow box slightly */
  box-shadow: 0 8px 20px rgba(0, 0, 0, 0.15); /* Soft drop shadow glow */
}

.mySlides {
  display: none;
  width: 100%;
  height: 100%;
}

.mySlides img {
  width: 100%;
  height: 100%;
  object-fit: contain;
  cursor: pointer;
  display: block;
  transition: transform 0.3s ease;
}

/* Slight image zoom effect on hover */
.slideshow-container:hover .mySlides img {
  transform: scale(1.02);
}

/* Right side: Welcome Text Container */
.welcome-text {
  flex: 1 1 300px;
  text-align: justify;
}

.welcome-text h2 {
  margin-top: 0;
}

/* Transition */
.fade {
  animation-name: blurFade;
  animation-duration: 1.2s;
}

@keyframes blurFade {
  from { filter: blur(6px); opacity: 0; }
  to { filter: blur(0px); opacity: 1; }
}

/* LIGHTBOX (MODAL) STYLES */
.lightbox-modal {
  display: none; 
  position: fixed;
  z-index: 10000;
  left: 0;
  top: 0;
  width: 100%;
  height: 100%;
  background-color: rgba(0, 0, 0, 0.85);
  justify-content: center;
  align-items: center;
}

.lightbox-content {
  max-width: 95%;
  max-height: 85vh;
  border-radius: 6px;
}

.lightbox-close {
  position: absolute;
  top: 15px;
  right: 25px;
  color: #ffffff;
  font-size: 35px;
  font-weight: bold;
  cursor: pointer;
}

/* Mobile Breakpoint Adjustments */
@media (max-width: 768px) {
  .welcome-section {
    flex-direction: column;
    gap: 20px;
  }

  .slideshow-container {
    max-width: 100%;
    height: 250px;
  }
}
</style>

<!-- SIDE-BY-SIDE SECTION -->
<div class="welcome-section">

  <!-- LEFT: SLIDESHOW CONTAINER -->
  <div class="slideshow-container">
    <div class="mySlides fade">
      <img src="images/2Dfab.png" alt="Photo 1" onclick="openLightbox(this.src)">
    </div>

    <div class="mySlides fade">
      <img src="images/LLIC.png" alt="Photo 2" onclick="openLightbox(this.src)">
    </div>

    <div class="mySlides fade">
      <img src="images/Vertical+Lateral_ECM.png" alt="Photo 3" onclick="openLightbox(this.src)">
    </div>
  </div>

  <!-- RIGHT: WELCOMING TEXT CONTAINER -->
  <div class="welcome-text">
    <h2><b>Welcome to the 2D Crystal Fab</b></h2>
    <p>
      We are an interdisciplinary research group focused on the synthesis, advanced characterization, and device integration of novel two-dimensional (2D) nanomaterials and heterostructures.
    </p>
    <p>
      Our lab explores cutting-edge applications spanning flexible electronics, memristive neural interfaces, sustainable energy storage, and bio-sensing technologies.
    </p>
  </div>

</div>

<!-- LIGHTBOX OVERLAY -->
<div id="lightbox" class="lightbox-modal" onclick="closeLightbox()">
  <span class="lightbox-close" onclick="closeLightbox()">&times;</span>
  <img id="lightbox-img" class="lightbox-content">
</div>

<!-- SCRIPT FOR AUTOMATIC SLIDESHOW & LIGHTBOX -->
<script>
let slideIndex = 0;
let slideTimer;
let isPaused = false;

showSlides();

function showSlides() {
  if (isPaused) return;

  let slides = document.getElementsByClassName("mySlides");
  for (let i = 0; i < slides.length; i++) {
    slides[i].style.display = "none";  
  }
  
  slideIndex++;
  if (slideIndex > slides.length) { slideIndex = 1; }    
  
  slides[slideIndex - 1].style.display = "block";  
  slideTimer = setTimeout(showSlides, 3500);
}

function openLightbox(imgSrc) {
  isPaused = true;
  clearTimeout(slideTimer);
  
  let lightbox = document.getElementById("lightbox");
  let lightboxImg = document.getElementById("lightbox-img");
  
  lightboxImg.src = imgSrc;
  lightbox.style.display = "flex";
}

function closeLightbox() {
  let lightbox = document.getElementById("lightbox");
  lightbox.style.display = "none";
  
  isPaused = false;
  showSlides();
}
</script>

{% comment %}
<!-- AUTOMATIC LATEST NEWS SECTION (COMMENTED OUT) -->
<h2 style="text-align:left; margin-top:30px;"><b>Latest News</b></h2>
<hr style="margin-bottom:20px;">

<div style="max-width:1100px; margin:0 auto;">
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
{% endcomment %}
