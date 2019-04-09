---
layout: page
show_meta: false
title: "Audio"
# subheadline: "Audio by Kayhan"
teaser: "Some of my audio work I've done"
header:
   image_fullwidth: "header_audio_bw.jpg"
   caption: I sprinkle binary bits on my alphabits. <br>The cyberlife and times of Kayhan B, digital librarian extraordinaire, podcaster and all around nice guy.
permalink: "/audio/"
---

#### Podcast

<ul>
    {% for post in site.posts limit:1 %}
      {% if post.exclude_rss != true %}
         <li><a href="{{ site.url }}{{ post.url }}">{{ post.title }}</a></li>
      {% endif %}
    {% endfor %}
</ul>

#### Dquarium Podcasts

![Dquarium Logo](/images/dquarium-logo-small.png)

Dquarium Podcasts are audio podcasts that discuss everything and anything related to digital technology. Here is a podcast called Bibliotech, a show that discusses all things digital technology in libraries
