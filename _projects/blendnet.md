---
title: BlendNet
excerpt: Blender addon and distributed rendering farm system with cloud dynamic provisioning
header:
  image: /assets/images/projects/blendnet/header.jpg
  teaser: /assets/images/projects/blendnet/teaser.png
sidebar:
  - image: /assets/images/projects/blendnet/teaser.png
    image_alt: icon
  - title: Links
    text: |
      [GitHub](https://github.com/state-of-the-art/BlendNet)
      [blenderartirsts](https://blenderartists.org/t/simple-cloud-rendering/1183255)
  - title: Stack
    text: Blender 2.80+, Python 3.7
  - title: Platforms
    text: Linux, MacOSX, Windows
  - title: UI
    text: Blender UI
gallery:
  - url: /assets/images/projects/blendnet/screenshot-01.jpg
    image_path: /assets/images/projects/blendnet/screenshot-01.jpg
    alt: "Preferences with BlendNet parameters and info"
  - url: /assets/images/projects/blendnet/screenshot-02.jpg
    image_path: /assets/images/projects/blendnet/screenshot-02.jpg
    alt: "Sent task to Manager and continue to work"
  - url: /assets/images/projects/blendnet/screenshot-03.jpg
    image_path: /assets/images/projects/blendnet/screenshot-03.jpg
    alt: "Switch to second task with opened preview window"
---

{% include gallery caption="Couple of screenshots" %}

## Description

Opensource Blender addon and distributed cloud rendering system.

## Authors

* Idea & realization: [Rabit](https://github.com/rabits)

## Usage

Please check out the wiki page: [Wiki](https://github.com/state-of-the-art/BlendNet/wiki)

## Requirements

* Blender >= 2.80
* GCP Provider: Google Cloud Platform project and google cloud sdk
* AWS Provider: Amazon Web Services account and aws cli v2
* Local Provider: no reqs

## Purpose

Existing blender addons, that enabling network rendering on a cluster of instances
are too complicated, not enough automated or too expensive. The solution is just
to use the existing cloud providers with their cheap preemptible instances costs
~3 times less than the regular ones.

For example `GCP` n1-highcpu-64 (**64 core 57.6GB RAM**) will cost you just
**$0.48 per hour**. Just imagine this - a quite complicated `Cycles engine` frame
will cost just $0.50.

## Overview

The system consists of 3 main parts:

* Addon - blender interface to simplify run and manage the tasks
* Manager - controls Agents, merges results, provides status to Addon
* Agent - worker of the system, rendering task, provides status to Manager

All the components are using HTTPS & Basic Auth to protect the connection.

Read more on the GitHub page: [README](https://github.com/state-of-the-art/BlendNet/)

### Features

* Dynamic preview - user can see the progress of rendering, picture updated every 5s (default)
* Non-destructive preview engine - you can close preview and open it again without interrupting
* Allow to create providers - right now supported local run & GCP
* Saves your money - if some resources are not needed right now - they will be terminated

## Plans

You can see all the feature requests/bugs on the github page:

* [Milestones](https://github.com/state-of-the-art/BlendNet/milestones)
* [Issues](https://github.com/state-of-the-art/BlendNet/issues)

### Tasks

* Use buckets to cache dependencies/results
* Cost estimation before rendering
* Distributed smoke baking (per-domain): it's hard to bake multiple domains - it requires one domain
  per bake, others should be turned off
* Allocating of preemptible GPU on the instances
* Detailed statistics to optimize the pipeline
* Simplify the setup process for the end-user
* Web interface to check the status

### OpenSource

This is an experimental project. The main goal is to test State of the Art philosophy in practice.

We would love to see independent developers working on the project's issues: for fun and interest
as well as for monetary compensation (say, attached to the tickets).

#### License

The repository and its contents are covered by `Apache v2.0`, so anyone can use it without any concerns.

If you have any changes you'd like to share, don't hesitate to make a pull-request and push them into
the original repository. Definitely no pressure though.

#### Build

There is no need to build the project, just download zip archive with the latest release from
[GitHub](https://github.com/state-of-the-art/BlendNet/releases) and install the addon using Blender
add-on installer.

## Privacy policy

It's very important to save user private data and you can be sure: we are working on security
of our applications and improving it every day. No data could be sent somewhere without
user notification and his direct approval. This application is using network connection
as minimum as possible to perform only the operations of its main purpose. All the
connections are secured by the wide using open standards. Any internet connection will not be
allowed to collect any user personal data anyway.
