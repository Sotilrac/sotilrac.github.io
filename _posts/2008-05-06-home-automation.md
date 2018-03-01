---
layout: post
status: publish
published: true
title: Home Automation
author: carlos
date: '2008-05-06 22:17:00 -0400'
date_gmt: '2008-05-07 05:17:00 -0400'
categories:
- My Projects
tags: []
---
Here is some information about a home automation system my team and I did some time ago. This was done for the Embedded Systems class and require two [Altera UP1](http://www.altera.com/literature/univ/univ.pdf) FPGA boards, two computers and two [USB-to-TTL](http://www.ftdichip.com/Products/EvaluationKits/TTL-232R.htm) wires.

[![](http://1.bp.blogspot.com/_940DBYqYeYo/SCFr24JSHAI/AAAAAAAAArA/s_al6j1dMH0/s320/system+diagram.png)](http://1.bp.blogspot.com/_940DBYqYeYo/SCFr24JSHAI/AAAAAAAAArA/s_al6j1dMH0/s1600-h/system+diagram.png)
- The nice picture above was done by Frank (see below) -

Although at the beginning of the project we were really motivated to do a robust and optimal design that could set an example on how to do home automation and that could be shared with everybody, the project quickly degenerated and the general design approach became: "We don't care of how inelegant, inefficient or completely surrealist the system is as long as it works". The main reason for this radical change was the implacable deadline that got closer and closer, and the usual lack of time Electrical Engineering students suffer from.

The system consists of a PC that takes high level decisions for the control of lighting, heating and power consumption in general for a house. This decisions are serially sent to an FPGA board that take some lower level decisions (such as debouncing switches, counting time, etc) and controls trough a very large number of IO pins (~90) the actual house hardware.

[![](http://3.bp.blogspot.com/_940DBYqYeYo/SCFr3YJSHCI/AAAAAAAAArQ/YL2kiGDffrc/s320/system.png)](http://3.bp.blogspot.com/_940DBYqYeYo/SCFr3YJSHCI/AAAAAAAAArQ/YL2kiGDffrc/s1600-h/system.png)

Since this is a small project, we do not have the actual house or its hardware, so we resorted to simulate it using a second FPGA board and another computer. The second computer controls the house status (temperature in each room, level of room light, motion in the rooms, status of the TV, etc) and offers an inteface so the user can turn on lights, move in a room, set the desired room temperature, turn on the microwave oven, etc. All this information is serially sent to the second FPGA board which then adjusts its pins status to mimic the house hardware.

[![](http://2.bp.blogspot.com/_940DBYqYeYo/SCFr3IJSHBI/AAAAAAAAArI/MIF_vx2AeAY/s320/simulator.png)](http://2.bp.blogspot.com/_940DBYqYeYo/SCFr3IJSHBI/AAAAAAAAArI/MIF_vx2AeAY/s1600-h/simulator.png)
-The GUI and the Java program were done by Yev and Ritvik -

All the coding was done in Java and VHDL and since it is not very well organized or useful to anybody else, I won't be posting it. Nevertheless, the documents describing this project are very nicely done (all modesty aside) and give a clear description of what we did. Here you have: the [SRS](http://carlitoscontraptions.com/wp-content/uploads/2009/04/srs.pdf), the [SDD](http://carlitoscontraptions.com/wp-content/uploads/2009/04/sdd.pdf), and the [STC](http://carlitoscontraptions.com/wp-content/uploads/2009/04/stc.pdf) (not the final version). Please keep in mind that this documents are not published under the CC license, they have full copyright.

[![](http://1.bp.blogspot.com/_940DBYqYeYo/SCFsm4JSHFI/AAAAAAAAAro/etV81uE8WuE/s320/ss851269.jpg)](http://1.bp.blogspot.com/_940DBYqYeYo/SCFsm4JSHFI/AAAAAAAAAro/etV81uE8WuE/s1600-h/ss851269.jpg)

Above you can see my friend Frank, he's the leader of the group (transformed from the norm by the nuclear goop).

Just so you know, the project went well and allowed us to learn a lot. We even ended up having a very good mark, so everybody should be (and is) happy.

If you are wondering what did I do in the project (I'm sure you are): I did the serial communication protocol in Java.