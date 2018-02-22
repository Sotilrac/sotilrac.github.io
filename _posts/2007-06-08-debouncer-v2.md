---
layout: post
status: publish
published: true
title: Debouncer v2
author: carlos
date: '2007-06-08 23:56:00 -0400'
date_gmt: '2007-06-09 06:56:00 -0400'
categories:
- My Projects
- FPGA
tags: []
---
I wrote a quick debouncer code in VHDL that I thought people could enjoy and may be useful for FPGA projects. For more info on debouncers see [this post](http://carlitoscontraptions.com/2007/03/switch-debouncer/ "Switch debouncer").

As shown in the block diagram below, it takes as inputs a switch signal (SW_IN) and a clock signal (CLK) and outputs a signal SIG.

[![](http://4.bp.blogspot.com/_940DBYqYeYo/RmpRwgO16GI/AAAAAAAAASk/LDFQuLpOTYU/s320/CC_Debouncer.png)](http://4.bp.blogspot.com/_940DBYqYeYo/RmpRwgO16GI/AAAAAAAAASk/LDFQuLpOTYU/s1600-h/CC_Debouncer.png)

When SW_IN goes high, the module outputs a once-clock-cycle wide pulse on the next clock rising edge. Then it waits for 8388607 clock cycles (~ 0.17 s when clocked @ 50MHz). This is illustrated in the state transition diagram below.

[![](http://3.bp.blogspot.com/_940DBYqYeYo/RmpRwQO16FI/AAAAAAAAASc/r-01Ch0cJxI/s320/CC_Debouncer+std.png)](http://3.bp.blogspot.com/_940DBYqYeYo/RmpRwQO16FI/AAAAAAAAASc/r-01Ch0cJxI/s1600-h/CC_Debouncer+std.png)

You can download the code [here](http://carlos.asmat.googlepages.com/CC_Debouncer.vhd).