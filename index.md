---
layout: layout.njk
pageTitle: Welcome to my blog
---

# My Homepage

Met een beetje tekst **bold** of _italic_ of gewone tekst? Toch

{%- for post in collections.posts -%}
    <h2><a href="{{ post.url }}">{{ post.data.title }}</a></h2>
    <p>{{ post.data.intro }}</p>
    <p>Date: {{ post.date | date: "%d-%m-%Y" }}</p>
{%- endfor -%}