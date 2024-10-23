---
layout: post
title:  "Getting Started with Jekyll and GitHub Pages"
date:   2024-10-22 21:39:02 -0400
tags: jekyll dayone
---

The [walkthrough][walkthrough] on GitHub worked pretty well to get up and running with Jekyll.
* Remember that if you want the Jekyll site to live in a folder inside the root of your repo, it must be named `docs`.
* Blog post files have to be named in the right format: `YEAR-MONTH-DAY-title.MARKUP`.
* Use `jekyll serve` to run the web server and regenerate the site.

Jekyll also does [code snippets][code-snippets]:

{% highlight csharp %}
string player1 = "Crosby";
string player2 = "Malkin";
string player3 = "Guentzel";

// Brute force comparison (equality only)
bool isSamePlayer = player1.Length == player3.Length;
if (isSamePlayer)
{
    for (int i = 0; i < player1.Length; i++)
    {
        if (player1[i] != player3[i])
        {
            isSamePlayer = false;
            break;
        }
    }
}
{% endhighlight %}

The [Jekyll docs][jekyll-docs] are thorough. Bugs and feature requests can be found at [Jekyll’s GitHub repo][jekyll-gh]. Ask questions on [Jekyll Talk][jekyll-talk].

[code-snippets]: https://jekyllrb.com/docs/liquid/tags/#code-snippet-highlighting
[walkthrough]: https://docs.github.com/en/pages/setting-up-a-github-pages-site-with-jekyll/about-github-pages-and-jekyll
[jekyll-docs]: https://jekyllrb.com/docs/home
[jekyll-gh]:   https://github.com/jekyll/jekyll
[jekyll-talk]: https://talk.jekyllrb.com/
