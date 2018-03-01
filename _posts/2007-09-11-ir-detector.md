---
layout: post
status: publish
published: true
title: IR Detector
author: carlos
date: '2007-09-11 15:18:00 -0400'
date_gmt: '2007-09-11 22:18:00 -0400'
categories:
- My Projects
tags: []
---
Besides [my POV display](http://carlitoscontraptions.blogspot.com/2007/08/pov-prototype-part-2.html), I'm trying to do a robot that detects obstacles using IR light. In order to make it easy to work with IR light, [infertility](http://cialis24online.net/) I built a very simple IR detector based on [this article](http://www.thekeeser.com/Projects/simple_ir_detector.htm).

## General Idea

An IR signal is "seen" by a reverse biased IR diode which produces an electrical signal according to the light intensity. This signal is then amplified trough a transistor which powers an ordinary LED. This means that the LED will light up when the IR diodes receives some IR light (from a TV remote for instance).

[![](http://4.bp.blogspot.com/_940DBYqYeYo/RuloSbsPf0I/AAAAAAAAAag/pgRrG1gyMoA/s320/dcp_0019.jpg)](http://4.bp.blogspot.com/_940DBYqYeYo/RuloSbsPf0I/AAAAAAAAAag/pgRrG1gyMoA/s1600-h/dcp_0019.jpg)

## Materials

*   An IR Diode (I got mine from an old TV set)
*   An LED (a [yellow one](http://alan-parekh.vstore.ca/product_info.php/cPath/4_6/products_id/18) in my case)
*   A 1k Ohms resistor
*   A 50 Ohms resistor (two 100 Ohms resistors in parallel)
*   A BJT (I used the 2N3904, but any common BJT should work with the right biasing)
*   An old 9V battery (for the casing)
*   A new 9V battery (for power)

[![](http://1.bp.blogspot.com/_940DBYqYeYo/RuloRrsPfxI/AAAAAAAAAaI/OzzYmlfYPgY/s320/dcp_0002.jpg)](http://1.bp.blogspot.com/_940DBYqYeYo/RuloRrsPfxI/AAAAAAAAAaI/OzzYmlfYPgY/s1600-h/dcp_0002.jpg)

## The Circuit

[![](http://3.bp.blogspot.com/_940DBYqYeYo/RuoRY7sPf2I/AAAAAAAAAaw/j5YrhE8ALsQ/s320/IRD_circuit.png)](http://3.bp.blogspot.com/_940DBYqYeYo/RuoRY7sPf2I/AAAAAAAAAaw/j5YrhE8ALsQ/s1600-h/IRD_circuit.png)

## Construction Notes

I built the circuit by soldering the components together without using a PCB and enclosed it in an old 9V battery.

I used a battery as the casing because it is free, it looks cool, and it includes a battery clip.

The battery's cap is actually a battery clip that can be soldered to the circuit in order to connect it to another 9V battery.

When using a battery as a case, keep in mind that:

*   the inside of the battery should be insulated (with blue masking take in my case)
*   it is a good idea keep one or two of the AAAA batteries (that can be found inside the 9V battery) and use them to keep the top and bottom caps in place (make sure they are insulated two).