#They are talking about us !

<section class="press">
<div class="col-xs-12">
<ul class="list-inline">
{% for blogPost in site.blogPost %}
{% assign blogPostImage = blogPost.name | downcase | replace:" ","-" | replace:"é","e" | remove:"!" | split:"-" | join:"-" | prepend: "img/partner/" | append:".jpg" %}
<li >
<div class="img-container">
<a target="_blank" href="{{blogPost.url}}">
<img class="img-responsive" alt="{{blogPost.title}}" src="{{blogPostImage}}">
</img>
</a>
</div>
</li>
{% endfor %}
</ul>
</div>
</section>

