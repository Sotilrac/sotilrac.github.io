---
layout: post
status: publish
title: Fully Featured Media Center on a Budget
author: carlos
date: '2007-07-15 00:14:00 -0400'
date_gmt: '2007-07-15 07:14:00 -0400'
categories:
- My Projects
tags: []
---
Recently my girlfriend got rid of her cable television connection and moved to a cheaper (almost free) and fully featured media center solution (i.e. Xbox + Xbox Media Center).

[![](http://4.bp.blogspot.com/_940DBYqYeYo/RpxM_06eeQI/AAAAAAAAATI/9imY9X9iqHk/s320/800px-Xbox.jpg)](http://4.bp.blogspot.com/_940DBYqYeYo/RpxM_06eeQI/AAAAAAAAATI/9imY9X9iqHk/s1600-h/800px-Xbox.jpg)

## Meterials

*   Xbox (not 360)
*   Xbox remote (not required, but useful)
*   Xbox Controller (usually comes with the Xbox)
*   Xbox memory card (8 MB is enough)
*   Modded Xbox from a relative (for a one time use)
*   [MechAssault](http://www.xbox.com/en-US/games/m/mechassault/) game disk
*   Softmod installer
*   Computer, router, high speed internet connection, electricity (you should already have these).

## General Idea  
The idea is to unlock the Xbox, which is basically a very cheep computer, in order to run the very excellent and free Xbox Media Center (XBMC), a very advanced media player. Then, the Xbox can be use to watch videos, play music, stream content from the internet, and more (all in the comfort of the living room).

I know XBMC has been around for many years now, but I think is a good idea to write a post to show off its incredible features and explain how to get it.

## How to do it  
First, get all the materials. My girlfriend and I got a second hand Xbox complete with a remote and a controller for 100$ at Comptant.com after searching around a lot for a good deal. Then, I got a Mechassault original (not the platinum edition) game disk for 9$ and an 8MB memory card for 10$ (all second hand). So we spent a total of 120$ (much cheaper than any commercial media center).

In order to get the Xbox to run homebrew software (i.e. software that is not signed by Microsoft such as XBMC) its security system must be disabled. This can be done by installing a softmod (witch doesn't require any hardware modification of the gaming system).

I choose to use the [Krayzie Ndure SOFTMOD Pack](http://www.torrentbox.com/download/24832/XBOX%20Krayzie%20Ndure%20SOFTMOD%20Pack.torrent) that can be downloaded from the torrents. The idea is to get one of the game saves from this package (depending on which game you want to use) into the memory card and then into the Xbox. In order to get the MechAssault save to the memory card I used my own ([hard](http://www.xbox100.com/tutorials/beginnermodfaq.htm))modded Xbox: I copied the game save folder to the E:UDATA folder trough FTP and then I copied the game save (named Linux Installer) to the memory card by using the original Xbox dash. If you don't have access to a modded Xbox, there are other ways of getting the save to the Xbox such as [Action Replay](http://us.codejunkies.com/shop/product.asp?c=US&cr=USD&cs=$&r=0&amp;amp;amp;amp;amp;amp;amp;amp;amp;l=1&ProdID=119) or building a [USB adapter](http://www.xbox-linux.org/wiki/Xbox_Linux_USB_HOWTO).

Now, the easy part. Once you have the game save in the memory card, connect the Xbox to the router (as you would connect any other computer to it), plug the card into the controller, and turn the console on. Then, in the Xbox dash, go to the memory menu and copy the game save to the Xbox hard drive (hdd). Afterwards, insert the MechAssault disk, select the campaign menu entry, and then select "Linux Installer". This will take you to a dashboard that will guide you through the installation of the softmod. Simply follow the steps (back up the eeprom and install the softmod) and in less than 2 minutes you will have a modded Xbox with your dashboard of choice (you can chose between EvolutionX or UnleashedX).

Now you can play game backups, run unsigned software and much more. Note that you need to update the Xbox dash to the latest version in order for the softmod installer to work properly. This can be done by using the "Live" menu entry in the Xbox dash.

Now that the Xbox is modded, you need to install XBMC. I used the latest [Pimped](http://torrentspy.com/download.asp?id=1736745) version that comes with all the features you would want (codecs, scripts, visualizations, skins) and can be downloaded from the torrents. Once you have it downloaded and unziped, you must copy the XBMC folder to E:/apps in the Xbox's hdd (the usual applications folder) through FTP (sending files trough FTP is the standard way of installing application onto the Xbox).

For FTP communication with the Xbox you can use any FTP client you want (I use [Konqueror](http://www.konqueror.org/)). In order to connect to the Xbox you need to know its IP address (which is normally shown on the main menu of the evolution dashboard) and its user name (Xbox) and password (Xbox). for further information in connecting to the Xbox trough FTP, please see this site.

Once the XBMC folder has been copied to E:/apps, reboot the Xbox (this will update the dashboard menu), and go to the applications menu an chose Xbox Media Center in order to start this wonderful program. You can also set it to start automatically (I recommend this) by following [this guide](http://www.xboxmediacenter.com/wiki/index.php?title=As_a_Dashboard).

Now that you have XBMC up , running and connected to the internet you can:

*   play videos/music/pictures stored on any computer connected to router trough SMB (windows network) or stored in the local hd (it support almost all audio/video formats known to man).
*   Play PAL and NTSC DVDs/VCDs from any region.
*   Stream media from the internet, including tv shows, podcasts, movies, music, music videos, and much more.
*   Check the weather forecast.
*   And tons of other cool things.

## Some Screenshots

[![](http://1.bp.blogspot.com/_940DBYqYeYo/RpxN8E6eeWI/AAAAAAAAAT4/Ed97S4ftmaQ/s320/media.bmp)](http://1.bp.blogspot.com/_940DBYqYeYo/RpxN8E6eeWI/AAAAAAAAAT4/Ed97S4ftmaQ/s1600-h/media.bmp)

[![](http://1.bp.blogspot.com/_940DBYqYeYo/RpxRZE6eedI/AAAAAAAAAUw/_4Jkyl-J5tU/s320/video.bmp)](http://1.bp.blogspot.com/_940DBYqYeYo/RpxRZE6eedI/AAAAAAAAAUw/_4Jkyl-J5tU/s1600-h/video.bmp)

[![](http://1.bp.blogspot.com/_940DBYqYeYo/RpxN8E6eeXI/AAAAAAAAAUA/Wo-ZzWx2ypU/s320/movies_menu_2.bmp)](http://1.bp.blogspot.com/_940DBYqYeYo/RpxN8E6eeXI/AAAAAAAAAUA/Wo-ZzWx2ypU/s1600-h/movies_menu_2.bmp)

[![](http://1.bp.blogspot.com/_940DBYqYeYo/RpxN8E6eeYI/AAAAAAAAAUI/Dbd4m9mtd14/s320/movies_menu_1.bmp)](http://1.bp.blogspot.com/_940DBYqYeYo/RpxN8E6eeYI/AAAAAAAAAUI/Dbd4m9mtd14/s1600-h/movies_menu_1.bmp)

[![](http://2.bp.blogspot.com/_940DBYqYeYo/RpxN8U6eeZI/AAAAAAAAAUQ/EiRv3daDVkQ/s320/music.bmp)](http://2.bp.blogspot.com/_940DBYqYeYo/RpxN8U6eeZI/AAAAAAAAAUQ/EiRv3daDVkQ/s1600-h/music.bmp)

[![](http://4.bp.blogspot.com/_940DBYqYeYo/RpxRY06eebI/AAAAAAAAAUg/a2s1K1cgGo4/s320/shoutcast.bmp)](http://4.bp.blogspot.com/_940DBYqYeYo/RpxRY06eebI/AAAAAAAAAUg/a2s1K1cgGo4/s1600-h/shoutcast.bmp)

[![](http://4.bp.blogspot.com/_940DBYqYeYo/RpxM_06eeRI/AAAAAAAAATQ/XuQO5k7-SsA/s320/audio_playback.bmp)](http://4.bp.blogspot.com/_940DBYqYeYo/RpxM_06eeRI/AAAAAAAAATQ/XuQO5k7-SsA/s1600-h/audio_playback.bmp)

[![](http://1.bp.blogspot.com/_940DBYqYeYo/RpxNAE6eeSI/AAAAAAAAATY/TBBZjxQ6AWU/s320/games.bmp)](http://1.bp.blogspot.com/_940DBYqYeYo/RpxNAE6eeSI/AAAAAAAAATY/TBBZjxQ6AWU/s1600-h/games.bmp)

[![](http://2.bp.blogspot.com/_940DBYqYeYo/RpxNAU6eeUI/AAAAAAAAATo/qY5Xj7nnPtY/s320/live.bmp)](http://2.bp.blogspot.com/_940DBYqYeYo/RpxNAU6eeUI/AAAAAAAAATo/qY5Xj7nnPtY/s1600-h/live.bmp)

[![](http://4.bp.blogspot.com/_940DBYqYeYo/RpxN706eeVI/AAAAAAAAATw/NoNnM1gfOns/s320/live_places.bmp)](http://4.bp.blogspot.com/_940DBYqYeYo/RpxN706eeVI/AAAAAAAAATw/NoNnM1gfOns/s1600-h/live_places.bmp)

[![](http://4.bp.blogspot.com/_940DBYqYeYo/RpxRY06eecI/AAAAAAAAAUo/lZWySrV6inI/s320/trailers.bmp)](http://4.bp.blogspot.com/_940DBYqYeYo/RpxRY06eecI/AAAAAAAAAUo/lZWySrV6inI/s1600-h/trailers.bmp)

[![](http://3.bp.blogspot.com/_940DBYqYeYo/RpxRYk6eeaI/AAAAAAAAAUY/Anqxb5qu5eg/s320/playback.bmp)](http://3.bp.blogspot.com/_940DBYqYeYo/RpxRYk6eeaI/AAAAAAAAAUY/Anqxb5qu5eg/s1600-h/playback.bmp)

[![](http://1.bp.blogspot.com/_940DBYqYeYo/RpxRZE6eeeI/AAAAAAAAAU4/f1bQZqswWtw/s320/weather.bmp)](http://1.bp.blogspot.com/_940DBYqYeYo/RpxRZE6eeeI/AAAAAAAAAU4/f1bQZqswWtw/s1600-h/weather.bmp)

[![](http://1.bp.blogspot.com/_940DBYqYeYo/RpxNAE6eeTI/AAAAAAAAATg/_GIj-JwbwGM/s320/joox.bmp)](http://1.bp.blogspot.com/_940DBYqYeYo/RpxNAE6eeTI/AAAAAAAAATg/_GIj-JwbwGM/s1600-h/joox.bmp)

(note that the top and bottom black borders are not shown in the TV screen)

## Final Remarks  
Don't forget to configure XBMC to adjust it to your needs (I recommend using the MC360 skin). For further information about using XBMC please consult the [user's manual](http://www.xboxmediacenter.com/wiki/index.php?title=Xbox_Media_Center_Online_Manual).

You have now a very powerful media center that is far superior than any of the commercial alternatives I know. Enjoy.

Besides, you may also want to install some other great application such as [dvd2xbox,](http://dvd2xbox.xbox-scene.com/) which allows to backup entire games to the Xbox hdd, and [boXplorer](http://www.xbox-hq.com/html/modules.php?name=Xbox_Homebrew&amp;amp;amp;op=view&gid=288), an excellent file manager. You can get them from the [usual places](http://www.xbox-scene.com/articles/xbins.php).