---
layout: post
title: How to change jekyll theme
---

So you just installed Jekyll and got your blog running through the <a href="https://pages.github.com/">github pages</a>. But how can you change the site's layout or theme? The general approach is to create a new installation, name that into username.github.io, copy your old posts and images into the new folders, and other custom stuff.

<h2>Jekyll themes</h2>
There is all kinds of nice Jekyll themes, most of them clean, minimal and functional. Check for example <a href="http://jekyllthemes.org/">Jekyllthemes.org</a> for a quick overview of some templates. And there is even a lot more themes worth checking out and are not listed there. Check the long <a href="https://github.com/jekyll/jekyll/wiki/Themes">list of themes</a> on the Jekyll Wiki.

<h3>Requirements</h3>
<ul><li>Make sure you've got Jekyll <a href="http://jekyllrb.com/docs/installation/">installed</a>.</li>
<li>For easy testing check <a href="http://localhost:4000">localhost:4000</a> if you've got your site working locally.</li><li> If that's not the case, just type <code>jekyll serve</code> while in your site's directory</li> </ul>

<h2>Make a new installation</h2>
To use themes you should create a new installation based on that theme and then merge or migrate your posts and other custom stuff from the old to the new installation.
<p>
Fork your new theme into your Git repository, rename it (click on settings) and name it yourusername.github.io. Then clone it.
</p>
<h3>Following steps:</h3>
<ul><li>Removed content in the post directory and copied the _posts/ from the old installation into new directory. Also copy stuff that's in _images/ if any.
<li>Copied also the file "about.md" from the old installation to the new one.</li> 
<li>If you have made any more customisations, then copy those too into the new directory as well.</li>
<li>Edit the new _config.yml that came with your new theme to suite your needs</li>
</ul>

<h3>Troubleshooting</h3>
For some reason the posts didn't show up initially. That was a bummer. Why? I found out that it was because I had copied my backup files of the posts into the new folder as well. Due to this the posts didn't show up. Deleting the backup files did the trick.

<!--
<h2>Jekyll Bootstrap</h2>
With Jekyll Bootstrap it's pretty straightforward to change your theme. All you need to do is <a href="http://jekyllbootstrap.com/usage/jekyll-quick-start.html">install it</a>. Dir into the installation and change the theme with this one simple command. 

<code><a href="https://rubygems.org/gems/rake">rake</a> theme:install git="https://github.com/jekyllbootstrap/theme-the-minimum.git" --trace</code>

There is not many <a href="http://themes.jekyllbootstrap.com/">themes on bootstrap</a> (yet) but its ease of use is really nice. And of course, you can also clone existing themes and make them <a href="http://jekyllbootstrap.com/api/theme-api.html">available</a> for Bootstrap yourself.


(<small>note: It is at this point that I encounter <a href="http://ruhoh.com/">http://ruhoh.com/</a> which seems to be a lot easier to deploy with different themes</small>)

-->
