---
layout: post
title: How to change jekyll theme
---

So you just installed Jekyll and got your blog running. But how to change the site's layout or theme. That's not so straightforward to do. The general approach is say to have a new installation and you choose your theme beforehand. But what if you haven't done so and you just went ahead with the default theme that comes with the most used installation.

<h2>Jekyll themes</h2>
There is all kinds of nice Jekyll themes, most of them clean, minimal and functional. Check for example <a href="http://jekyllthemes.org/">Jekyllthemes.org</a> for a quick overview of some templates. And there is even a lot more themes worth checking out and are not listed there. Check the long <a href="https://github.com/jekyll/jekyll/wiki/Themes">list of themes</a> on the Jekyll Wiki.

<h3>Requirements</h3>
<ul><li>Make sure you've got Jekyll <a href="http://jekyllrb.com/docs/installation/">installed</a>.</li>
<li>For easy testing check <a href="http://localhost:4000">localhost:4000</a> if you've got your site working locally.</li><li> If that's not the case, just type <code>jekyll serve</code> while in your site's directory</li> </ul>

<h2>Jekyll Bootstrap</h2>
With Jekyll Bootstrap it's pretty straightforward to change your theme. All you need to do is <a href="http://jekyllbootstrap.com/usage/jekyll-quick-start.html">install it</a>. Dir into the installation and change the theme with this one simple command. 

<code><a href="https://rubygems.org/gems/rake">rake</a> theme:install git="https://github.com/jekyllbootstrap/theme-the-minimum.git" --trace</code>

There is not many <a href="http://themes.jekyllbootstrap.com/">themes on bootstrap</a> (yet) but its ease of use is really nice. And of course, you can also clone existing themes and make them <a href="http://jekyllbootstrap.com/api/theme-api.html">available</a> for Bootstrap yourself.

<h2>Make a new installation</h2>
To use themes that are not included in Bootstrap (well, that's most of them) you could merge or migrate your existing posts and other custom stuff to a new installation.

<strong>Don't follow these instructions, they are a work in progress and probably not good</strong>

Fork your new theme into your Git repository. Then clone it. I am choosing <a href="https://github.com/poole/hyde">Hyde</a> here, because that one goes well with Jekyll. Once done I took the following steps:

<ul><li>Removed posts directory and Copied _posts from the old installation into the new directory. And delete any other posts that came along with the new theme.
<li>Copy also the file about.md if you've changed that.</li> 
<li>If you have made any more customisations, then copy those too into the new directory as well</li>
<li>Edit the new _config.yml that came with your new theme to suite your needs</li>
<li>Remove any custom stuff that came along with the new theme</li></ul>


Once everything is completed,  Renaming Didn't work. Trying to work this out.


(<small>note: It is at this point that I encounter <a href="http://ruhoh.com/">http://ruhoh.com/</a> which seems to be a lot easier to deploy with different themes</small>)
