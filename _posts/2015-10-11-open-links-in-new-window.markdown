---
layout: post
title:  "[jQuery] Open External Links in a New Window"
date:   2015-10-11
categories: snippet javascript jquery
---

This snippet will open external links in a new window using jQuery/Javascript

    $('a').each(function() {
       var a = new RegExp('/' + window.location.host + '/');
       if(!a.test(this.href)) {
           $(this).click(function(event) {
               event.preventDefault();
               event.stopPropagation();
               window.open(this.href, '_blank');
           });
       }
    });
