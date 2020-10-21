---
layout: layout.njk
pageTitle: Welcome to my blog
---

# Overzicht van recepten

Met een beetje tekst **bold** of _italic_ of gewone tekst? Toch

{%- for recept in collections.recepten -%}
    <h2><a href="/_site{{ recept.url }}">{{ recept.data.title }}</a></h2>
    <p>{{ recept.data.intro }}</p>
    <p>{{ recept.data.ingredienten }}</p>
{%- endfor -%}