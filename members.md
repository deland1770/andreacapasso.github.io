---
layout: default
title: Members
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

<h2 id="Researchers" style="text-align: center;">Researchers</h2>
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

<h2 id="Graduate" style="text-align: center;">Graduate</h2>
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

</div>
