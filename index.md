---
layout: default
title: 2D Crystal Fab
---

<div style="text-align:center; margin-top:20px;">

<img src="images/AC.jpg" alt="Andrea Capasso" style="width:200px; border-radius:50%; margin-bottom:20px;">


<h1 style="margin-bottom:10px;">Andrea Capasso</h1>

<p style="font-size:18px; margin:0;">
<strong>Research Scientist – Principal Investigator </strong>

</p>

<p style="font-size:18px; margin:0;">
<strong> Head of Laboratory </strong> / 2D Crystal Fab
</p>

<p style="font-size:18px; margin:0;">
<strong> Coordinator </strong> / Transversal Line on Advanced Materials
</p>

<p style="font-size:18px; margin:0;">
International Iberian Nanotechnology Laboratory (INL), Braga, Portugal
</p>
<br>
<p style="font-size:18px; margin:0;">
<strong>Co-Lead</strong> / Working Group 4 – Electronics, IAM-I
</p>
<br>
<p style="font-size:18px; margin:0;">
<strong> Editor </strong> / Diamond and Related Materials (Elsevier)
</p>
<br>
<a href="mailto:andrea.capasso@inl.int">
  andrea.capasso@inl.int
</a> |
<a href="https://scholar.google.com/citations?user=lSos5ssAAAAJ&hl=pt-PT&oi=ao" target="_blank">
  Google Scholar
</a> |
<a href="https://orcid.org/0000-0003-0299-6764" target="_blank">
  Orcid
</a> |
<a href="https://inl.int/community/andrea-capasso/" target="_blank">
  inl.int
</a>


</div>


<h2 style="text-align:left; margin-top:10px;">Education</h2>
<hr style="margin-bottom:10px;">

<div style="display:grid; grid-template-columns:auto 1fr; row-gap:6px; column-gap:48px; max-width:700px;">

  <div style="text-align:justify; font-weight:bold;">Ph.D. 2012</div>
  <div style="text-align:justify;">Queensland University of Technology / Materials Science</div>
  <div style="text-align:justify; font-weight:bold;">Laurea (Integrated MSc) 2007 </div>
  <div style="text-align:justify;">University of Roma Tre / Electronic Engineering</div>

</div>

<h2 style="text-align:left; margin-top:10px;">Professional Experience</h2>
<hr style="margin-bottom:10px;">


<div style="display:grid; grid-template-columns:auto 1fr; row-gap:6px; column-gap:48px; max-width:700px;">


  <div style="text-align:justify;">Diamond and Related Materials / Editor</div>
<div style="text-align:justify; font-weight:bold;">2026 – present</div>

<div style="text-align:justify;">INL / Head of Laboratory, 2D Crystal Fab</div>
<div style="text-align:justify; font-weight:bold;">2025 – present</div>

<div style="text-align:justify;">IAM-I / Co-Lead, Working Group 4 – Electronics</div>
<div style="text-align:justify; font-weight:bold;">2025 – present</div>

<div style="text-align:justify;">INL / Coordinator, Transversal Line on Advanced Materials</div>
<div style="text-align:justify; font-weight:bold;">2025 – present</div>

<div style="text-align:justify;">University of Minho / Guest Lecturer</div>
<div style="text-align:justify; font-weight:bold;">2024 – present</div>

<div style="text-align:justify;">INL / Research Scientist – Principal Investigator</div>
<div style="text-align:justify; font-weight:bold;">2018 – present</div>

<div style="text-align:justify;">Yonsei University / Research Scientist</div>
<div style="text-align:justify; font-weight:bold;">2018</div>

<div style="text-align:justify;">Italian Institute of Technology / Researcher</div>
<div style="text-align:justify; font-weight:bold;">2014 – 2017</div>

<div style="text-align:justify;">ENEA Casaccia Research Centre / Research Fellow</div>
<div style="text-align:justify; font-weight:bold;">2013 – 2014</div>

<div style="text-align:justify;">Queensland University of Technology / Postdoctoral Research Fellow</div>
<div style="text-align:justify; font-weight:bold;">2011 – 2012</div>

</div>

<h2 style="text-align:left; margin-top:10px;">Selected Publications</h2>
<hr style="margin-bottom:10px;">

<li>
  “Stable Graphene Membranes for Selective Ion Transport and Emerging Contaminants Removal in Water” Advanced Functional Materials (2023) 
</li>

<li>
  “Bipolar Resistive Switching in 2D MoSe2 Grown by Atmospheric Pressure Chemical Vapor Deposition” ACS Applied Materials & Interfaces (2024)
</li>
 
<li>
  “Sustainable MXene Membranes for Ion Sieving and Antibacterial Water Purification” Journal of Membrane Science (2026)
</li>
 
<li>
  “Multifunctional Superhydrophobic TiB2@Ag Composite-Based Fabric with Broadband Solar Absorption for Efficient Anti-Icing and Photothermal De-Icing” Chemical Engineering Journal (2026) 
</li>


<br>
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





