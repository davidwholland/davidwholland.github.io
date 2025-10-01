---
layout: post
title:  "Day One: Docker Containers"
date:   2024-10-25 09:15:22 -0400
tags: docker dayone
---

Getting started docs are [here][getting-started].

Step 1: Install [Docker Desktop][docker-desktop].

Docker has an interesting first-run experience. If you aren't familiar with the concept of containers, it starts by creating a small container for you that runs a web app. It's a nice way to get your feet wet.

Multiple advertisement banners are shown at various points while running the app. Not a great look, but given their fairly generous allowances for small shops and indie developers, I guess it's hard to avoid.

Docker next walks you through building your first container. As instructed, I cloned a repo from GitHub to get started with, and then I ran this command:

`docker build -t welcome-to-docker .`

 Which then produced my first error:

`=> ERROR [internal] load metadata for docker.io/library/node:18-alpine`

Docker tried to load the base nodejs image called `18-alpine`. That operation failed. I'm guessing it has something to do with the security settings on my Mac.

[Sigh] It turns out that downloading the image from Docker won't work until you verify your email. I didn't see *that* mentioned anywhere, but moving on...

Everything worked pretty painlessly after that. Downloading and running other containers is straightforward, and the Docker Desktop app is well organized and fairly easy to navigate. 

Multi-container applications are next.

[getting-started]: https://docs.docker.com/get-started/
[docker-desktop]: https://docs.docker.com/desktop/install/mac-install/
