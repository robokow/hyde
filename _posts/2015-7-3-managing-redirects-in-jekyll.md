---
layout: post
title: Managing Redirects in Jekyll
tags: [Jekyll]
#image: /images/editing-from-terminal.jpg
---
I moved one repository to another at Github and wanted to create 301 redirects from one Github Pages to another in an easy way. I couldn't use [jekyll-redirect-from](https://github.com/jekyll/jekyll-redirect-from) for this because I need a redirect to, not from. The "redirect from" is hosted in a different repository than "redirect to". That's where the issue comes from.

This turned out fairly easy though. I created a new layout call `redirects.html` in the repo using the old name, following the same style as "Jekyll Redirect From" generates in your _site folder when you use it in the way it's designed.

```
{% raw %}
<!DOCTYPE html>
<meta charset=utf-8>
<title>Redirecting...</title>
<link rel=canonical href="{{redirect_to}}">
<meta http-equiv=refresh content="0; url={{redirect_to}}">
<h1>Redirecting...</h1>
<a href="{{redirect_to}}">Click here if you are not redirected.</a>
<script>location='{{redirect_to}}'</script>
</html>
{% endraw %}
```

Then I add the page that I want to redirect. The permalink is the old link you used to visit the page. 

``` 
---
layout: redirect
redirect_to: /jekyll/about/
permalink: /about/
--- 
```

You probably still need to enable [jekyll-redirect-from](https://github.com/jekyll/jekyll-redirect-from) to make this work though.
