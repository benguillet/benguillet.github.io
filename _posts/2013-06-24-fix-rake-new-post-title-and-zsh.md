---
layout:     post
title:      Fix rake new_post['title'] and Zsh
date:       2013-06-24 16:09
summary:
categories: octopress, rake, zsh, bug
---

There is a bug with Zsh and the Octopress `rake new_post` command.

Everytime you try to create a new post using this command, you get this:
{% highlight bash %}
$ rake new_post["My new post"]
zsh: no matches found: new_post[My new post]
{% endhighlight %}

The only workaround so far is:
{% highlight bash %}
rake new_post\["My new post"\]
{% endhighlight %}

