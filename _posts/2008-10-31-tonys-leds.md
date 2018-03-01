---
layout: post
status: publish
published: true
title: Tony's LEDs
author: carlos
carloswordpress_id: 62
wordpress_url: http://carlitoscontraptions.com/?p=62
date: '2008-10-31 12:40:00 -0400'
date_gmt: '2008-10-31 19:40:00 -0400'
categories:
- My Projects
tags:
- Electronics
---
I received many questions about the circuits driving the LEDs in many of my projects, especially for the Iron Man's repulsor.

LEDs are pretty neat devices. You make some current flow forward through it and you get some light as a result. Nevertheless, since they are diodes, they can allow an infinite amount of current to flow (which in practice means a lot of current) and this can be problematic since, as any electrical device, it cannot handle that much current. In order to prevent them to pass too much current, a current limiting circuit is required (usually implemented as a resistor in series).

When you buy an LED, you (should) get two very important parameters, the voltage drop across them (say, V\_LED), and the maximum continuous current (I\_LED).

So, for the trivial case where we have a battery (V_bat) in series with a resistor (R) and an LED, the value of R must obey the following inequation:

[![](http://1.bp.blogspot.com/_940DBYqYeYo/SQtqJBSrh1I/AAAAAAAAA3o/j1sBKstmoKo/s320-R/eq1.png)](http://1.bp.blogspot.com/_940DBYqYeYo/SQtqJBSrh1I/AAAAAAAAA3o/ExdAkldX0OU/s1600-h/eq1.png)

If you decide to place many (say, n) LEDs in series, the inequation becomes:

[![](http://2.bp.blogspot.com/_940DBYqYeYo/SQtqKOiUzjI/AAAAAAAAA3w/W7Sx_sD0KO8/s320-R/eq2.png)](http://2.bp.blogspot.com/_940DBYqYeYo/SQtqKOiUzjI/AAAAAAAAA3w/l6gU6lG5wNo/s1600-h/eq2.png)

Finally, if the LEDs are in parallel (as is the case for the repulsor), the inequation becomes:

[![](http://4.bp.blogspot.com/_940DBYqYeYo/SQtqLbqdonI/AAAAAAAAA34/cgeDhMSOq_w/s320-R/eq3.png)](http://4.bp.blogspot.com/_940DBYqYeYo/SQtqLbqdonI/AAAAAAAAA34/EzzOtWjwzBA/s1600-h/eq3.png)

This result can be obtained by applying Ohm's law (V= RI) to the circuits described above. The proof is of course let as an exercise for the reader ;) .  
This page has a very nice LED calculator which makes life really easy when calculating resistor values: [alan-parekh.com/led\_resistor\_calculator.html](http://alan-parekh.com/led_resistor_calculator.html)

**WARNING**: the repulsor circuit may cause the LEDs to fail sooner or later. I'll post an update as soon as I have one. Thanks to [Tim](http://kd7jz.blogspot.com/) for the hint.

For those interested in the repulsor circuit, below you can find a diagram describing it. It is the same as the circuit with many LEDs in parallel but with a potentiometer added to regulate the light intensity. The only requisite for the potentiometer is to be large enough to attain the dimmest light according to your needs.

[![](http://3.bp.blogspot.com/_940DBYqYeYo/SQtfucqU7bI/AAAAAAAAA3g/2jt7B0roQ2c/s320-R/circuit.png)](http://3.bp.blogspot.com/_940DBYqYeYo/SQtfucqU7bI/AAAAAAAAA3g/gA_3WEfIZps/s1600-h/circuit.png)