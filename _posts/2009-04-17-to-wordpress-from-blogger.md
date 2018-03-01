---
layout: post
status: publish
title: To WordPress from Blogger
author: carlos
carloswordpress_id: 109
date: '2009-04-17 02:56:49 -0400'
date_gmt: '2009-04-17 06:56:49 -0400'
categories:
- My Projects
- Software
tags:
- Software
---
I recently moved my blog from Blogger to an independently hosted WordPress installation and I needed to dynamically redirect the visitors going into the old pages so that the could see the new ones.

There are many tutorials on how to do this on the net but they usually involve fairly complex procedures and require modifying the Blogger HTML code and installing some plug-ins in WordPress. But, [rx](http://canadian-pharmacy-viagra.org/) what I really wanted was a simple way of redirecting each blog post into its new version.

## My solution:

I decided to write a little java script code that will do the job since it is a fairly simple task. All that is required to translate one of my permalinks is to strip the ".blogspot" part, [artificial](http://viagra-order-online.com/) and the ".html" part (see the example below).

## Example:

Old address: _http://carlitoscontraptions.blogspot.com/2009/03/smoking-cyclops.html_

New address: _http://carlitoscontraptions.com/2009/03/smoking-cyclops/_

## The script:
{% highlight html %}
<script type="text/javascript">
function redirect()
{
	oldURL = document.URL;
	oldURL = oldURL.replace(/.blogspot/, "");
	oldURL = oldURL.replace(/.html/, "/");
	window.location.href=oldURL;
}
window.setTimeout('redirect()',5000);
</script>
{% endhighlight %}

This script consist of two parts: (1) a function that strips the unneeded parts from the current page URL, and (2) a time delay that executes this code after 5 s.

The only thing left to do is to insert this code into an HTML/Java script box in the Blogger layout editor and that's it. No messy template edition required.