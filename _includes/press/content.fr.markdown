<div class="row">
<div class="col-xs-12 col-md-4" markdown="1">

##Documents

###[Dossier de presse](https://drive.google.com/open?id=1btb1a-Dz3kX6AV9Bv84Qj7ZWSf9aj-8mZFQ5sGgaC7g&authuser=0)

###[Dossier de communication](https://drive.google.com/folderview?id=0B8qoF4rdMqh_aEtPWWNLbkx5aFU&usp=sharing)

###[Newsletters](http://us7.campaign-archive1.com/?u=b0542d8d13b538bc63aa779a9&id=fbc5baff8a)

</div>
<div class="col-xs-12 col-md-4" markdown="1">

## Contact Presse

OXYGEN Strasbourg

Tel. +33 (0)3 67 10 05 68

[evek@oxygen-rp.com](mailto:evek@oxygen-rp.com)

Jérémie LOTZ

[jlotz@oxygen-rp.com](mailto:jlotz@oxygen-rp.com)

Eve KEMLER
</div>
<div class="col-xs-12 col-md-4" markdown="1">

## Contact Communication

ALSACE DIGITALE

Sébastien LETELIE

Tel: +33 (0)3 88 41 86 95
Tel. +33 (0)6 24 72 04 96

[s.letelie@hackinghealth.ca](mailto:s.letelie@hackinghealth.ca)

</div>
</div>

##Ils parlent de nous !

<section class="press">
  <div class="container">
      <div class="row category">
        <div class="col-xs-12">
          <ul class="list-inline">
	   {% for blogPost in site.blogPost %}
            <li>
              <div class="img-container">
	      	{% assign blogpost_name = blogPost.name | downcase | replace:" ","-" | replace:"é","e" | remove:"!" | split:"-" | join:"-" | append:".jpg" %}
		{% assign img_url= "/img/partner/" | append: blogpost_name | prepend: site.baseurl %}
                <a href="{{ blogPost.url }}" target="_blank">
                  <img src="{{ img_url }}" alt="{{ blogPost.title }}" class="img-responsive" />
                </a>
              </div>
            </li>
          {% endfor %}
          </ul>
        </div>
      </div>
  </div>
</section>
