---
layout: default
title: math-top4
---

<div id="home">
  <h1> 最新目录 </h1>
  <ul class="posts">
    {% for cat in site.categories %}
      {% if cat[0] == "math" %}
        <h1> 最新一期目录 </h1>
      {% endif %}
      {% if cat[0] == "AI" %}
        <h1> {{ cat[0] }}文章列表 </h1>
      {% endif %}
      {% if cat[0] == "other" %}
        <h1> 其他文章列表 </h1>
      {% endif %}
      {% for post in cat[1] %}
        <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ post.url }}">{{ post.title }}</a></li>
      {% endfor %}
    {% endfor %}
  </ul>

  <h1>四大杂志官网</h1>
  <ul class="posts">
    <li><span>29 Feb 2020</span> &raquo; <a href="http://annals.math.princeton.edu/">Annals of Mathematics</a>
    <li><span>29 Feb 2020</span> &raquo; <a href="https://www.intlpress.com/site/pub/pages/journals/items/acta/_home/_main/index.php">Acta Mathematica</a>
    <li><span>29 Feb 2020</span> &raquo; <a href="http://www.ams.org/journals/jams/all_issues.html">Journal Of The American Mathematical Society</a>
    <li><span>29 Feb 2020</span> &raquo; <a href="https://link.springer.com/journal/volumesAndIssues/222">Inventiones Mathematicae</a>
  </ul>
</div>
