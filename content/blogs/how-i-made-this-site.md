---
title: "How I made this portfolio"
date: 2025-02-25T3:48:58+05:30
draft: false
github_link: "https://github.com/felixcaronpare"
author: "Felix"
tags:
  - Web development
  - Frontend
  - Golang
  - Hugo
  - CI/CD
image: /images/blogs/how-i-made-this-site/head-image.jpg
description: ""
toc: 
---

**Keep it simple, stupid**

As I am starting to consider my next career move, it was high time I stopped procrastinating my personal website. With my experience in web development being largely aimed towards more heavy-duty stacks, one of my main priorities with this portfolio site was to come back to simpler roots:

- Simple to develop: this is a simple static website -- no need to have React and all the bells and whistles;
- Simple to deploy: No need for an IaaS cloud provider, [Github Pages](https://github.com/features/actions) should be plenty enough;
- Simple to update: the chosen solution needs to integrate with a very basic CI/CD pipeline.

For this reason, I looked for the first time into templating solutions and found [Hugo](https://gohugo.io/), and more specifically a theme called [Hugo-Profile](https://themes.gohugo.io/themes/hugo-profile/) which suits my needs beautifully.

While Hugo has its own quirks and takes a bit of time to get used to, this has been overall a great solution for me. Turns out not everything needs to be built with the same requirements as the most robust web applications ever, especially when you are making a static website with low traffic.

Using this theme has allowed me to focus on the content of the portfolio while spending minimal time on its UI/UX. Of course the interface wasn't 100% to my liking and required tweaks, but having such a complete base theme instead of a white page helped save a lot of time.

It also integrates beautifully with Github Actions to do the Hugo generations of the files that is necessary for CI/CD purposes.

<hr>