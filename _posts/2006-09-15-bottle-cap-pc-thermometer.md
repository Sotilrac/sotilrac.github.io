---
layout: post
status: publish
published: true
title: Bottle Cap PC Thermometer
author: carlos
date: '2006-09-15 12:32:00 -0400'
date_gmt: '2006-09-15 19:32:00 -0400'
categories:
- My Projects
tags: []
---
Based on a circuit I found in [this website](http://web.archive.org/web/20040215182109/http://www.electronics-lab.com/projects/pc/013/index.html "Wayback Machine Link"),  
I built a very simple thermometer. The major thing I added to the original design is a nice case.

## Materials:

*   1 Diode
*   1 Thermistor
*   1 Capacitor
*   1 Serial cable (or plug)
*   2 Plastic bottle caps (one slightly bigger than the other)

## The Circuit

\[caption id="attachment_704" align="aligncenter" width="266" caption="Digital Thermometer Circuit Schematics"\][![Digital Thermometer Circuit Schematics](http://carlitoscontraptions.com/wp-content/uploads/2006/09/shema.jpg "Digital Thermometer Circuit Schematics")](http://carlitoscontraptions.com/wp-content/uploads/2006/09/shema.jpg)\[/caption\]

I salvaged all the parts from old electronics (found in garbage) so they were free. All the parts are very easy to find except for the thermistor. I did not get precisely a thermistor but a very close approximation to it. In fact, I'm not very sure of what it is that I used.

I just soldered the components together, no need of PCB.  
[![](http://carlitoscontraptions.com/wp-content/uploads/blogger/blogger/4122/3639/200/thermometer%20circuit.jpg)](http://carlitoscontraptions.com/wp-content/uploads/blogger/blogger/4122/3639/1600/thermometer%20circuit.jpg)

## My Thermistor

I got the thermistor form a broken drinking water dispenser /cooler.

The relationship between the temperature and resistance in an usual thermistor is mostly linear. For my thermistor, the lower bound for the linear region of the resistance-temperature relation is 11Â°C. Below this point, its resistance goes to infinity (is doesn't allow any current to pass). I suppose this is used to stop cooling the water when it gets at the desired 11Â°C temperature. I haven't yet found an upper bound for the liner region.

[![](http://carlitoscontraptions.com/wp-content/uploads/blogger/blogger/4122/3639/200/thermometer%20extended.jpg)](http://carlitoscontraptions.com/wp-content/uploads/blogger/blogger/4122/3639/1600/thermometer%20extended.jpg)Anyways, the only problem is that it can't measure temperatures below 11Â°C.

## The Case

To build a nice looking case, I simply used two plastic bottle cap (from a Propel and Powerade bottles) that my girlfriend brought me from the recycling bin at her job (a gym).

[![](http://photos1.blogger.com/blogger/4122/3639/320/thermometer.2.jpg)](http://photos1.blogger.com/blogger/4122/3639/1600/thermometer.2.jpg)These two caps happen to fit perfectly one inside the other. So I simply cut a hole for the cable and drilled another for the probe (MT). I placed the circuit (properly insulated with tape, of course) inside, closed it and the thermometer was done.  
[![](http://photos1.blogger.com/blogger/4122/3639/200/thermometer%20inside.jpg)](http://photos1.blogger.com/blogger/4122/3639/1600/thermometer%20inside.jpg)

## The Software

In order to run use the thermometer you need a small program. I used the original [digital thermometer program](http://carlitoscontraptions.com/wp-content/uploads/2006/09/tempmeter.zip) but it wouldn't be hard to right a new one or to improve the existing one.

[![](http://photos1.blogger.com/blogger/4122/3639/200/thermometer%20full.jpg)](http://photos1.blogger.com/blogger/4122/3639/1600/thermometer%20full.jpg)