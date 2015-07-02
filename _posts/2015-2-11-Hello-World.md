---
layout: post
title: Hello world!
tags: [Jekyll]
image: /images/editing-from-terminal.jpg
---

I mostly use github as an instant messaging platform. And issue tracking from time to time. Now it also hosts my new blog. And I even got my first own repository. ha! What about that.

<h3>To do:</h3>
<ul><li>Figure out how not to type in username-pw each time I write something</li>
<li>How can I use gedit for example and commit posts with just one shortcut?</li>
</ul>

<h3>Done!</h3>
<code>
robino@leno:~/sites$ ssh -T git@github.com
Hi robokow! You've successfully authenticated, but GitHub does not provide shell access.
</code>

This is pretty neat! Without filling in any passwords or username been able to make a change to this blogpost! Still need to figure out the other step, because three cli commands is still quite a lot.

<h3>Jekyll Publish blog posts the easy way!</h3>
<strong>update</strong>: got it down two commands. <code>git commit -a -m "edit post" && git push origin master</code>. So after I save a new file, I just have to hit this command in the terminal and that's it to update or publish a new post. Nice :-)

**Update 2**: Got it into a script and now all I need to do is type one command. This is fantastic.

<img src="/images/editing-from-terminal.jpg">
