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
      [Milestones](https://github.com/state-of-the-art/Handy3DScanner/milestones)
      [Issues](https://github.com/state-of-the-art/Handy3DScanner/issues)
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

It's a general-purpose portable 3D scanner complex.

## Requirements

* Host:
  * **Smartphone** - anything with Android 4.0.1+ and usb3 host is ok (*later usb2 will be supported*)
  * **Linux workstation** - Ubuntu LTS, Debian, CentOS...
* **Intel Realsense D400** - stereo camera with D4 board (right now tested D415, but D435 also should be ok)
* **USB-C/USB-C cable** - USB3.1 Gen 1 should work properly (*seems could also work on usb2 + 5V1A cable*)
* **Handy 3D Scanner** - application piece, published in Android store and available for workstations.

## Price

* Professional 3d scanners: ~$10'000-$20'000.
* Table laser scanners: ~$70-$500.

With Intel Realsense D415 (~$140) and mobile app we can get a simple and cheap solution to provide a really
cheap mid-range HD solution with advanced specifications:
* Resolution: 1Mpix (1280x720)
* Frame-rate: 30-60 fps
* Angle: 63°x40°, 85°x58°
* Range: .16-10m, .11-10m

Means that finally for ~$200 users can get simple solution to build second instagram, now in 3D - and the
last piece is just a userspace software.

## Application

Basically have just 3 main functions:
* **Capture** - allow to get shots and records of the environment
  * Single shot mode -
    Just getting shot of the current view and converting it to pointcloud (`pc`)
  * Record mode (*in dev*) -
    Useful for experimenting with AI, but consumes alot of memory
  * Walk-around mode (*in dev*) -
    to capture relatively small objects and humans just walking around and taking pictures
  * Panorama mode (*uses phone `gyro` to get panorama*) -
    allow to capture panoramas & huge environments around the camera
* **View/Edit** - shows what `pc` you have and allow to edit them
  * List of the captured `pc`
  * Show/Hide `pc` from the list
  * Camera controls: rotation, zoom, focus to point
  * Selection of `pc` points: single, line, box
  * Hide points: selected or unselected
  * Delete points: selected or unselected
* **Load/Save** - when we would like to view or store `pc` or mesh (*in dev*)

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
* Save captured pc in PCD format (to internal app dir)
* Simple pc edit tools
* Gyro-based panoramic shots (need improvement)

### TODO

Here is a list of usecases/features that will be good to see soon:

* Save & load pc to user folder
* Autogenerate triangle surface for `pc`
* Save triangle surface as mesh file (obj)
* Implement walk-around-object mode
* Improve panorama mode
* ROS bag stream capture support
* Compress pcd/obj files
* Create advanced selection tools:
  * Select near points by height
  * Select nearest object to strip background
  * Free selection
* Implement settings to adjust parameters
* Implement automatic/manual align of `pc` using `PCL` algorythms
* Animation of the pointclouds (live avatars)

### OpenSource

We have plans to publish full source code on github to make sure application will live for a long time.

This is an exprerimental project - main goal is to test State Of The Art philosophy on practice.

So for now we starting with closed source & Android PlayStore, but when there will
be something to show - source code will be opened and we will start to actually search developers
in opensource community to help with implementation some non-standard logic with `pc` procesing.

## Privacy policy

It's very important to save user private data and you can be sure: we working on security
of our applications and improving it every day. No data could be sent somewhere without
user notification and his direct approve. This application will work standalone without
any internet connection and will not collect any user personal data anyway.
