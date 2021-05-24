---
layout: page
title: Theories
descriptions: Various theories of how the crime may have occurred.
show_collection: theories
no_groups: true
---

{% for theory in site.theories %}
  <a href="/theories/{{ theory }}/">{{ theory }}</a><br>
{% endfor %}
