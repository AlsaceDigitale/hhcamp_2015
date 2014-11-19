#Last Event description

##\<insert usefull desceription content here\>
<a href="http://projects.digitalhealthcamp.eu/" class="btn btn-primary btn-block">
          See projects from last event !
        </a>

{% for video in site.last_event_videos %}
<iframe width="380" height="285" src="{{video.url}}" frameborder="0" allowfullscreen>{{video.name}}</iframe>
{% endfor %}
