---
layout: post
title:  "Installation of Jekyll"
date:   2014-12-08 10:10:10
categories: jekyll
---

### Requirements

Installing Jekyll is easy and straight-forward, but there are a few requirements
you’ll need to make sure your system has before you start.

- Ruby
- RubyGems
- Linux, Unix, or Mac OS X
- NodeJS

#### Install NodeJS 
{% highlight bash %}
$ sudo apt-get install nodejs
{% endhighlight %}

#### Install ruby2.1-dev 
{% highlight bash %}
$ sudo apt-get install ruby2.1-dev
{% endhighlight %}

#### Install Jekyll
{% highlight bash %}
$ sudo gem install jekyll
$ jekyll --version
{% endhighlight %}

Now that you’ve got everything installed, let’s get to work!

### Quick-start Instructions

{% highlight bash %}
$ jekyll new my-awesome-site
$ cd my-my-awesome-site
$ jekyll serve
{% endhighlight %}

Now browse to http://localhost:4000
