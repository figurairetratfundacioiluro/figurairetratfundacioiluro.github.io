---
layout: page
title: "Obres de l'exposició Figura<span class='copulativa'>i</span><span class='light'>Retrat</span>"
category: mur-diari
---

<div class="posts clearfix">
  {% for post in site.categories['simboliques'] reversed %}
  <div class="post">

    {{ post.excerpt }}    

  <h2 class="post-title">
      <a href="{{ post.url }}">
        {{ post.title }}
      </a>
    </h2>
    <p class="text-center"><a href="{{ post.url }}"><i class="fa fa-lg fa-plus-square-o"></i></a></p>
    </div>
  {% endfor %}
</div>
---
<div class="posts clearfix">
  {% for post in site.categories['figuracions'] reversed %}
  <div class="post">

    {{ post.excerpt }}    

  <h2 class="post-title">
      <a href="{{ post.url }}">
        {{ post.title }}
      </a>
    </h2>
    <p class="text-center"><a href="{{ post.url }}"><i class="fa fa-lg fa-plus-square-o"></i></a></p>
    </div>
  {% endfor %}
</div>
---
<div class="posts clearfix">
  {% for post in site.categories['retrats'] reversed %}
  <div class="post">

    {{ post.excerpt }}    

  <h2 class="post-title">
      <a href="{{ post.url }}">
        {{ post.title }}
      </a>
    </h2>
    <p class="text-center"><a href="{{ post.url }}"><i class="fa fa-lg fa-plus-square-o"></i></a></p>
    </div>
  {% endfor %}
</div>