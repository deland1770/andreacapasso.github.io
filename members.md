---
layout: default
title: Members
---

<h1 style="text-align: center;margin-top:40px;">People</h1>

<hr style="margin-bottom:40px;">

<!-- Container set to 1100px max-width, fully responsive -->
<div style="max-width:1100px; width:100%; margin:0 auto; padding: 0 15px; box-sizing: border-box;">

<style>
.small-text {
  font-size: 15px;
  line-height: 1.35;
  color: #555;
}

.person-card {
  text-align: center;
  width: 100%;
}

.person-card h4 {
  font-size: 18px;
  margin-top: 10px;
  margin-bottom: 5px;
}

/* Card layout for 2, 3 & 4 items per row (LARGER DESKTOP SIZING) */
.person-card-md {
  max-width: 200px;
  margin: 0 auto;
}

.person-card-md img {
  width: 180px;
  max-width: 100%;
  height: 180px;
  object-fit: cover;
  border-radius: 50%;
  display: block;
  margin: 0 auto 12px auto;
  box-shadow: 0 4px 10px rgba(0,0,0,0.08);
}

/* Card layout for 5 items per row */
.person-card-sm {
  max-width: 170px;
  margin: 0 auto;
}

.person-card-sm img {
  width: 150px;
  max-width: 100%;
  height: 150px;
  object-fit: cover;
  border-radius: 50%;
  display: block;
  margin: 0 auto 12px auto;
  box-shadow: 0 4px 10px rgba(0,0,0,0.08);
}

/* Grids for fixed counts per row on desktop */
.people-grid-2 {
  display: grid;
  grid-template-columns: repeat(2, 200px);
  gap: 40px;
  justify-content: center;
}

.people-grid-3 {
  display: grid;
  grid-template-columns: repeat(3, 200px);
  gap: 40px;
  justify-content: center;
}

.people-grid-4 {
  display: grid;
  grid-template-columns: repeat(4, 200px);
  gap: 32px;
  justify-content: center;
}

.people-grid-5 {
  display: grid;
  grid-template-columns: repeat(5, 170px);
  gap: 24px;
  justify-content: center;
}

/* TABLET RESPONSIVE FIXES */
@media (max-width: 900px) {
  .people-grid-2,
  .people-grid-3,
  .people-grid-4,
  .people-grid-5 {
    grid-template-columns: repeat(3, minmax(160px, 1fr));
    gap: 25px;
  }
}

/* MOBILE RESPONSIVE ENHANCEMENTS */
@media (max-width: 600px) {
  .people-grid-2,
  .people-grid-3,
  .people-grid-4,
  .people-grid-5 {
    grid-template-columns: 1fr !important;
    gap: 35px !important;
  }
  
  .person-card-md img,
  .person-card-sm img {
    width: 180px !important;
    height: 180px !important;
  }

  .person-card h4 {
    font-size: 19px !important;
    margin-top: 10px !important;
    margin-bottom: 4px !important;
  }

  .small-text {
    font-size: 15px !important;
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

<br><br>

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
