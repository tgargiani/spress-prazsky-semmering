---
layout: "page"
title: "Fotogalerie"
pictures:
   Žvahov:
      title: "Žvahov"
      picture: zvahov.jpg 
      picture_cc: 'Honza Groh, <a href="https://creativecommons.org/licenses/by-sa/3.0">CC BY-SA 3.0</a>'
      picture_url: "https://commons.wikimedia.org/wiki/File:Praha-%C5%BDvahov,_p%C5%99%C3%ADst%C5%99e%C5%A1ek.jpg"
   Jinonice:
      title: "Jinonice"
      picture: jinonice.jpg 
      picture_cc: 'VitVit, <a href="https://creativecommons.org/licenses/by-sa/4.0/deed.en">CC BY-SA 4.0</a>'
      picture_url: "https://commons.wikimedia.org/wiki/File:Jinonice_n%C3%A1dra%C5%BE%C3%AD_0.jpg"   
---

{% for P in page.pictures %}
<div class="photo">
    <h2>{{ P.title }}</h2>
	<p><img src="{{ site.url }}/assets/img/{{ P.picture }}" /></p>
   	<p class="author">&copy; {{ P.picture_cc }},
    <a href="{{ P.picture_url }}">originál</a>
  	</p>
</div>
{% endfor %}