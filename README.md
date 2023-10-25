<p align="center">
Fork of the Polybar project - a fast and easy-to-use tool for creating status bars.
</p>

**Multibar** is a fork of an existing project named Polybar and aims to help users build beautiful and highly customizable status bars
for their desktop environment, without the need of having a black belt in shell scripting.

I created this fork primarily for my personal usage as I have several improvements over the "vanilla" version and I wanted to make this maintainable.
I have changed the name since I want both this and Polybar to be installed simultaneously on my system and "_polybar2_" seemed too lame...

![default configuration screenshot](doc/_static/default.png)

My intention is to keep as much compatibility with Polybar and point out things that are different. You can use Polybar Wiki for most of the things here.

## Table of Contents

* [Introduction](#introduction)
* [Getting started](#getting-started)
  * [Installation](#installation)
  * [First Steps](#first-steps)
* [License](#license)
* [Signatures](#signatures)

## Introduction

The main purpose of **Multibar** is to help users create awesome status bars.
It has built-in functionality to display information about the most commonly used services.
Some of the services included so far:

- Systray icons
- Window title
- Playback controls and status display for [MPD](https://www.musicpd.org/) using [libmpdclient](https://www.musicpd.org/libs/libmpdclient/)
- [ALSA](https://www.alsa-project.org/main/index.php/Main_Page) and [PulseAudio](https://www.freedesktop.org/wiki/Software/PulseAudio/) volume controls
- Workspace and desktop panel for [bspwm](https://github.com/baskerville/bspwm) and [i3](https://github.com/i3/i3)
- Workspace module for [EWMH compliant](https://specifications.freedesktop.org/wm-spec/wm-spec-1.3.html#idm140130320786080) window managers
- Keyboard layout and indicator status
- CPU and memory load indicator
- Battery display
- Network connection details
- Backlight level
- Date and time label
- Time-based shell script execution
- Command output tailing
- User-defined menu tree
- Inter-process messaging
- And more...

[See the Polybar wiki for more details](https://github.com/polybar/polybar/wiki).

## Getting started

### Installation
If you are using **Gentoo**, you can use [my overlay](https://github.com/xoores/gentoo-overlay) that will have necessary ebuilds.

Otherwise, you will have to [build from source](https://github.com/polybar/polybar/wiki/Compiling).

### First Steps
[See the Polybar wiki for details on how to run and configure polybar](https://github.com/polybar/polybar/wiki).

## License

Polybar is licensed under the MIT license. [See LICENSE for more information](https://github.com/xoores/multibar/blob/master/LICENSE).

## Signatures

Release archives and tags are signed by a maintainer using GPG. Everything is signed by my GPG key.