---
layout: post
title: The Power of Yaml
tags: [Jekyll, Yaml, Liquid]
image: /jekyll/images/jekyllrb-docs-variables-screenshot.jpg
description: Customising Jekyll is very easy as soon as you grasp Yaml and Liquid. My experience on how you can make use of these powerful tools. 
---

Very little I knew about *Liquid*, *Yaml* and *Rubi* until I caught up with Jekyll, the software this website is generated with. Up until a week ago I only had heard of Rubi (I actually have one of its cookbooks) but never did anything with it. Now I am blown away by the ease of use of Yaml and how, together with Liquid, it forms a powerful duo. It makes customising this website dead easy.

	---
	layout: post
	title: The Power of Yaml
	tags: [Jekyll, Yaml, Liquid]
	image: /images/jekyllrb-docs-variables-screenshot.jpg
	description: Customising Jekyll is very easy as soon as you grasp Yaml and Liquid. My experience on how you can make use of these powerful tools.
	---
<p id="caption">Jekyll frontmatter styled with Yaml</p>

At first when I was reading into Jekyll I had no clue about Yaml, let alone what was meant with the term "[frontmatter](http://jekyllrb.com/docs/frontmatter/)". Now I do know. It's a basic way to define all sorts of variables for the post that I am writing. These [variables](http://jekyllrb.com/docs/variables/) you can easily pull into your posts and sites with Liquid.

>The front matter is where Jekyll starts to get really cool.

Apart from basic stuff such as post-title and which default layout to use, it also gives me the option to define featured images that go with the post. Or what about tags? Just add them in the Yaml frontmatter! My mind got blown away with the ease of this. 

There is also other stuff that can go into the Yaml front-matter, such as a site-description which is pretty important for the types of sites that I manage. And I am sure there is more to come across while diving into Jekyll.

But the Yaml front-matter is not much without Liquid. It's with Liquid that you pull the frontmatter into the posts and into the layouts. It takes me some time to figure out how to do this (especially as a non-coder) but its power is very clear to me. In any case, even setting these [custom variables](http://jekyllrb.com/docs/frontmatter/#custom-variables) is not hard to understand. Your key is Yaml if you want to master Jekyll.

*Further reading:* 

 * <http://sampedley.com/jekyll-tricks/>
 * <http://jekyllrb.com/docs/frontmatter/> 

