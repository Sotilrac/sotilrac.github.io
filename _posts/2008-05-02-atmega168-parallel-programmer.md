---
layout: post
status: publish
published: true
title: ATmega168 Parallel Programmer
author: carlos
carloswordpress_id: 50
wordpress_url: http://carlitoscontraptions.com/?p=50
date: '2008-05-02 00:26:00 -0400'
date_gmt: '2008-05-02 07:26:00 -0400'
categories:
- My Projects
tags: []
---
[![](http://2.bp.blogspot.com/_940DBYqYeYo/SB4hg4JSG6I/AAAAAAAAAp4/zM-0biU-OgE/s320/ss851490.jpg)](http://2.bp.blogspot.com/_940DBYqYeYo/SB4hg4JSG6I/AAAAAAAAAp4/zM-0biU-OgE/s1600-h/ss851490.jpg)

I own a few Rev. C [Bare Bones Boards](http://moderndevice.com/) witch came with ATmega168 chips burned with the old Arduino bootloader (NG). I wanted to upgrade them to the newer (Diecimilia) bootloader so I built a parallel programmer following the instructions in the [Arduino website](http://www.arduino.cc/en/Hacking/ParallelProgrammer) and using parts I found in the garbage (as usual).

## Materials

*   Two 470 Ohms resistors
*   One 220 Ohms resistor
*   Some wire
*   A female header at least 3x2
*   A ferrite core (not required but looks cool)
*   Some heat shrink (it could be replaced by some electrical tape)
*   A male parallel port connector (DB-25)

## Programmer Schematics

(this is a [vectorized version](http://carlitoscontraptions.com/wp-content/uploads/2009/04/parallelprogrammer.svg "Parallel Programmer") of the original schematics on the Arduino site)

[![](http://3.bp.blogspot.com/_940DBYqYeYo/SB4jUIJSG-I/AAAAAAAAAqY/uQgGrthC_aA/s320/schematics.png)](http://3.bp.blogspot.com/_940DBYqYeYo/SB4jUIJSG-I/AAAAAAAAAqY/uQgGrthC_aA/s1600-h/schematics.png)

## Construction

I got a DB-25 connector from an extension parallel port of a PC I found in the garbage. First, I removed the original cable that came with it and I soldered the programmer's resistors to the back of the DB-25 and connected them to new wires. Then, I covered the resistors and cable connections with a piece of heat shrink tubing.

[![](http://2.bp.blogspot.com/_940DBYqYeYo/SB4hh4JSG9I/AAAAAAAAAqQ/hgKSHsB-Omo/s320/ss851498.jpg)](http://2.bp.blogspot.com/_940DBYqYeYo/SB4hh4JSG9I/AAAAAAAAAqQ/hgKSHsB-Omo/s1600-h/ss851498.jpg)

The new wires where terminated in a 4x2 female header (even though there are only 5 wires). The wires and female headers come from an old computer (they connected the power buttons and the case LEDs to the motherboard). I cut the header to size from a larger header (form the same old computer) and I used an extra row to mark it with a white pin cap so I could easily remember where the #1 pin is located.

[![](http://2.bp.blogspot.com/_940DBYqYeYo/SB6Ej4JSG_I/AAAAAAAAAqg/wHEluYVtKxY/s320/ss851496-mod.jpg)](http://2.bp.blogspot.com/_940DBYqYeYo/SB6Ej4JSG_I/AAAAAAAAAqg/wHEluYVtKxY/s1600-h/ss851496-mod.jpg)

Finally, I added a ferrite core and twisted the cables in order to reduce noise and cross-talk. I don't think this is really required but it looks nice.

[![](http://4.bp.blogspot.com/_940DBYqYeYo/SB4hhYJSG7I/AAAAAAAAAqA/ifDJ_Qd3d1o/s320/ss851494.jpg)](http://4.bp.blogspot.com/_940DBYqYeYo/SB4hhYJSG7I/AAAAAAAAAqA/ifDJ_Qd3d1o/s1600-h/ss851494.jpg)