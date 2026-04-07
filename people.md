---
layout: default
title: People
---

<h1 style="text-align: center;margin-top:40px;">People</h1>

<hr style="margin-bottom:40px;">

<div style="max-width:900px; margin:0 auto;">

<style>
.small-text {
  font-size: 14px;
}

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

/* Grid for 3 people per row */
.people-grid-3 {
  display: grid;
  grid-template-columns: repeat(3, 200px);
  gap: 40px;
  justify-content: center;
}

/* FIXED: flexible grid that keeps last row centered */
.people-grid-4 {
  display: grid;
  grid-template-columns: repeat(auto-fit, 200px);
  gap: 40px;
  justify-content: center;
}

/* Responsive */
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

<h2 style="text-align: center;">Researchers</h2>
<br>
<div class="people-grid-3">
  <div class="person-card">
    <img src="images/SV.jpg">
    <h4><b>Sushmitha Veeralingam</b></h4>
    <p class="small-text">Application & Systems Integration Engineer</p>
  </div>

  <div class="person-card">
    <img src="images/SK.jpg">
    <h4><b>Shusmitha Kyatam</b></h4>
    <p class="small-text">Application & Systems Integration Engineer</p>
  </div>

  <div class="person-card">
    <img src="images/Lisa.jpg">
    <h4><b>Lisa Buttò</b></h4>
    <p class="small-text">Research Assistant</p>
  </div>
</div>

<br>
<h2 style="text-align: center;">Students</h2>
<br>
<div class="people-grid-3">
  <div class="person-card">
    <img src="images/Vicente.jpg">
    <h4><b>Vicente Lopes</b></h4>
    <p class="small-text">Ph.D. Course</p>
  </div>

  <div class="person-card">
    <img src="images/Pedro.jpg">
    <h4><b>Pedro Silva</b></h4>
    <p class="small-text">Masters Course</p>
  </div>

  <div class="person-card">
    <img src="images/Gabriel.jpg">
    <h4><b>Gabriel Barbosa</b></h4>
    <p class="small-text">Masters Course</p>
  </div>
</div>

<br>
<h2 style="text-align: center;">Former Members</h2>
<br>
<div class="people-grid-4">
  <div class="person-card">
    <img src="images/Siva.jpg">
    <h4><b>Siva S. Nemala</b></h4>
    <p class="small-text">Application & Systems Integration Engineer</p>
  </div>

  <div class="person-card">
    <img src="images/Guilherme.jpg">
    <h4><b>Guilherme Araújo</b></h4>
    <p class="small-text">Masters Course</p>
  </div>

  <div class="person-card">
    <img src="images/Bea.jpg">
    <h4><b>Beatriz Silva</b></h4>
    <p class="small-text">Masters Course</p>
  </div>
  
  <div class="person-card">
    <img src="images/GabrielM.png">
    <h4><b>João Fernandes</b></h4>
    <p class="small-text">Masters Course</p>
  </div>
  
  <div class="person-card">
    <img src="images/GabrielM.png">
    <h4><b>Gabriel Moreira</b></h4>
    <p class="small-text">Masters Course</p>
  </div>
  
  <div class="person-card">
    <img src="images/Tiago.jpg">
    <h4><b>Tiago Abreu</b></h4>
    <p class="small-text">Masters Course</p>
  </div>
</div>

</div>
