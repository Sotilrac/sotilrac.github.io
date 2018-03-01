---
layout: post
status: publish
published: true
title: Solitudes
author: carlos
carloswordpress_id: 69
date: '2009-02-18 16:35:00 -0500'
date_gmt: '2009-02-18 23:35:00 -0500'
categories:
- Info
tags:
- Trash
---
In many drugstores and bookstores here in Montreal (AFAIK), we find the [Solitudes](http://www.solitudes.com/) CDs. These are CDs containing music mainly based on nature sounds (elevator music really). The interesting thing about this CDs is that they are displayed on a shelf with an interactive player that the customer can use to get a glimpse of the content of the CDs being offered. In other words, the customer touches on a CD icon, and the shelf starts to play (what seems to be) the contents of that CD.

[![](http://4.bp.blogspot.com/_940DBYqYeYo/SZyYBT9AoGI/AAAAAAAABZQ/6EYfBQ6xyLA/s320/img_1538.jpg)](http://4.bp.blogspot.com/_940DBYqYeYo/SZyYBT9AoGI/AAAAAAAABZQ/6EYfBQ6xyLA/s1600-h/img_1538.jpg)

Oddly enough, I found the guts of one of those shelves in the garbage and I will expose my findings here. Also, the system I found is in perfect working condition except for the power button which was broken.

## How the system works

One might think that the shelf contains a CD library that plays the selected CD on command (that is what I thought anyways). But it is much simpler than that. The system consists of a computer CD drive connected to a small computer power supply and a sort of IDE controller (run by a microcontroller). The IDE controller is told what to do by the user interface, a sort of large keypad hooked up to a(nother) microcontroller. The sound is taken from the CD drive by using the standard audio port.

[![](http://1.bp.blogspot.com/_940DBYqYeYo/SZyX5gO8HvI/AAAAAAAABZI/46H468NY8DQ/s320/img_1537.jpg)](http://1.bp.blogspot.com/_940DBYqYeYo/SZyX5gO8HvI/AAAAAAAABZI/46H468NY8DQ/s1600-h/img_1537.jpg)

[![](http://3.bp.blogspot.com/_940DBYqYeYo/SZyfaWk_lsI/AAAAAAAABaQ/fmU_zZvTo1w/s200/img_1551.jpg)](http://3.bp.blogspot.com/_940DBYqYeYo/SZyfaWk_lsI/AAAAAAAABaQ/fmU_zZvTo1w/s1600-h/img_1551.jpg)

But, how come it can play all the CDs if there is a single drive? Simple, it doesn't. It plays a special CD, with tracks corresponding to each one of the displayed CD. The tracks contain a mix featuring short samples of the CDs' songs. One can have the illusion the entire CD is playing since nobody stays near those shelves for long enough.

## Some Pictures

[![](http://2.bp.blogspot.com/_940DBYqYeYo/SZyZBnghwdI/AAAAAAAABZw/9T8-DPV4Wk0/s320/img_1545.jpg)](http://2.bp.blogspot.com/_940DBYqYeYo/SZyZBnghwdI/AAAAAAAABZw/9T8-DPV4Wk0/s1600-h/img_1545.jpg)

[![](http://2.bp.blogspot.com/_940DBYqYeYo/SZyYVb5e4AI/AAAAAAAABZY/4qiPZ80pTpI/s320/img_1541.jpg)](http://2.bp.blogspot.com/_940DBYqYeYo/SZyYVb5e4AI/AAAAAAAABZY/4qiPZ80pTpI/s1600/img_1541.jpg)

[![](http://3.bp.blogspot.com/_940DBYqYeYo/SZyYklj-ZEI/AAAAAAAABZg/QjF3o46rNfc/s320/img_1542.jpg)](http://3.bp.blogspot.com/_940DBYqYeYo/SZyYklj-ZEI/AAAAAAAABZg/QjF3o46rNfc/s1600-h/img_1542.jpg)

[![](http://2.bp.blogspot.com/_940DBYqYeYo/SZyYy8ZgtRI/AAAAAAAABZo/sMPncVxpJyA/s320/img_1543.jpg)](http://2.bp.blogspot.com/_940DBYqYeYo/SZyYy8ZgtRI/AAAAAAAABZo/sMPncVxpJyA/s1600-h/img_1543.jpg)

[![](http://1.bp.blogspot.com/_940DBYqYeYo/SZyZPk_sofI/AAAAAAAABZ4/_os1t7ULEiM/s320/img_1546.jpg)](http://1.bp.blogspot.com/_940DBYqYeYo/SZyZPk_sofI/AAAAAAAABZ4/_os1t7ULEiM/s1600/img_1546.jpg)

[![](http://2.bp.blogspot.com/_940DBYqYeYo/SZyZengJE2I/AAAAAAAABaA/5OrNvnnm9bs/s320/img_1549.jpg)](http://2.bp.blogspot.com/_940DBYqYeYo/SZyZengJE2I/AAAAAAAABaA/5OrNvnnm9bs/s1600-h/img_1549.jpg)

(BTW, I thing the pictures are much more enlightening than my explanation. They show the naked keypad, the back of the keypad with the microcontroller and dip switch position guide, the inside of the black box, and the IDE controller.)