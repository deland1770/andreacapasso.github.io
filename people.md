---
layout: default
title: People
---

<h1 style="text-align: center;margin-top:40px;">People</h1>

<hr style="margin-bottom:40px;">

<div style="max-width:900px; margin:0 auto;">

<style>
.small-text {
  font-size: 14px; /* adjust as needed */
}
</style>

<style>
/* Common styles for all person cards */
.person-card {
  text-align: center;
}

.person-card img {
  width: 180px;
  height: 180px;
  object-fit: cover;
  border-radius: 50%;
  display: block;
  margin: 0 auto 10px auto;
}

/* Grid for 3 people per row, centered */
.people-grid-3 {
  display: grid;
  grid-template-columns: repeat(3, 200px);
  gap: 40px;
  justify-content: center;
}

/* Grid for 4 people per row, centered */
.people-grid-4 {
  display: grid;
  grid-template-columns: repeat(4, 200px);
  gap: 40px;
  justify-content: center;
}

/* Optional: responsive adjustments for smaller screens */
@media (max-width: 900px) {
  .people-grid-3 {
    grid-template-columns: repeat(2, 200px);
  }
  .people-grid-4 {
    grid-template-columns: repeat(2, 200px);
  }
}

@media (max-width: 500px) {
  .people-grid-3,
  .people-grid-4 {
    grid-template-columns: 1fr;
  }
}
</style>

<h2 style="text-align: center;">Post-Doc</h2>
<br>
<div class="people-grid-3">
  <div class="person-card">
    <img src="images/SVg.jpg" alt="Person 1">
    <h4><b>Sushmitha Veeralingam</b></h4>
    <p class="small-text">Application & Systems Integration Engineer</p>
    <p class="small-text">2D Materials Fabrication</p>
  </div>

  <div class="person-card">
    <img src="images/SKg.jpg" alt="Person 2">
    <h4><b>Shusmitha Kyatam</b></h4>
    <p class="small-text">Application & Systems Integration Engineer</p>
    <p class="small-text">2D Materials Fabrication</p>
  </div>

  <div class="person-card">
    <img src="images/Lisa.jpg" alt="Person 3">
    <h4><b>Lisa Buttò</b></h4>
    <p class="small-text">Research Assistant</p>
    <p class="small-text">2D Materials Fabrication</p>
  </div>
</div>

<br>
<h2 style="text-align: center;">Students</h2>
<br>
<div class="people-grid-3">
  <div class="person-card">
    <img src="images/Vicente.jpg" alt="Person 4">
    <h4><b>Vicente Lopes</b></h4>
    <p class="small-text">Ph.D. Course</p>
    <p class="small-text">2D Materials Fabrication</p>
  </div>

  <div class="person-card">
    <img src="images/Pedro.jpg" alt="Person 5">
    <h4><b>Pedro Silva</b></h4>
    <p class="small-text">Masters Course</p>
    <p class="small-text">2D Materials Fabrication</p>
  </div>

  <div class="person-card">
    <img src="images/gabriel_barbosa.jpeg" alt="Person 6">
    <h4><b>Gabriel Barbosa</b></h4>
    <p class="small-text">Masters Course</p>
    <p class="small-text">2D Materials Fabrication</p>
  </div>
</div>
<br>
<h2 style="text-align: center;">Former Members</h2>
<br>
<div class="people-grid-4">
  <div class="person-card">
    <img src="images/Siva.jpg" alt="Person 7">
    <h4><b>Siva S. Nemala</b></h4>
    <p class="small-text">Application & Systems Integration Engineer</p>
    <p class="small-text">2D Materials Fabrication</p>
  </div>

  <div class="person-card">
    <img src="images/Guilherme.jpg" alt="Person 8">
    <h4><b>Guilherme Araújo</b></h4>
    <p class="small-text">Masters Course</p>
    <p class="small-text">2D Materials Fabrication</p>
  </div>

  <div class="person-card">
    <img src="images/Beatriz.png" alt="Person 9">
    <h4><b>Beatriz Silva</b></h4>
    <p class="small-text">Masters Course</p>
    <p class="small-text">2D Materials Fabrication</p>
  </div>

  <div class="person-card">
    <img src="images/Tiago.png" alt="Person 10">
    <h4>Tiago Abreu</h4>
    <p class="small-text">Masters Course</p>
    <p class="small-text">2D Materials Fabrication</p>
  </div>
</div>
