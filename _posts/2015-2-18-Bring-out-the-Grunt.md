---
layout: post
title: Bring out the Grunt
tags: [Jekyll, Grunt, CSS]
image: /images/grunt.jpg
description: Unused CSS can make loading your website slow. Grunt can do the job for you to strip your css files into one small one. Using grunt with Jekyll. 
---

For a new project website I decided to use a Jekyll installation with a theme that I liked: [Shiori](http://ellekasai.github.io/shiori/). I started in the usual way, importing the posts into the _posts directory, editing the _config file in the root file, and customizing the theme to my liking: changing its colors, navigation and sidebar. 

![The Grunt is very powerful](/images/grunt.jpg)

<!--read more-->

So far so good. But when rendering the site I was surprised seeing the filesize of the css-output; it was over 200kb big. For the project I was working on, that was way too big. It would take about 80% of the total bandwidth for a single pageload.

Upon further investigating I noticed the theme was made with Bootstrap. Therefore there was lots of unneeded CSS loaded into the global css file. This file was full with unnecessary code to render the website. I was sure the css that the site would require didn't have to be more than a mere 20 kb file. Surely there must be a way to strip this down I thought.

This is when I encountered *[Grunt](http://gruntjs.com/)*, a taskrunner to automate things such as minimizing your CSS. I really didn't have much time to dive into it and just went straight into getting what I wanted. After following some instructions I just let it run through my _site directory (so much for automation before _site is generated ;-) and it did exactly that: from a 200kb it generated a little just over 20kb css file. Job done. Publish site. 

Sure there must be a better way to integrate the Grunt even better with Jekyll automating its css output to a bare minimum, but that's for another time. *Further reading?* See also this [manual](http://addyosmani.com/blog/removing-unused-css/) on how to use grunt to strip down your css.

