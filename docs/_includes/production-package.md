{% case page.lang %}
{% when 'en' %}
{% capture production_package_content %}{% include en/production-package.md %}{% endcapture %}
{% when 'ru' %}
{% capture production_package_content %}{% include ru/production-package.md %}{% endcapture %}
{% when 'th' %}
{% capture production_package_content %}{% include th/production-package.md %}{% endcapture %}
{% else %}
{% capture production_package_content %}{% include en/production-package.md %}{% endcapture %}
{% endcase %}

<div class="production-package text-content">
{{ production_package_content | markdownify }}
</div>