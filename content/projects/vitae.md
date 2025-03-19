---
type: "projects"
layout: "single"
title: "Vitae Comptabilite's Website"
date: 2025-02-27T3:12:58+05:30
draft: false
github_link: "https://github.com/felixcaronpare"
author: "Felix"
list: never
tags:
  - "Frontend"
  - "Web Development"
  - "Freelance"
  - "Typecript"
  - "React"
  - "Vite"
  - "Tailwind"
---

<div id="carouselExampleIndicators" class="carousel slide pb-4" data-bs-ride="carousel">
  <ol class="carousel-indicators">
    <li data-bs-target="#carouselExampleIndicators" data-bs-slide-to="0" class="active"></li>
    <li data-bs-target="#carouselExampleIndicators" data-bs-slide-to="1"></li>
    <li data-bs-target="#carouselExampleIndicators" data-bs-slide-to="2"></li>
    <li data-bs-target="#carouselExampleIndicators" data-bs-slide-to="3"></li>
  </ol>
  <div class="carousel-inner">
    <div class="carousel-item active">
      <img class="d-block w-100 carousel-img" src="/images/vitae/vitae-1.png" alt="First slide">
    </div>
    <div class="carousel-item">
      <img class="d-block w-100 carousel-img" src="/images/vitae/vitae-2.png" alt="Second slide">
    </div>
    <div class="carousel-item">
      <img class="d-block w-100 carousel-img" src="/images/vitae/vitae-3.png" alt="Third slide">
    </div>
    <div class="carousel-item">
      <img class="d-block w-100 carousel-img" src="/images/vitae/vitae-4.png" alt="fourth slide">
    </div>
    <div class="carousel-item">
      <img class="d-block w-100 carousel-img" src="/images/vitae/vitae-5.png" alt="fourth slide">
    </div>
    <div class="carousel-item">
      <img class="d-block w-100 carousel-img" src="/images/vitae/vitae-6.png" alt="fourth slide">
    </div>
  </div>
  <button class="carousel-control-prev" type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide="prev">
    <span class="carousel-control-prev-icon" aria-hidden="true"></span>
    <span class="visually-hidden">Previous</span>
  </button>
  <button class="carousel-control-next" type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide="next">
    <span class="carousel-control-next-icon" aria-hidden="true"></span>
    <span class="visually-hidden">Next</span>
  </button>
</div>

First, you can view the end result of this freelance project [**here**](https://vitaecomptabilite-alpha.netlify.app/).

This project is a solo freelance contract that I accomplished during 2025. **Vitae Comptabilite** is a Montreal (QC) based accounting business which is specialized in accounting for healthcare doctorate professionals such as physicians, dentists and more. Vitae Comptabilite wanted a website for their business with specific criterias in mind: a website that is elegant, has optimized page speed and is fully responsive.

To achieve this, I developed their website with a minimal stack of technologies which are reliable and performant. For a static website where render speed is prioritized, it was clear that the simpler the development stack, the better :

- Typescript + React for an industry standard modern development environment;
- Astro as a web framework due to its server-first optimized performance
- Vite for an extremely performant frontend build tool;
- TailwindCSS for simple styling needs;

The above stack allowed me to have a smooth and simple development experience which resulted in a beautiful and lightning fast website that was succesfully delivered ahead of schedule.

[**Feel free to visit Vitae Comptabilite's website, the end result of this project.**](https://vitaecomptabilite-alpha.netlify.app/)

<hr>

<!-- Bootstrap CSS -->
<link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha1/dist/css/bootstrap.min.css" rel="stylesheet">

<!-- Bootstrap JS (with Popper.js) -->
<script src="https://cdn.jsdelivr.net/npm/@popperjs/core@2.11.6/dist/umd/popper.min.js"></script>
<script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha1/dist/js/bootstrap.min.js"></script>

<style>
  .carousel-img {
    object-fit: cover; /* Ensures the image covers the container */
    height: 500px; /* Set a fixed height to maintain uniformity */
    width: 100%; /* Ensure it takes the full width of the container */
  }

  .carousel-control-prev-icon,
  .carousel-control-next-icon {
    background-color: CornflowerBlue; /* Make the arrows black to match the border */
  }
</style>
