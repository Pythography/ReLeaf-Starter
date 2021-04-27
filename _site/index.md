---
title: Welcome
date: Created
layout: page
tags:
  - home
  - welcome
  - info
---
<body>
<h>Testing </h1>
<ul>
{%- for post in collections.post -%}
  <li>{{ post.data.title }}</li>
{%- endfor -%}
</ul>
</body>