---
layout: layout.njk
pageTitle: Overzicht van mijn recepten
---

<h1>{{ pageTitle }}</h1>

Met een beetje tekst **bold** of _italic_ of gewone tekst?

{%- for recept in collections.recepten -%}
    <h2><a href="..{{ recept.url }}">{{ recept.data.naam }}</a></h2>
    <p>{{ recept.data.ingredienten }}</p>
{%- endfor -%}