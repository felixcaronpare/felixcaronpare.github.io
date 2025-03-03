---
title: "Multiplayer backend"
date: 2025-02-27T3:12:58+05:30
draft: false
github_link: "https://github.com/felixcaronpare"
author: "Felix"
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
image: /images/blogs/multiplayer-netcode/head-image.jpg
description: ""
toc: 
---

**Learning advanced Server-Side and Netcode programming through multiplayer development**

For the past few months, I have been spending some time working on a passion project of mine -- a spiritual successor to *Guild Wars 1* built with Unreal Engine 5. GW1 is my favorite video game of all time and, since no similar game has ever come out, I decided to satisfy my cravings by working on a successor project of my own.
While the scope of the project is ridiculously large for a solo developer and the end result is unlikely to ever come to fruition, I am still having a blast working on it.

"Why?", you may ask.

Because apparently multiplayer games have a LOT in common with web development, and this side project is turning out to be a huge learning opportunity for advanced server-side and netcode programming.

In an online video game, one may create an account, then create characters in this account which he can view (character select screen), modify (gain power by playing the game), or delete if he so desires. If this sounds similar to your average CRUD service in a web application, it's because that's exactly what it is.

You want the game servers to handle all critical logic and give the client as little privileges as possible to avoid cheating and hacking. Sounds like standard web development security practices? Yep, you're right.

When playing the game, the client may interact with a game server which is, ideally, containerized for portability and hosted somewhere in the cloud. If many other clients want to join this same game server, you may need to scale up that server according to client demand. If this sounds like cloud orchestration infrastructure for web applications... you guessed it, you're right once again.

The crazy part is you can use a lot of the same tools for web development and for server-side game development. For instance, you CAN make a standard CRUD service for your game in whatever backend programming language you like that interacts with whatever database technology you prefer. In some sense, you can view an online game backend almost exactly the same as a web application backend, except that it interacts with a graphics rendering engine client instead of a web browser. For all the research I did on the subject, this is the sort of architecture you will usually find in modern multiplayer RPG's.

![architecture](/images/blogs/multiplayer-netcode/ht-architecture.jpg)

Also, You CAN containerize a game server with Docker and you CAN use Kubernetes to orchestrate your deployments (granted, this one requires a bit of tinkering with, so you may want to turn towards an open source project like [Agones](https://agones.dev/site/docs/), which provides custom K8 configurations to address game server specific needs).

There is, however, one fascinating area that is massively different for game and web development.

**Communication protocols.**

In web development, we can be somewhat loose with how efficiently we are transmiting data between services. For example, we can afford to use JSON for its human readability even though its not the fastest data transfering solution. Many browsers are unable to accept anything else than standard HTTP, so it is only natural to use that as our network protocol by default.

In online games, however, efficiency is everything. You may not bat an eye if your favorite social media is a tiny bit slower to load its components, but you WILL have a terrible experience in a video game if the data transfer logic is inefficient. JSON will add latency to everything your players do, so suddenly you are forced to look into different communication protocols you may have never heard about: [protobufs](https://protobuf.dev/overview/), Thrift, Captain proto, etc. HTTP/2 is built for performance and optimization over standard HTTP, so it is wise to look into that too. Then, there's also the massive subject of lag compensation, but that one gets way too technical for the scope of this blog post.

**So how am I adressing all these multiplayer gaming specific needs in my personal project?**

The first thing I did was install Unreal Engine 5, use one of their starter templates and built it into a Linux Server ready for deployment. This way I can tinker with the multiplayer side of the project immediately. I containerized it using Docker to make it portable, scalable and easier to deploy.

![containerized linux server with windows clients](/images/blogs/multiplayer-netcode/container-server.jpg)

Next, I wrote a simple CRUD microservice for managing Accounts that interacts with a PostgreSQL database (chosen for its scalability). I chose to write the microservice in Golang considering its one of the programming languages that offers the best performance for while still remaining low-complexity. I added [gRPC](https://grpc.io/about/) to the project, an amazing framework that allows me to easily use Protocol Buffers as a communication protocol in the backend to leverage its performance and built-in versioning. An API gateway is used to facilitate the transfer of the calls from the client.

 Finally, I installed Agones and gave the Linux Server the Kubernetes configurations necessary for the scaling and orchestration of a game server (which is an entire conversation in itself).

While this slice of programming barely scrapes the surface of all the development necessary for a full game, it is a working vertical slice which covers a functioning prototype from end to end.

Next up on the list is implementing the login UI, a character selection screen and start building the logic necessary to play around with a character (inventory, character statistics, skills, etc.)

More about this project soon!

<hr>