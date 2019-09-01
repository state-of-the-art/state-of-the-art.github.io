---
title: Handy 3D Scanner
excerpt: General purpose 3d scaner based on Intel Realsense D400 cameras
header:
  image: /assets/images/projects/handy3dscanner/header.jpg
  teaser: /assets/images/projects/handy3dscanner/teaser.png
sidebar:
  - image: /assets/images/projects/handy3dscanner/teaser.png
    image_alt: icon
  - title: Links
    text: |
      [GitHub](https://github.com/state-of-the-art/Handy3DScanner)
      [PlayStore](https://play.google.com/store/apps/details?id=io.stateoftheart.handy3dscanner)
  - title: Stack
    text: C++, Qt 5.12, librealsense 2
  - title: Platforms
    text: Linux, Android
  - title: UI
    text: Qt QML + js, OpenGL ES 3
  - title: Hardware
    text: Intel Realsense D415, D435
gallery:
  - url: /assets/images/projects/handy3dscanner/screenshot-01.jpg
    image_path: /assets/images/projects/handy3dscanner/screenshot-01.jpg
    alt: "Capture fireplace"
  - url: /assets/images/projects/handy3dscanner/screenshot-02.jpg
    image_path: /assets/images/projects/handy3dscanner/screenshot-02.jpg
    alt: "Edit fireplace"
  - url: /assets/images/projects/handy3dscanner/screenshot-03.jpg
    image_path: /assets/images/projects/handy3dscanner/screenshot-03.jpg
    alt: "Edit fireplace close look"
  - url: /assets/images/projects/handy3dscanner/screenshot-04.jpg
    image_path: /assets/images/projects/handy3dscanner/screenshot-04.jpg
    alt: "Capture table mess"
  - url: /assets/images/projects/handy3dscanner/screenshot-05.jpg
    image_path: /assets/images/projects/handy3dscanner/screenshot-05.jpg
    alt: "Edit table mess"
  - url: /assets/images/projects/handy3dscanner/screenshot-06.jpg
    image_path: /assets/images/projects/handy3dscanner/screenshot-06.jpg
    alt: "Edit table mess close look"
---

{% include gallery caption="Couple of screenshots from Samsung S8" %}

## Description

Opensource general-purpose portable 3D scanner application.

## Requirements

* Host:
  * **Smartphone / Tablet** - anything with Android 5+ (Lollipop or better) and usb2/3 host is ok
  * **Linux workstation** - Ubuntu LTS, Debian, CentOS...
* **Intel Realsense D400** - stereo camera with D4 board (tested D415 and D435i)
* **USB-C/USB-C cable** - USB3.1 Gen 1 and USB2 will work properly
* **Handy 3D Scanner** - application piece, published in Android store and available for workstations.

## Price

* Professional 3d scanners: ~$10'000-$20'000.
* Table laser scanners: ~$70-$500.

With Intel Realsense D415 (~$140) and mobile app you can get a simple solution with the next parameters:
* Resolution: 1Mpix (1280x720)
* Frame-rate: 30-60 fps
* Angle: 63°x40°, 85°x58°
* Range: .16-10m, .11-10m

## Application

### Overview

Basically have just 3 main functions:
* **Capture** - allow to get shots and records of the environment
  * General mode -
    you can take pointclouds capturing your surrounding with a proper positioning of the
    shots (gyroscope or arcore positioning).
  * Record mode (*in dev*) -
    Useful for experimenting with AI, but consumes alot of memory
* **View/Edit** - shows what `pc` you have and allow to edit them
  * List of the captured `pc`
  * Show/Hide `pc` from the list
  * Camera controls: rotation, zoom, focus to point
  * Selection of `pc` points: single, line, box
  * Hide points: selected or unselected
  * Delete points: selected or unselected
* **Load/Save** - when we would like to view or store `pc` or mesh
* **Export** - save the whole 3d scene as glTF 2.0 glb file to import it in 3d edit software or share

Also there will be settings, skeletal animation and other stuff.

### Applications

* VR/AR avatars,  objects - scan yourself, your cat or entire house and bring them to VR/AR.
* General purpose portable 3d scanner for 3d printer - if you want to build a copy of object you like.
* Modelling - sometimes it's much easier to scan and edit in 3d editor (Blender / 3DSMax).
* Measuring - it's pretty accurate, so you can use it to measure stuff or proportions.
* 3d Instagram - hopefully we will get to this state :)
* Who knows - when such techs are going wild, it's hard to predict how they will be used.

### Features

* Easy capture from Intel Realsense D415/D435
* Full available camera resolution (D415 1280x720 points)
* Preview of the captured point clouds (pc)
* Save captured pc in PCD format and export scene to glTF 2
* Simple pc edit tools
* Gyro-based panoramic shots

### Plans

You can see all the feature requests/bugs on the github page:

* [Milestones](https://github.com/state-of-the-art/Handy3DScanner/milestones)
* [Issues](https://github.com/state-of-the-art/Handy3DScanner/issues)

But overall we have a huge plans to make this application better!
* **Prepare version 1.0** - it should be useful for everyday use.
* **Kickstarter campagin** - customers want to see the complete product - so why not?
* **Publish source code** - necessary to make sure the project will live it's long life.
* **Reach the top** - the market could be bigger, any smartphone should get this feature
  because AR/VR is coming. So Handy 3D Scanner can help with building the new future where
  everyone will take not just photo, but capture part of the 3d world and place it in VR.

### OpenSource

This is an experimental project - main goal is to test State Of The Art philosophy on practice.

We would like to see a number of independent developers working on the same project issues
for the real money (attached to the ticket) or just for fun. So let's see how this will work.

#### License

Repository and it's content is covered by `Apache v2.0` - so anyone can use it without any concerns.

If you will have some time - it will be great to see your changes merged to the original repository -
but it's your choise, no pressure.

#### Build

You can find application sources in the [GitHub](https://github.com/state-of-the-art/Handy3DScanner/)
repository and build your own binaries for workstation/android devices following the README.md
build steps.

## Privacy policy

It's very important to save user private data and you can be sure: we working on security
of our applications and improving it every day. No data could be sent somewhere without
user notification and his direct approve. This application will work standalone without
any internet connection and will not collect any user personal data anyway.
