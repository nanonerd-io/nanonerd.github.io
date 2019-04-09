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

<p class="teaser">
    {% for post in site.posts limit:25 %}
      {% if post.exclude_podcast_rss != true %}
         <a href="{{ site.url }}{{ post.url }}">{{ post.title }}</a><br>
         	<audio controls>
					<source src="{{ page.file }}" type="audio/mp3">
				</audio>
      {% endif %}
    {% endfor %}
</p>

#### Dquarium Podcasts

![Dquarium Logo](/images/dquarium-logo-small.png)

Dquarium Podcasts are audio podcasts that discuss everything and anything related to digital technology. Here is a podcast called Bibliotech, a show that discusses all things digital technology in libraries
