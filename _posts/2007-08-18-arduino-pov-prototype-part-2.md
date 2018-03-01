---
layout: post
status: publish
published: true
title: Arduino POV Prototype - Part 2
author: carlos
date: '2007-08-18 21:15:00 -0400'
date_gmt: '2007-08-19 04:15:00 -0400'
categories:
- My Projects
- Arduino
tags: []
---
I polished up the code for my [Arduino POV display](http://carlitoscontraptions.blogspot.com/2007/08/arduino-pov-prototype.html) and I think it is now ready to be shown to the world!

The source code for the POV display can be downloaded [here](http://carlos.asmat.googlepages.com/POV_0_01.pde).

The parameters in the code can be changed in order to display other images besides of the default arrows.

## Data

The displayed image is stored in the data string. Each drawing is divided in frames (i.e. one frame for each letter of a word) and each frame is divided in columns. The image to be displayed must be encoded into 1s (ON) and 0s (OFF) and each value must be stored in the data string in the order illustrated below.  
  
[![](http://1.bp.blogspot.com/_940DBYqYeYo/RsfbNAGzkOI/AAAAAAAAAXI/ILObPelhFUo/s320/format.png)](http://1.bp.blogspot.com/_940DBYqYeYo/RsfbNAGzkOI/AAAAAAAAAXI/ILObPelhFUo/s1600-h/format.png)

The duration of each column (i.e. how much time they stay ON), the spacing between frames and the spacing between images are set respectively by the integers timer1, timer2 and timer3. Keep in mind that their values depend on the rotation speed.

Finally, the number of frames and their length is set respectively by frame_num and frame_len.

## Arrow (>):

*   timer1: 3
*   timer2: 15
*   timer3: 0
*   data: {1,0,0,0,0,1, 1,1,0,0,1,1, 0,1,1,1,1,0, 0,0,1,1,0,0}
*   frame_len: 4
*   frame_num: 1

[![](http://3.bp.blogspot.com/_940DBYqYeYo/RsfXegGzkKI/AAAAAAAAAWo/2ReHyCoFKhE/s320/arrow.JPG)](http://3.bp.blogspot.com/_940DBYqYeYo/RsfXegGzkKI/AAAAAAAAAWo/2ReHyCoFKhE/s1600-h/arrow.JPG)

## "Alan":

*   timer1: 3
*   timer2: 15
*   timer3: 13
*   data: {1,1,1,1,1,1, 1,0,0,1,0,0, 1,0,0,1,0,0, 1,1,1,1,1,1, 1,1,1,1,1,1, 0,0,0,0,0,1, 0,0,0,0,0,1, 0,0,0,0,0,1, 1,1,1,1,1,1, 1,0,0,1,0,0, 1,0,0,1,0,0, 1,1,1,1,1,1, 1,1,1,1,1,1, 0,1,1,0,0,0, 0,0,0,1,1,0, 1,1,1,1,1,1}
*   frame_len: 4
*   frame_num: 4

[![](http://4.bp.blogspot.com/_940DBYqYeYo/RsfXewGzkLI/AAAAAAAAAWw/kVpsgagELwA/s320/alan.JPG)](http://4.bp.blogspot.com/_940DBYqYeYo/RsfXewGzkLI/AAAAAAAAAWw/kVpsgagELwA/s1600-h/alan.JPG)

## Sinewave (or flower):

*   timer1: 3
*   timer2: 3
*   timer3: 0
*   data: {0,0,1,0,0,0, 0,1,0,0,0,0, 1,0,0,0,0,0, 1,0,0,0,0,0, 0,1,0,0,0,0, 0,0,1,0,0,0, 0,0,0,1,0,0, 0,0,0,0,1,0, 0,0,0,0,0,1, 0,0,0,0,0,1, 0,0,0,0,1,0, 0,0,0,1,0,0}
*   frame_len: 12
*   frame_num: 1

[![](http://1.bp.blogspot.com/_940DBYqYeYo/RsfXfAGzkMI/AAAAAAAAAW4/S8FwL_TlwIk/s320/sine.JPG)](http://1.bp.blogspot.com/_940DBYqYeYo/RsfXfAGzkMI/AAAAAAAAAW4/S8FwL_TlwIk/s1600-h/sine.JPG)

## E = MC²:

*   timer1: 2
*   timer2: 10
*   timer3: 22
*   data: {1,1,1,1,1,1, 1,0,0,1,0,1, 1,0,0,1,0,1, 1,0,0,1,0,1, 1,0,0,1,0,1, 0,0,0,1,0,1, 0,0,0,1,0,1, 0,0,0,1,0,1, 0,0,0,1,0,1, 0,0,0,1,0,1, 1,1,1,1,1,1, 0,1,0,0,0,0, 0,0,1,0,0,0, 0,1,0,0,0,0, 1,1,1,1,1,1, 0,1,1,1,1,0, 1,0,0,0,0,1, 1,0,0,0,0,1, 1,0,0,0,0,1, 0,1,0,0,1,0, 0,1,0,0,1,0, 1,0,0,1,1,0, 1,0,1,0,1,0, 0,1,0,0,1,0, 0,0,0,0,0,0}
*   frame_len: 5
*   frame_num: 5

[![](http://3.bp.blogspot.com/_940DBYqYeYo/RsfXfgGzkNI/AAAAAAAAAXA/irwYC4rg1pY/s320/e_mc2.JPG)](http://3.bp.blogspot.com/_940DBYqYeYo/RsfXfgGzkNI/AAAAAAAAAXA/irwYC4rg1pY/s1600-h/e_mc2.JPG)