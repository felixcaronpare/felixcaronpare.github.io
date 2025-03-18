---
type: "projects"
layout: "single"
title: "UFood"
date: 2025-02-27T3:12:58+05:30
draft: false
github_link: "https://github.com/felixcaronpare"
author: "Felix"
list: never
tags:
  - "Frontend"
  - "Web Development"
  - "Javascript"
  - "VueJS"
  - "HTML/CSS"
  - "Google Maps Javascript API"
---

This project is a restaurant searching and reviewing social media application. It has an authentification token system that uses OAuth, a landing page that fetches all relevant data from the [provided database](https://github.com/GLO3102/UFood?tab=readme-ov-file) from the project specifications with a custom-built API, Google Maps imbeds to allow users to search for nearby restaurants and get directions, and many more features.

<!-- Bootstrap Carousel HTML -->
<div id="carouselExampleIndicators" class="carousel slide pb-4" data-bs-ride="carousel">
  <ol class="carousel-indicators">
    <li data-bs-target="#carouselExampleIndicators" data-bs-slide-to="0" class="active"></li>
    <li data-bs-target="#carouselExampleIndicators" data-bs-slide-to="1"></li>
    <li data-bs-target="#carouselExampleIndicators" data-bs-slide-to="2"></li>
    <li data-bs-target="#carouselExampleIndicators" data-bs-slide-to="3"></li>
  </ol>
  <div class="carousel-inner">
    <div class="carousel-item active">
      <img class="d-block w-100 carousel-img" src="/images/ufood/ufood1.png" alt="First slide">
    </div>
    <div class="carousel-item">
      <img class="d-block w-100 carousel-img" src="/images/ufood/UFood1.89dd8bfdcf1ebb3f0baa.png" alt="Second slide">
    </div>
    <div class="carousel-item">
      <img class="d-block w-100 carousel-img" src="/images/ufood/ufood3.jpg" alt="Third slide">
    </div>
    <div class="carousel-item">
      <img class="d-block w-100 carousel-img" src="/images/ufood/ufood4.jpg" alt="fourth slide">
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

The project was built with a simpler stack of technologies, as the requirements were not too complex and the project was meant as an introduction to web application development:

- Javacript;
- VueJS as the frontend development framework;
- Vuetify as the visual framework;
- Google Maps Javascript API for map embeds.

Although the project is not hosted online anymore, you can [**view the source code of the project here**](placeholder).

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
