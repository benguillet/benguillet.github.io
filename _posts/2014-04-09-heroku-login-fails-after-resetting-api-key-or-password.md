---
layout:     post
title:      Fix heroku login
date:       2014-04-09 11:59
summary:    If it fails after resetting the api key (or the password).
categories: heroku heartbleed
---

If you are using this awesome Heroku accounts plugin: [https://github.com/ddollar/heroku-accounts](https://github.com/ddollar/heroku-accounts),
you might not be able to login using the heroku toolbelt after an api key reset. The reason is because the plugin
stores a copy of the key in:

{% highlight bash %}
~/.heroku/accounts/<account_name>
{% endhighlight %}

So to be able to log in again, you just need to update this file with the new api key. Then a simple `heroku login` should work.
