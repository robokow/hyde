---
layout: post
title: Adding tags to Jekyll
tags: [Jekyll]
---

Well, that's an easy one but as a beginner it took me some time to figure out. To add a tag simply at the existing [Yaml data](http://jekyllrb.com/docs/frontmatter/) on top of the post. See the codebox below. This ease of use was a mind-blower to me. But my main question remained: how to show the tag on the rendered posts?

    ---
    layout: post
    title: Adding tags to Jekyll
    tags: [Jekyll]
    ---

That was not easy to figure out for someone who knows little about Liquid. I tried several solutions, but finally got it working when I followed these [instructions](http://charliepark.org/tags-in-jekyll/) and added the code below in my template *post.html* file.


	<h2>Tags:</h2> {.% for tag in page.tags %} <a href="/tags/{{ tag }}">{{ tag }}</a> {.% if forloop.last != true %} {.% endif %} {.% endfor %}

<p id="caption">When copying, you have to remove the dots before the %</p>

That did the trick. Things aren't perfect yet though, there is no hyphens between the words of multiple-word-tags and I also noticed a problem with capital letters in my slugs. Also, in order to get the tags working with github pages I also manualy copied the <code>/_site/tags</code> folder into a separate <code>/tags</code> folder at the rootlevel.

So far not a fully automated tag system but nevertheless something I am pleased to work with. I am generally happy to see how easy it is to use Jekyll and how I learn while doing it. I know there is many other systems out there, but for now I first like to set up a decent site with this framework.

