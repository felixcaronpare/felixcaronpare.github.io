---
type: "projects"
layout: "single"
title: "Ugram.uk"
date: 2025-02-27T3:12:58+05:30
draft: false
github_link: "https://github.com/felixcaronpare"
author: "Felix"
list: never
tags:
    - "Full stack"
    - "Backend"
    - "Frontend"
    - "Web Development"
    - "React"
    - "Typescript"
    - "NodeJS"
    - "PostgreSQL"
    - "AWS"
    - "Docker"
    - "Github Actions"
    - "Jest"
---
Ugram is a content sharing web application like Instagram. It is a full-stack project that uses modern industry standard technologies. Ugram was built as a group project for an advanced web development course. My personal contribution to the project was that of a full-stack developer, where I end-to-end programmed functionalities such as account management, hashtag implementation, content recommendation algorithms, and more. I implemented all logic for these features: React frontend, RESTful API and documentation, NodeJS backend, and database interaction through NestJS's ORM. Last but not least, I contributed to and reviewed the code of my peers on multiple other aspects of the project.

The project was built with a robust stack meant to reflect what is expected from a modern web applications:
- Typescript + React frontend ();
- Typescript + NodeJS backend (monolithic architecture, uses NestJS too);
- PostgreSQL database;
- Hosted on AWS and uses multiple of their services (EC2, Elastic Beanstalk, ECS, Cloudflare, etc.)
- Containerized application with Docker;
- Robust CI/CD using multiple Github Actions and automated unit tests (Jest);
- Google Analytics and Sentry implementation for monitoring and logging needs.

As of today, the project is no longer online.

<!-- Bootstrap Carousel HTML -->
<div id="carouselExampleIndicators" class="carousel slide pb-4" data-bs-ride="carousel">
  <ol class="carousel-indicators">
    <li data-bs-target="#carouselExampleIndicators" data-bs-slide-to="0" class="active"></li>
    <li data-bs-target="#carouselExampleIndicators" data-bs-slide-to="1"></li>
    <li data-bs-target="#carouselExampleIndicators" data-bs-slide-to="2"></li>
    <li data-bs-target="#carouselExampleIndicators" data-bs-slide-to="3"></li>
    <li data-bs-target="#carouselExampleIndicators" data-bs-slide-to="4"></li>
  </ol>
  <div class="carousel-inner">
    <div class="carousel-item active">
      <img class="d-block w-100 carousel-img" src="/images/ugram/ugram3.jpg" alt="First slide">
    </div>
    <div class="carousel-item">
      <img class="d-block w-100 carousel-img" src="/images/ugram/UGram1.4501738010288294de1a.png" alt="Second slide">
    </div>
    <div class="carousel-item">
      <img class="d-block w-100 carousel-img" src="/images/ugram/ugram2.jpg" alt="Third slide">
    </div>
    <div class="carousel-item">
      <img class="d-block w-100 carousel-img" src="/images/ugram/ugram4.jpg" alt="fourth slide">
    </div>
    <div class="carousel-item">
      <img class="d-block w-100 carousel-img" src="/images/ugram/ugram5.jpg" alt="fourth slide">
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

<hr>

<!-- Bootstrap CSS -->
<link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha1/dist/css/bootstrap.min.css" rel="stylesheet">

<!-- Bootstrap JS (with Popper.js) -->
<script src="https://cdn.jsdelivr.net/npm/@popperjs/core@2.11.6/dist/umd/popper.min.js"></script>
<script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha1/dist/js/bootstrap.min.js"></script>

<style>
  .carousel-img {
    object-fit: cover; /* Ensures the image covers the container */
    height: 800px; /* Set a fixed height to maintain uniformity */
    width: 100%; /* Ensure it takes the full width of the container */
  }

  .carousel-control-prev-icon,
  .carousel-control-next-icon {
    background-color: CornflowerBlue; /* Make the arrows black to match the border */
  }
</style>