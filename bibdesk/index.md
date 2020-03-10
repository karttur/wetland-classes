---
layout: page
title: Bibdesk reference
excerpt: "Jekyll generation of bibdesk reference file"
search_omit: true
---

<ul class="post-list">
{% for post in site.categories.literature %}

  {% if post.bibdesk %}
    <li><article>
    <span class="excerpt">{{ post.bibdesk | remove: '\[ ... \]' | remove: '\( ... \)' | markdownify | strip_html | escape_once | newline_to_br }}</span>
    </article></li>
  {% endif %}
{% endfor %}
</ul>
