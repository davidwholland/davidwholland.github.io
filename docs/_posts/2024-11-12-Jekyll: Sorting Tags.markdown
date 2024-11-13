---
layout: post
title:  "How to Sort Tags in Jekyll"
date:   2024-11-12 22:12:26 -0400
tags: jekyll programming
---

As I'm making more extensive use of Jekyll, I noticed that the [Tags](/tags) page seemed to be sorted randomly. That seems like an odd default. But a bit of searching revealed a simple way to fix it.

The [Tags](/tags) page is generated from a file called `tags.markdown`. It's simple, and it turns out that making the tags sort alphabetically only requires changing two lines.

{% highlight liquid %}
{% raw %}
{% assign sorted_tags = site.tags | sort %}
{% for tag in sorted_tags %}
  <h3>{{ tag[0] }}</h3>
  <ul>
    {% for post in tag[1] %}
      <li><a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
  </ul>
{% endfor %}
{% endraw %}
{% endhighlight %}

The first change is to add the following line:

{% highlight liquid %}
{% raw %}
{% assign sorted_tags = site.tags | sort %}
{% endraw %}
{% endhighlight %}

This change sets up the new variable called `sorted_tags` and sorts the Jekyll-provided array called `site.tags`. Once we have that, it's easy to replace `site.tags` in the loop below.

{% highlight liquid %}
{% raw %}
{% for tag in sorted_tags %}
{% endraw %}
{% endhighlight %}

*Et voilà!* Sorted tags for everyone. Don't let the power go to your head.