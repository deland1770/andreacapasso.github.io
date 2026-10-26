---
layout: default
title: People
---

<h1 style="text-align: center;margin-top:40px;">People</h1>

<hr style="margin-bottom:40px;">

<!-- Container set to 1000px to give 5 items comfortable breathing room -->
<div style="max-width:1000px; margin:0 auto; padding: 0 20px;">

<style>
.small-text {
  font-size: 13px;
  line-height: 1.3;
}

.person-card {
  text-align: center;
}

/* Card layout for 2, 3 & 4 items per row */
.person-card-md {
  width: 160px;
}

.person-card-md img {
  width: 150px;
  height: 150px;
  object-fit: cover;
  border-radius: 50%;
  display: block;
  margin: 0 auto 10px auto;
}

/* Card layout for 5 items per row */
.person-card-sm {
  width: 130px;
}

.person-card-sm img {
  width: 120px;
  height: 120px;
  object-fit: cover;
  border-radius: 50%;
  display: block;
  margin: 0 auto 10px auto;
}

/* Grids for fixed counts per row */
.people-grid-2 {
  display: grid;
  grid-template-columns: repeat(2, 160px);
  gap: 30px;
  justify-content: center;
}

.people-grid-3 {
  display: grid;
  grid-template-columns: repeat(3, 160px);
  gap: 30px;
  justify-content: center;
}

.people-grid-4 {
  display: grid;
  grid-template-columns: repeat(4, 160px);
  gap: 24px;
  justify-content: center;
}

.people-grid-5 {
  display: grid;
  grid-template-columns: repeat(5, 130px);
  gap: 20px;
  justify-content: center;
}

/* Responsive collapse on smaller screens */
@media (max-width: 850px) {
  .people-grid-2,
  .people-grid-3,
  .people-grid-4,
  .people-grid-5 {
    grid-template-columns: repeat(3, 150px);
  }
}

@media (max-width: 600px) {
  .people-grid-2,
  .people-grid-3,
  .people-grid-4,
  .people-grid-5 {
    grid-template-columns: repeat(2, 140px);
  }
}

@media (max-width: 400px) {
  .people-grid-2,
  .people-grid-3,
  .people-grid-4,
  .people-grid-5 {
    grid-template-columns: 1fr;
  }
}
</style>

<h2 style="text-align: center;">Researchers</h2>
<br>

<div class="people-grid-4">
  <div class="person-card person-card-md">
    <img src="images/SV.jpg" alt="Sushmitha Veeralingam">
    <h4><b>Sushmitha Veeralingam</b></h4>
    <p class="small-text">Application & Systems Integration Engineer</p>
  </div>

  <div class="person-card person-card-md">
    <img src="images/SK.jpg" alt="Shusmitha Kyatam">
    <h4><b>Shusmitha Kyatam</b></h4>
    <p class="small-text">Application & Systems Integration Engineer</p>
  </div>

  <div class="person-card person-card-md">
    <img src="images/Siva.jpg" alt="Siva S. Nemala">
    <h4><b>Siva S. Nemala</b></h4>
    <p class="small-text">Application & Systems Integration Engineer</p>
  </div>

  <div class="person-card person-card-md">
    <img src="images/Lisa.jpg" alt="Lisa Buttò">
    <h4><b>Lisa Buttò</b></h4>
    <p class="small-text">Research Assistant</p>
  </div>
</div>

<br>
<h2 style="text-align: center;">Students</h2>
<br>

<div class="people-grid-2">
  <div class="person-card person-card-md">
    <img src="images/Vicente.jpg" alt="Vicente Lopes">
    <h4><b>Vicente Lopes</b></h4>
    <p class="small-text">Ph.D. Course</p>
  </div>

  <div class="person-card person-card-md">
    <img src="images/Gabriel.jpg" alt="Gabriel Barbosa">
    <h4><b>Gabriel Barbosa</b></h4>
    <p class="small-text">Masters Course</p>
  </div>
</div>

<br>
<h2 style="text-align: center;">Former Members</h2>
<br>

<div class="people-grid-3">
  <div class="person-card person-card-md">
    <img src="images/Guilherme.jpg" alt="Guilherme Araújo">
    <h4><b>Guilherme Araújo</b></h4>
    <p class="small-text">Masters Course</p>
  </div>

  <div class="person-card person-card-md">
    <img src="images/Bea.jpg" alt="Beatriz Silva">
    <h4><b>Beatriz Silva</b></h4>
    <p class="small-text">Masters Course</p>
  </div>

  <div class="person-card person-card-md">
    <img src="images/joao_Fernandes.png" alt="João Fernandes">
    <h4><b>João Fernandes</b></h4>
    <p class="small-text">Masters Course</p>
  </div>
  
</div>

<div class="people-grid-3">
  <div class="person-card person-card-md">
    <img src="images/GabrielM.png" alt="Gabriel Moreira">
    <h4><b>Gabriel Moreira</b></h4>
    <p class="small-text">Masters Course</p>
  </div>

  <div class="person-card person-card-md">
    <img src="images/Tiago.jpg" alt="Tiago Abreu">
    <h4><b>Tiago Abreu</b></h4>
    <p class="small-text">Masters Course</p>
  </div>

  <div class="person-card person-card-md">
    <img src="images/Pedro.jpg" alt="Pedro Silva">
    <h4><b>Pedro Silva</b></h4>
    <p class="small-text">Masters Course</p>
  </div>
</div>

</div>
