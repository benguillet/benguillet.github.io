---
layout: post
title: Fix SSL error with ruby 2.0 and Rails4 on OSX
date: 2013-06-24 18:06
summary:
categories: ruby2.0 rails4 gem
---

If you encounter this error when trying to bundle install:
{% highlight bash %}
Gem::RemoteFetcher::FetchError: SSL_connect returned=1 errno=0 state=SSLv3 read server certificate B: certificate verify failed
{% endhighlight %}

Then it probably means than you need to upgrade your rubygem version.
Check the current version:
{% highlight bash %}
$ gem -v
{% endhighlight %}

You need to use at least the 2.0.3. To upgrade, just run:
{% highlight bash %}
$ gem update --system
{% endhighlight %}

