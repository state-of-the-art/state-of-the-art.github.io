---
title: Visit3D
excerpt: 3D site engine / example
header:
  image: /assets/images/projects/visit3d/header.jpg
  teaser: /assets/images/projects/visit3d/teaser.png
sidebar:
  - image: /assets/images/projects/visit3d/teaser.png
    image_alt: icon
  - title: Links
    text: |
      [GitHub](https://github.com/state-of-the-art/visit3d)
  - title: Stack
    text: JavaScript, HTML/CSS, BabylonJS, Golang, Python
  - title: Platforms
    text: Win/Lin/Mac + iOS/Android and major browsers
  - title: UI
    text: WebGL + HTML
gallery:
  - url: /assets/images/projects/visit3d/screenshot-01.jpg
    image_path: /assets/images/projects/visit3d/screenshot-01.jpg
    alt: "Linux/Chromium screenshot"
  - url: /assets/images/projects/visit3d/screenshot-02.jpg
    image_path: /assets/images/projects/visit3d/screenshot-02.jpg
    alt: "Android/Firefox screenshot"
  - url: /assets/images/projects/visit3d/screenshot-03.jpg
    image_path: /assets/images/projects/visit3d/screenshot-03.jpg
    alt: "Blender render of the main scene"
---

{% include gallery caption="The site screenshots and render pictures" %}

## Description

Visit3D is aimed to prepare a relatively simple starting point / example of creating 3d site. It
was prepared as an idea of game wedding invite site with huge territory that could be explored by
the visitor, but was shrinked down to one chapel location due to time restrictions.

## Authors

* Idea & realization: [Rabit](https://github.com/rabits)

## Features

* Uses only opensource tooling
* Supports Win/Lin/Mac + IOS/Android with Firefox/Chromium/Safari browsers (except for IE or Edge)
* Supports JWE/JWT invite links for personalized messages through templating
* Includes golang-based webserver for easy deployment
* Relatively easily customizable

## Build

The site consists of 2 parts - javascript static site and visit3d minimalistic golang server to
process the templates based on the user token (or absence of it).

You can find all the sources in the [GitHub](https://github.com/state-of-the-art/visit3d/)
repository and build your own site following the README.md build steps. After that it could be
deployed to any cloud provider (like GCP/AWS) with their load balancers or any other way suitable
for you to put your site in www.

## License

The repository and its contents are covered by `Apache v2.0`, so anyone can use it without any concerns.

If you have any changes you'd like to share, don't hesitate to make a pull-request and push them into
the original repository. Definitely no pressure though.

## Privacy policy

It's very important to save user private data and you can be sure: we are working on security
of our applications and improving it every day. No data could be sent somewhere without
user notification and his direct approval. This application will work standalone without
any internet connection and will not collect any user personal data anyway.
