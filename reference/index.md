---
layout: page
title: Bibdesk references
excerpt: "Jekyll generation of bibdesk reference file"
search_omit: true
---

<ul class="post-list">
{% for post in site.categories.reference %}
    {{ post.content | newline_to_br }}
{% endfor %}
</ul>
