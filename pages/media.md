---
layout: kz-page
title:
permalink: "/media/"
meta_description:
header: no
widgets:
- url: https://unworldoceansday.org/2020
  image: world-ocean-day-2020.jpg
  title: <a href="https://unworldoceansday.org/2020" target="_self">UN World Oceans Day 2020</a>
  text: I was an invited speaker, see 5:09:30 in the video.
- url: https://www.globalcitizen.org/en/content/plastic-pollution-cameroon-youth-activist/
  image: global-citizen.jpg
  title: <a href="https://www.globalcitizen.org/en/content/plastic-pollution-cameroon-youth-activist/" target="_self">'Plastic Man'&#58; This Cameroonian Activist Is Working to End Plastic Pollution in His Community</a>
  text: In June 2020...



  


---

<div class="row">
  {% for widget in page.widgets %}
    {% assign loopindex = forloop.index | modulo: 3 %}
    <div id="{{ widget.anchor }}">{% include _frontpage-widget.html widget=widget %}</div>
    {% if loopindex == 0 %}
  <hr style="height:1px; visibility:hidden;" /> <!-- Prevents long first column items from pushing new rows to the right -->
    {% endif %}
  {% endfor %}
</div>
