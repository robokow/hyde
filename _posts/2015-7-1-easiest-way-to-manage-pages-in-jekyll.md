---
layout: post
title: The easiest way to manage pages in Jekyll
tags: [Jekyll]
#image: /images/editing-from-terminal.jpg
---

It's easy to manage pages in Jekyll, but if you have quite a few of them, you may get some clutter in 
your main root folder. There is a really easy solution to this: just add your pages in a new index 
folder.

Simply put, just like you've got all your posts in your _posts folder, you can easily add all your pages 
in your index folder. Inside the index folder you add the main index.md file (the main index page). And add `permalink: /` in the yaml - or else you get a permission issue.

But inside the same folder you can easily add all your other pages. Just make sure you add a different 
permalink to it. You can do this simple by adding a permalink to it. For example, save the page 
about.md inside the /index folder. To make it actually work, just add this to the top of the page:

``` 
--- 
layout: page 
title: about
permalink: /about/ 
--- 
```

That's it. You can add as many pages to the folder as long as you designate them with a different 
permalink.
