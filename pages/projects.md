---
layout: kz-page
title: "Projects"
permalink: "/projects/"
meta_description:
header: no
widgets:
- url: https://oceanic.global/projects/conscious-coloring-book/
  image: conscious-coloring-book.jpg
  title: <a href="https://oceanic.global/projects/conscious-coloring-book/" target="_self">Conscious Coloring Book</a>
  text: Text
- url: https://thinkoceanglobal.org/forbi
  image: think-ocean.jpg
  title: <a href="https://thinkoceanglobal.org/forbi" target="_self">Collaboration with ThinkOcean</a>
  text: Text
- url: https://greeningforward.org/programs/cameroon
  image: 2019_May_Comic_Contest.jpg
  title: <a href="https://greeningforward.org/programs/cameroon" target="_self">Greening Forward Cameroon</a>
  text: Text
- url: https://www.soalliance.org/blog/soa-cameroon-sea-turtle-conservation
  image: soa_project.jpg
  title: <a href="https://www.soalliance.org/blog/soa-cameroon-sea-turtle-conservation" target="_self">Collaboration with Sustainable Ocean Alliance</a>
  text: Text
- url: /projects/community_cleanups
  image: 2018_Jun_community_cleanup.jpg
  title: <a href="/projects/community_cleanups" target="_self">Collaboration with Sustainable Ocean Alliance</a>
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
