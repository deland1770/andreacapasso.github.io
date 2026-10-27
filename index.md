---
layout: default
title: 2D Crystal Fab
---

<style>
/* Parent container to place items side-by-side */
.welcome-section {
  display: flex;
  align-items: center;
  gap: 40px;
  max-width: 1000px;
  margin: 30px auto;
}

/* Left side: Slideshow Container */
.slideshow-container {
  flex: 1; /* Takes up equal/proportionate space */
  max-width: 500px; /* Adjust width as needed */
  height: 350px; /* Adjust height as needed */
  position: relative;
  overflow: hidden;
  border-radius: 8px;
  box-shadow: 0 4px 12px rgba(0,0,0,0.1);
}

.mySlides {
  display: none;
  width: 100%;
  height: 100%;
}

.mySlides img {
  width: 100%;
  height: 100%;
  object-fit: cover;
}

/* Right side: Welcome Text Container */
.welcome-text {
  flex: 1; /* Takes up equal/proportionate space */
  text-align: justify;
}

.welcome-text h2 {
  margin-top: 0;
}

/* Fade animation */
.fade {
  animation-name: fade;
  animation-duration: 1.5s;
}

@keyframes fade {
  from {opacity: .4} 
  to {opacity: 1}
}

/* Mobile responsiveness: stacks vertically on small screens */
@media (max-width: 768px) {
  .welcome-section {
    flex-direction: column;
  }
  .slideshow-container {
    width: 100%;
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
      <img src="images/NEUROMORPHIC WEBSITE.png" alt="Photo 1">
    </div>

  <div class="mySlides fade">
      <img src="images/SENSING AND BIOELECTRONICS WEBSITE.png" alt="Photo 2">
    </div>

  <div class="mySlides fade">
      <img src="images/Cover_Advanced.jpg" alt="Photo 3">
    </div>
  </div>

  <!-- RIGHT: WELCOMING TEXT CONTAINER -->
  <div class="welcome-text">
    <h2>Welcome to 2D Crystal Fab</h2>
    <p>
      We are an interdisciplinary research group focused on the synthesis, advanced characterization, and device integration of novel two-dimensional (2D) nanomaterials and heterostructures.
    </p>
    <p>
      Our lab explores cutting-edge applications spanning flexible electronics, memristive neural interfaces, sustainable energy storage, and bio-sensing technologies.
    </p>
  </div>

</div>

<!-- SCRIPT FOR AUTOMATIC SLIDESHOW -->
<script>
let slideIndex = 0;
showSlides();

function showSlides() {
  let i;
  let slides = document.getElementsByClassName("mySlides");
  
  for (i = 0; i < slides.length; i++) {
    slides[i].style.display = "none";  
  }
  
  slideIndex++;
  if (slideIndex > slides.length) {slideIndex = 1}    
  
  slides[slideIndex-1].style.display = "block";  
  setTimeout(showSlides, 3500); // Changes image every 3.5 seconds
}
</script>



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





