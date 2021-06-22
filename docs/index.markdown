---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
title: Home
---

## Documentation

Here are links to the documentation of QuiltMC's projects:

{% for doc in site.javadocs %}
- [{{ doc }}]({{ doc | downcase | relative_url }})
{%- endfor -%}
