---
layout: post
title:  "Back To Top Button"
date:   2015-10-14
categories: snippet javascript jquery html css
---

This is the `HTML` portion

    <a id="back-to-top" href="#" class="back-to-top" role="button">&#94;</a>

This is the `CSS` portion

    .back-to-top {
        cursor: pointer;
        position: fixed;
        bottom: 10px;
        right: 10px;
        display:none;
    }

This is the `JAVASCRIPT` portion

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
