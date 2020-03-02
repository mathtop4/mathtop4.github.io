---
layout: default
title: math-top4
---

<div id="home">
  <h1> 最新目录 </h1>
  <ul class="posts">
    {% for post in site.categories.annals limit:1 %}
      <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
    {% for post in site.categories.acta limit:1  %}
      <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
    {% for post in site.categories.jams limit:1  %}
      <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
    {% for post in site.categories.inventiones limit:1 %}
      <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
    <h1> 相关文章 </h1>
    {% for post in site.categories.other %}
      <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
  </ul>
    <!-- {% for cat in site.categories %}
      {% if cat[0] == "other" %}
        <h1> 相关文章 </h1>
      {% endif %}
      {% for post in cat[1] %}
        <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ post.url }}">{{ post.title }}</a></li>
      {% endfor %}
    {% endfor %} -->
  <!-- </ul> -->

  <h1>四大杂志官网</h1>
  <ul class="posts">
    <li><span>29 Feb 2020</span> &raquo; <a href="http://annals.math.princeton.edu/">Annals of Mathematics</a></li>
    <li><span>29 Feb 2020</span> &raquo; <a href="https://www.intlpress.com/site/pub/pages/journals/items/acta/_home/_main/index.php">Acta Mathematica</a></li>
    <li><span>29 Feb 2020</span> &raquo; <a href="http://www.ams.org/journals/jams/all_issues.html">Journal of The American Mathematical Society</a></li>
    <li><span>29 Feb 2020</span> &raquo; <a href="https://link.springer.com/journal/volumesAndIssues/222">Inventiones Mathematicae</a></li>
  </ul>
</div>
