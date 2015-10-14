---
layout: post
title:  "[HTML] Apple Web-App Meta"
date:   2015-10-12
categories: snippet html meta
---

Use these Apple Meta Tags to tailor your site's meta tags for Apple devices.

{% highlight html %}
<meta name="apple-mobile-web-app-title" content="My App"> <!-- New in iOS6 -->
<meta name='apple-mobile-web-app-capable' content='yes'>
<meta name='apple-touch-fullscreen' content='yes'>
<meta name='apple-mobile-web-app-status-bar-style' content='black'>
<meta name='format-detection' content='telephone=no'>
<meta name='viewport' content='width=device-width; content='width = 320; initial-scale=1.0; maximum-scale=1.0; user-scalable=yes; target-densitydpi=160dpi'>

<link href='/apple-touch-icon.png' rel='apple-touch-icon' type='image/png'>
<link href='touch-icon-ipad.png' rel='apple-touch-icon' sizes='72x72'>
<link href='touch-icon-iphone4.png' rel='apple-touch-icon' sizes='114x114'>
<link href='/startup.png' rel='apple-touch-startup-image'>

<link href='http://github.com/images/touch-icon-iphone4.png' sizes='114x114' rel='apple-touch-icon-precomposed'>
<link href='http://github.com/images/touch-icon-ipad.png' sizes='72x72' rel='apple-touch-icon-precomposed'>
<link href='http://github.com/images/apple-touch-icon-57x57.png' sizes='57x57' rel='apple-touch-icon-precomposed'>
{% endhighlight %}
