---
type: "projects"
layout: "single"
title: "UE5 multiplayer RPG"
date: 2025-02-27T3:12:58+05:30
draft: false
github_link: "https://github.com/felixcaronpare"
author: "Felix"
list: never
tags:
  - Backend
  - Game development
  - Netcode
  - UE5
  - protobufs
  - gRPC
  - Golang
  - PostgreSQL
  - Docker
  - Kubernetes
---

In this project, I use the medium of online game development to learn more advanced server-side and netcode programming. As explained in my [**first blog post**](placeholder) about this project, web development and multiplayer game development have a lot in common. In fact, the whole backend of an online RPG can be made in a similar fashion to a web application, except that it interacts with a client that's on a graphics rendering engine instead of a web browser.

<!-- Bootstrap Carousel HTML -->
<div id="carouselExampleIndicators" class="carousel slide pb-4" data-bs-ride="carousel">
  <ol class="carousel-indicators">
    <li data-bs-target="#carouselExampleIndicators" data-bs-slide-to="0" class="active"></li>
    <li data-bs-target="#carouselExampleIndicators" data-bs-slide-to="1"></li>
    <li data-bs-target="#carouselExampleIndicators" data-bs-slide-to="2"></li>
  </ol>
  <div class="carousel-inner">
    <div class="carousel-item active">
      <img class="d-block w-100 carousel-img" src="/images/ht/container-server.jpg" alt="First slide">
    </div>
    <div class="carousel-item">
      <img class="d-block w-100 carousel-img" src="/images/ht/head-image.jpg" alt="Second slide">
    </div>
    <div class="carousel-item">
      <img class="d-block w-100 carousel-img" src="/images/ht/ht-architecture.jpg" alt="Third slide">
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

With that in mind, I am using this project to teach myself new architectural paradigms and specific technologies that I have been wanting to explore:
- Microservices backend architecture;
- Golang as the main backend development language;
- Protocol buffers as communication protocol facilitated by the [gRPC](https://grpc.io/about/) framework;
- PostgreSQL as the main database technology;
- Docker and kubernetes for deployment and orchestration, facilitated by the [Agones](https://agones.dev/site/docs/) framework;
- AWS deployment of services, API gateways and Lambda Functions.

[**See my blog post to learn more**](placeholder) about how learning multiplayer paradigms can help you become a better web developer.

<hr>

<!-- Bootstrap CSS -->
<link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha1/dist/css/bootstrap.min.css" rel="stylesheet">

<!-- Bootstrap JS (with Popper.js) -->
<script src="https://cdn.jsdelivr.net/npm/@popperjs/core@2.11.6/dist/umd/popper.min.js"></script>
<script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha1/dist/js/bootstrap.min.js"></script>

<style>
  .carousel-img {
    object-fit: cover; /* Ensures the image covers the container */
    height: 400px; /* Set a fixed height to maintain uniformity */
    width: 100%; /* Ensure it takes the full width of the container */
  }

    .carousel-control-prev-icon,
  .carousel-control-next-icon {
    background-color: CornflowerBlue; /* Make the arrows black to match the border */
  }
</style>