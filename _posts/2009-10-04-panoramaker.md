---
layout: post
status: publish
published: true
title: Panoramaker
author: carlos
carloswordpress_id: 348
wordpress_url: http://carlitoscontraptions.com/?p=348
date: '2009-10-04 21:55:03 -0400'
date_gmt: '2009-10-05 01:55:03 -0400'
categories:
- My Projects
- Software
- Robotics
tags:
- Software
- Photography
---
As [promised before](http://carlitoscontraptions.com/2009/09/panoramic-camera-prototype/ "Panoramic Camera Prototype"), here is the Python script that runs my [panoramic camera hardware](http://carlitoscontraptions.com/2009/09/panoramic-camera-prototype/ "Panoramic Camera Prototype"). It is a very quick prototype and is by no means intended for widespread use since it requires manual calibration. Nevertheless, it might be very useful to those seeking to learn how to position the servos or control a digital camera through Python.

This script requires my [Pololu library](http://carlitoscontraptions.com/2009/07/pololu-python-library/ "Pololu Library") and includes some codes from [here](https://vmlaker.org/geek/python/digital-camera-control-with-gphoto2 "Digital Camera Control with gphoto2 ") in order to control the camera. Besides the basic requirements of lib_pololu, the script also requires [gPhoto](http://gphoto.sourceforge.net/ "gPhoto"). If you are running Linux, you most likely already have it but in case you do not, you can install it through your favourite package manager or by using the console (e.g. for Ubuntu/Debian):

{% highlight bash %}
sudo apt-get install gphoto
{% endhighlight %}

If you are using some other OS, you can download gPhoto from [here](http://sourceforge.net/projects/gphoto/files/ "Download gPhoto").

## The Code

\[gist id=3746452\]

Again, many thanks to [RobotShop](http://www.robotshop.com/ "RobotShop") who provided the hardware that made this project possible.