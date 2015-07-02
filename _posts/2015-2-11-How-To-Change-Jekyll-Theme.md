---
layout: post
title: How to change Jekyll theme
tags: [Jekyll]
image: /jekyll/images/changing-themes-jekyll.jpg
---

So you just installed Jekyll and got your blog running through the <a href="https://pages.github.com/">github pages</a>. But how can you change the site's layout or theme? One approach that works is to fork the new theme you want, rename it into username.github.io, and then copy from your previous installation your old posts, images and other custom content that you would like to maintain.

![Changing themes at Jekyll]({{ site.baseurl }}/images/changing-themes-jekyll.jpg)

<!--more-->

<h2>Jekyll themes</h2>
There is all kinds of nice Jekyll themes, most of them clean, minimal and functional. Check for example <a href="http://jekyllthemes.org/">Jekyllthemes.org</a> for a quick overview of some templates. And there is even a lot more themes worth checking out and are not listed there. Check the long <a href="https://github.com/jekyll/jekyll/wiki/Themes">list of themes</a> on the Jekyll Wiki.

###Requirements
 * Make sure you've got Jekyll <a href="http://jekyllrb.com/docs/installation/">installed</a>.
 * For easy testing type <code>jekyll serve</code> in your terminal and see it at <a href="http://localhost:4000">localhost:4000</a> to know you've got your site working locally.

##Make a new installation
To use themes there is a couple of ways. One way is to make a new installation based on that theme and then merge or migrate your posts and other custom stuff from the old to the new installation.

Then fork your new theme into your Git repository and rename it (click on settings) to <i>yourusername.github.io</i>. Then clone the git locally. This <a href="https://raw.githubusercontent.com/robokow/robokow-old-github/master/images/step1.gif">little video-image</a> explains it all. I then made the following steps:

 * Removed content in the post directory and copied the _posts/ from the old installation into new directory. Also copy stuff that's in _images/ if any.
 * Copied also the file "about.md" from the old installation to the new one.
 * If you have made any more customisations, then copy those too into the new directory as well.
 * Edit the new _config.yml that came with your new theme to suite your needs

<h2>Jekyll Bootstrap</h2>
With Jekyll Bootstrap it's pretty straightforward to change your theme. All you need to do is <a href="http://jekyllbootstrap.com/usage/jekyll-quick-start.html">install it</a>. Dir into the installation and change the theme with this one simple command. 

<code><a href="https://rubygems.org/gems/rake">rake</a> theme:install git="https://github.com/jekyllbootstrap/theme-the-minimum.git" --trace</code>

There is not many <a href="http://themes.jekyllbootstrap.com/">themes on bootstrap</a> (yet) but its ease of use is really nice. And of course, you can also clone existing themes and make them <a href="http://jekyllbootstrap.com/api/theme-api.html">available</a> for Bootstrap yourself.

(<small>note: It is at this point that I encounter <a href="http://ruhoh.com/">http://ruhoh.com/</a> which seems to be a lot easier to deploy with different themes</small>)

