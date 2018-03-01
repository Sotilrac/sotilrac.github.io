---
layout: post
status: publish
published: true
title: Inverted Pendulum
author: carlos
carloswordpress_id: 55
wordpress_url: http://carlitoscontraptions.com/?p=55
date: '2008-06-20 07:32:00 -0400'
date_gmt: '2008-06-20 14:32:00 -0400'
categories:
- My Projects
tags:
- Software
- Robot
---
[![](http://3.bp.blogspot.com/_940DBYqYeYo/SDPGFvyrO7I/AAAAAAAAAt4/1NkTj6x2sg0/s320/cart.png)](http://3.bp.blogspot.com/_940DBYqYeYo/SDPGFvyrO7I/AAAAAAAAAt4/1NkTj6x2sg0/s1600-h/cart.png)

My friend David and I implemented an inverted pendulum controller for the [Quanser cart](http://www.quanser.com/english/html/products/fs_product_challenge.asp?lang_code=english&pcat_code=exp-lin&prod_code=L2-invpen&tmpl=1) in th Control and Robotics Lab. The controller was implemented using Simulink and Matlab, which makes the tasks much simpler than dealing with microcontrollers and C.

We implemented many kinds of controllers, but the best turned out to be the full state feedback controller where we get to control the position and velocity of both the cart and the rod. The controller block diagram is shown below.

[![](http://1.bp.blogspot.com/_940DBYqYeYo/SGVk4OB5jaI/AAAAAAAAAv0/akVFNl3N_Tg/s320/Full+State+Feedback+Diagram.png)](http://1.bp.blogspot.com/_940DBYqYeYo/SGVk4OB5jaI/AAAAAAAAAv0/akVFNl3N_Tg/s1600-h/Full+State+Feedback+Diagram.png)  

Below you can find the slides for a presentation giving a quick overview of this subject and a video demonstration featuring David as the presenter.

[slideshare https://www.slideshare.net/Carlito/inverted-pendulum]
