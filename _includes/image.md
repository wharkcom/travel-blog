{% if include.caption and include.image and include.alt and include.source %}
<figure>
	<img src="{{site.image_path}}/{{include.source}}/{{include.image}}" alt="{{include.alt}}" />
	<figcaption>{{include.caption}}</figcaption>
</figure>
{% elsif include.image and include.alt and include.source %}
<img src="{{site.image_path}}/{{include.source}}/{{include.image}}" alt="{{include.alt}}" />
{% endif %}