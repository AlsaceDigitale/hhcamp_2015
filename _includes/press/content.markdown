#They are talking about us !

<section class="press">
<div class="container">
<div class="col-xs-12">
<ul class="list-inline">
{% for blogPost in site.blogPost %}
<li >
<div class="img-container">
{% assign blogpost_name = blogPost.name | downcase | replace:" ","-" | replace:"é","e" | remove:"!" | split:"-" | join:"-" | append:".jpg" %}
<a target="_blank" href="{{blogPost.url}}">
{% assign image_url= "/img/partner/" | append: blogpost_name | prepend: site.baseurl %}
<img class="img-responsive" alt="{{ blogPost.title }}" src="{{ image_url }}" />
</a>
</div>
</li>
{% endfor %}
</ul>
</div>
</div>
</section>

#Documents

###[press kit](https://drive.google.com/open?id=1btb1a-Dz3kX6AV9Bv84Qj7ZWSf9aj-8mZFQ5sGgaC7g&authuser=0)

###[communication kit](https://drive.google.com/folderview?id=0B8qoF4rdMqh_aEtPWWNLbkx5aFU&usp=sharing)

###[newsletters](http://us7.campaign-archive1.com/?u=b0542d8d13b538bc63aa779a9&id=fbc5baff8a)