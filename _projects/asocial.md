---
title: aSocial
excerpt: Distributed p2p social network with full control over the information
header:
  image: /assets/images/projects/asocial/header.jpg
  teaser: /assets/images/projects/asocial/teaser.png
sidebar:
  - image: /assets/images/projects/asocial/teaser.png
    image_alt: icon
  - title: Links
    text: |
      [GitHub](https://github.com/state-of-the-art/asocial)
  - title: Stack
    text: C++, Qt 5.14
  - title: Platforms
    text: Linux, Android
  - title: UI
    text: Qt QML+js
gallery:
  - url: /assets/images/projects/asocial/ui_main.png
    image_path: /assets/images/projects/asocial/ui_main.png
    alt: "Main interface (design)"
---

{% include gallery caption="Available images" %}

## Description

**aSocial** - is a peer-to-peer distributed social network that gives you full control over your
social information.

## Authors

* Idea & realization: [Rabit](https://github.com/rabits)

## Usage

Please check out the wiki page: [Wiki](https://github.com/state-of-the-art/asocial/wiki)

## Requirements

* Host:
  * **Smartphone / Tablet** - anything with Android 5+ (Lollipop or better)
  * **Linux** - any distributive with Qt 5.15 support should work
* **aSocial** - application piece, binaries published in Android store and available on the GitHub
release page.

## Purpose

Existing social networks and messangers are centralized or proprietary and not allow to control your
information. So aSocial is aimed to provide the simple way to control how your information is stored
and how it's available for your contacts.

More about the project, it's main ideas, features and the most important mechanisms you can read in
the [aSocial blog post](/project/asocial/distributed/network/encryption/asocial-description/). 

### History

The project was started as typical social 12/28/2013 and mutated to distributed and found itself
10/17/2014. The POC was focused on UI, but some basic components were also prepared. Stopped due to
breaking Qt changes, not ready Lightning network (second layer of Bitcoin for microtransactions) and
overall project complexity was stopped 03/30/2016.

The origins are stored on [Rabit's project GitHub page](https://github.com/rabits/asocial.co).

### Features

Basic features of the social platform:

* *Modules* - add or remove components or use the other vendor component as plugin
* *History* - store not just dates of item, but also any edit of the items
* *Persons* - personal & legal entities, existing (with profiles) or imaginary
* *Events* - anything happened, happening, going to happen in the life
* *Messages* - monetized conversation threads or any other interaction like profile updates, news
* *Overlays* - your vision or additional information for existing or new entities, could be password
  protected
* *Synchronization* - make sure your devices replicates the information / profiles you have
* *Sharing* - ability to share your files with friends from any device you have

## Plans

You can see all the feature requests/bugs on the github page:

* [Milestones](https://github.com/state-of-the-art/asocial/milestones)
* [Issues](https://github.com/state-of-the-art/asocial/issues)

### OpenSource

This is an experimental project. The main goal is to test State of the Art philosophy in practice.

We would love to see independent developers working on the project's issues: for fun and interest
as well as for monetary compensation (say, attached to the tickets).

#### License

The repository and its contents are covered by `Apache v2.0`, so anyone can use it without any
concerns.

If you have any changes you'd like to share, don't hesitate to make a pull-request and push them
into the original repository. Definitely no pressure though.

## Privacy policy

It's very important to save user private data and you can be sure: we are working on security of our
applications and improving it every day. No data could be sent somewhere without user notification
and his direct approval. This application is using network connection as minimum as possible to
perform only the operations of its main purpose. All the connections are secured by the wide using
open standards. Any internet connection will not be allowed to collect any user personal data anyway.
