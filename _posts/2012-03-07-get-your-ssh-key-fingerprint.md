---
layout:     post
title:      Get your SSH Key Fingerprint
date:       2012-03-7 02:55
summary:    When Github has been attacked, better verify your ssh keys.
categories: security
---

Always helpful especially when GitHub has been [attacked](https://github.com/blog/1068-public-key-security-vulnerability-and-mitigation) and asks for the verification of all you SSH keys...

{% highlight bash %}
$ ssh-keygen -lf ~/.ssh/ssh_host_rsa_key.pub
2048 d6:59:bc:0b:18:ba:17:15:41:fc:d0:2a:60:f4:7e:e8 ~/.ssh/ssh_host_rsa_key.pub
{% endhighlight %}
