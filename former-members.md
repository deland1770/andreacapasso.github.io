---
layout: default
title: Former Members
---

<h1 style="text-align: center;margin-top:40px;">People</h1>

<hr style="margin-bottom:40px;">

<!-- Container set to 1000px max-width, fully responsive -->
<div style="max-width:1000px; width:100%; margin:0 auto; padding: 0 15px; box-sizing: border-box;">

<style>
.small-text {
  font-size: 13px;
  line-height: 1.3;
}

.person-card {
  text-align: center;
  width: 100%;
}

/* Card layout for 2, 3 & 4 items per row */
.person-card-md {
  max-width: 160px;
  margin: 0 auto;
}

.person-card-md img {
  width: 150px;
  max-width: 100%;
  height: 150px;
  object-fit: cover;
  border-radius: 50%;
  display: block;
  margin: 0 auto 10px auto;
}

/* Card layout for 5 items per row */
.person-card-sm {
  max-width: 130px;
  margin: 0 auto;
}

.person-card-sm img {
  width: 120px;
  max-width: 100%;
  height: 120px;
  object-fit: cover;
  border-radius: 50%;
  display: block;
  margin: 0 auto 10px auto;
}

/* Grids for fixed counts per row on desktop */
.people-grid-2 {
  display: grid;
  grid-template-columns: repeat(2, 160px);
  gap: 30px;
  justify-content: center;
}

.people-grid-3 {
  display: grid;
  grid-template-columns: repeat(3, 160px);
  gap: 50px;
  justify-content: center;
  margin-bottom: 30px;
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

/* STEP 3 RESPONSIVE FIXES FOR MOBILE & TABLETS */
@media (max-width: 850px) {
  .people-grid-2,
  .people-grid-3,
  .people-grid-4,
  .people-grid-5 {
    grid-template-columns: repeat(3, minmax(130px, 1fr));
    gap: 20px;
  }
}

@media (max-width: 600px) {
  .people-grid-2,
  .people-grid-3,
  .people-grid-4,
  .people-grid-5 {
    grid-template-columns: repeat(2, minmax(120px, 1fr));
    gap: 15px;
  }
  
  .person-card-md img,
  .person-card-sm img {
    width: 110px;
    height: 110px;
  }
}

@media (max-width: 400px) {
  .people-grid-2,
  .people-grid-3,
  .people-grid-4,
  .people-grid-5 {
    grid-template-columns: 1fr;
    gap: 20px;
  }
}
</style>

<h2 id="Former Members" style="text-align: center;">Former Members</h2>
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
