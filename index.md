---
layout: default
---

# Liste des Guidelines

{% for file in site.static_files %}
  {% if file.path contains '.pdf' %}
    - [{{ file.basename }}]({{ site.baseurl }}{{ file.path }})
  {% endif %}
{% endfor %} 
