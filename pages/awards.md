---
layout: kz-page
title: "Awards"
permalink: "/awards/"
meta_description:
header: no
widgets:
- url: https://gradesofgreen.org/announcing-the-2020-waste-campaign-eco-grant-awardees/
  image: award-changemaker-2020.jpg
  title: <a href="https://gradesofgreen.org/announcing-the-2020-waste-campaign-eco-grant-awardees/" target="_self">Grades of Green International Changemakers Award 2020</a>
  text: Text
- url: https://leadasap.ysa.org/share_story/everyday-young-hero-perise-forbi/
  image: award-everyday-hero.jpg
  title: <a href="https://leadasap.ysa.org/share_story/everyday-young-hero-perise-forbi/" target="_self">Youth Service America Everyday Young Hero Award 2019</a>
  text: Text
- url: https://tunza.eco-generation.org/resourcesView.jsp?boardID=winners&viewID=46212
  image: award-eco-hero.jpg
  title: <a href="https://tunza.eco-generation.org/resourcesView.jsp?boardID=winners&viewID=46212" target="_self">Tunza Eco-generation Hidden Eco Hero Award 2018</a>
  text: Text




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
