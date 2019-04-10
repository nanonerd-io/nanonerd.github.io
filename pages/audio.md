---
layout: page
show_meta: false
title: "Audio"
# subheadline: "Audio by Kayhan"
# teaser: "Some of my audio work I've done"
header:
   image_fullwidth: "header_audio_bw.jpg"
   caption: I sprinkle binary bits on my alphabits. <br>The cyberlife and times of Kayhan B, digital librarian extraordinaire, podcaster and all around nice guy.
permalink: "/audio/"
---

![Dquarium Logo](/images/dquarium-logo-small.png)

Dquarium Podcasts are audio podcasts that discuss everything and anything related to digital technology. Go to <a href="https://dquarium.com">dquarium.com</a> now

<br>
<hr>
<br>

<p class="teaser">
   {% for post in site.posts limit:25 %}
      {% if post.exclude_podcast_rss != true %}
            <a href="{{ site.url }}{{ post.url }}">{{ post.title }}</a><br>
            {{post.teaser}}
            <p>
         	<audio controls>
               <source src="{{ post.file }}" type="audio/mp3">
            </audio>
            </p>
            {{post.description}}
            <p>
            <a href="{{ site.url }}{{ post.url }}">Read More</a> | <a href="{{ site.url }}/podcast.xml">Podcast RSS Feed</a>
            <hr>
      {% endif %}
   {% endfor %}
</p>
