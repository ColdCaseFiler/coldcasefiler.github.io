---
layout: page
title: Theories
descriptions: Various theories of how the crime may have occurred.
show_collection: theories
no_groups: true
---

{% assign theories = site.theories %}
{% for theory in theories %}
  {% theory %}
{% endfor %}
