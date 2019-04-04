---
layout: page
show_meta: false
title: "Search"
header:
   image_fullwidth: "header_blue.png"
   caption: I sprinkle binary bits on my alphabits. <br>The cyberlife and times of Kayhan B, digital librarian extraordinaire, podcaster and all around nice guy.
permalink: "/search/"
---

{% include google_search.html %}

<form style="padding-bottom: 200px;" onsubmit="google_search()" >
  <input type="text" id="google-search" placeholder="{{ site.data.language.enter_search_term }}">
</form>
