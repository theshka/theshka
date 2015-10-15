---
layout: post
title:  "Back To Top Button"
date:   2015-10-14
#image: "/assets/img/x.jpg"
categories: snippet javascript jquery html css
---
This snippet of `HTML`, `CSS`, and `JAVASCRIPT` will create a back-to-top button on your site.

This is the `HTML` portion
{% highlight html %}
<a id="back-to-top" href="#" class="back-to-top" role="button">&#94;</a>
{% endhighlight %}

This is the `CSS` portion
{% highlight css %}
.back-to-top {
    cursor: pointer;
    position: fixed;
    bottom: 10px;
    right: 10px;
    display:none;
}
{% endhighlight %}

This is the `JAVASCRIPT` portion
{% highlight javascript %}
$(document).ready(function(){
    $(window).scroll(function () {
        if ($(this).scrollTop() > 585) {
            $('#back-to-top').fadeIn();
        } else {
            $('#back-to-top').fadeOut();
        }
    });
    // scroll body to 0px on click
    $('#back-to-top').click(function () {
        $('body,html').animate({
            scrollTop: 0
        }, 800);
        return false;
    });
});
{% endhighlight %}
