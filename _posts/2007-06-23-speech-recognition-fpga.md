---
layout: post
status: publish
title: Speech Recognition Using on FPGA
author: carlos
date: '2007-06-23 15:28:00 -0400'
date_gmt: '2007-06-23 22:28:00 -0400'
categories:
- My Projects
- FPGA
tags: []
---
My friends David and Kanwen, and I implemented a speech recognition system on an FPGA development board (Altera DE2 Board) for the Design Project course at McGill (ECSE 494). We did this in two step: first we wrote a prototype for the algorithm in MATLAB (I'll maybe port it to Octave), and then we did the hardware description for the FPGA.

## MATLAB Prototype

[![](http://1.bp.blogspot.com/_940DBYqYeYo/Rn2fZAO16II/AAAAAAAAAS4/VPEe0O68dJY/s320/blackboard.jpg)](http://1.bp.blogspot.com/_940DBYqYeYo/Rn2fZAO16II/AAAAAAAAAS4/VPEe0O68dJY/s1600-h/blackboard.jpg)

Inspired by the algorithm described in [a site from the University of Toronto](http://www.eecg.toronto.edu/%7Eaamodt/ece341/speech-recognition/), we wrote two MATLAB scripts: [train.m](http://carlos.asmat.googlepages.com/train.m) and [recogniz.m](http://carlos.asmat.googlepages.com/recogniz.m).

train.m deals with the training phase, in which many versions of a sound (a spoken word for instance) are input and averaged in the frequency domain thus generating the sound's reference fingerprint.

recogniz.m deals with the recognition phase, where a sound is input, translated to the frequency domain (i.e. Its fingerprint is generated), and compared to the reference fingerprint by computing the euclidean distance between them (as if both fingerprints where vectors).

Both scripts need to detect the beginning of the sound (i.e tell when the spoken word begins). They do so by averaging two adjacent 1024-sound-samples groups (in the time domains) and computing the difference between the averages. So, if there is a sudden increase in the sound's amplitude, the difference will be significant and the sound is assumed to start after that sudden increase. The sound's length is fixed to 1,024 s (see the picture below for more details)

Note that the scripts use 16-bit WAV files as input @ 22050 Hz (this is the default windows sound recorder output, since I could not do it in Linux because the mic did not wanted to work). The sound input is downsampled and quantized in order to get it down to 8 bit /sample @ 5 kHz for processing.

Also you might encounter problems if the sound file is too short (it should last for more than 1,1 s), or if its volume level is too low (this happens because the detector threshold is fixed).

## Hardware Implementation

[![](http://1.bp.blogspot.com/_940DBYqYeYo/Rn2fZAO16JI/AAAAAAAAATA/XpG9KYlUIa8/s320/system.jpg)](http://1.bp.blogspot.com/_940DBYqYeYo/Rn2fZAO16JI/AAAAAAAAATA/XpG9KYlUIa8/s1600-h/system.jpg)

Once we had played enough with the MATLAB prototype parameters, we mapped the algorithm into combinational logic and finite state machines (FSM) by breaking it down into independent modules.

For more details about the hardware implementation and the project in general you can read the [full project report](http://carlos.asmat.googlepages.com/SpeechRecognitionUsingFPGATechnology.pdf). You may also want to see the slides for a presentation we did (below).

Unfortunately, I cannot post the project files (i.e. VHDL code).

[![](http://4.bp.blogspot.com/_940DBYqYeYo/Rn2fYwO16HI/AAAAAAAAASw/z7rsB-flDPY/s320/DE2+board.jpg)](http://4.bp.blogspot.com/_940DBYqYeYo/Rn2fYwO16HI/AAAAAAAAASw/z7rsB-flDPY/s1600-h/DE2+board.jpg)

Note that all the documentation for this project was done using the very excellent [OpenOffice.org](http://openoffice.org/).