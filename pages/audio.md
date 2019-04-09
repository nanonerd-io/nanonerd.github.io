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

   <div class="row">
        <div class="medium-6 columns">
            {% for post in site.posts limit:1 %}
            {% if post.exclude_podcast_rss != true %}
                {% if post.subheadline %}<p class="subheadline">{{ post.subheadline }}</p>{% endif %}
                <h2><a href="{{ site.url }}{{ post.url }}">{{ post.title }}</a></h2>
                <p>
                    {% if post.meta_description %}{{ post.meta_description | strip_html | escape }}{% elsif post.teaser %}{{ post.teaser | strip_html | escape }}{% endif %}
                    <a href="{{ site.url }}{{ post.url }}" title="Read {{ post.title escape_once }}"><strong>{{ site.data.language.read_more }}</strong></a>
                </p>
            {% endif %}
            {% endfor %}
        </div>
   </div>

#### Dquarium Podcasts

![Dquarium Logo](/images/dquarium-logo-small.png)

Dquarium Podcasts are audio podcasts that discuss everything and anything related to digital technology. Here is a podcast called Bibliotech, a show that discusses all things digital technology in libraries
