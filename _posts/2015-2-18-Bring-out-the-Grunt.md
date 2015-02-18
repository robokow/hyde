---
layout: post
title: Bring out the Grunt
tags: [Jekyll, Grunt, CSS]
image: /images/grunt.jpg
description: Unused CSS can make loading your website slow. Grunt can do the job for you to strip your css files into one small one. Using grunt with Jekyll. 
---

For a new project website I decided to use a Jekyll installation with a theme that I liked: [Shiori](http://ellekasai.github.io/shiori/). I imported my posts into the Jekyll installation base, editing the config file, and customized the theme to my liking, chaning colors, navigation and sidebar. 

So far so good. But when rendering the website I was a bit in shock to see the filesize of the css-output, that one was over 200kb big. For the project I was working on, that was too big.

Upon further investigating I noticed the theme was made with Bootstrap. Hence there were lots of unneeded CSS loaded into the global css file. This was all code that was not needed to render the pages of the website. I was sure the css needed couldn't be more than a 20 kb file. Surely there must be a way to strip this down I thought.

![The Grunt is very powerful](/images/grunt.jpg)

This is when I encountered *[Grunt](http://gruntjs.com/)*, which is a taskrunner to automate things such as minimizing your CSS. I really didn't have much time to dive into it and just went straight into getting what I wanted. After following some instructions I just let it run through my _site directory (so much for automation before _site is generated ;-) and it did exactly that: from a 200kb it generated a little just over 20kb css file. Job done. Publish site.

There must be a way to integrate the grunt even better with Jekyll, but that's for another time. See also this [manual](http://addyosmani.com/blog/removing-unused-css/) on how to use grunt to strip down your css.

