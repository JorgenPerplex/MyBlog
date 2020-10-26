---
layout: layout.njk
pageTitle: Welkom!

---

<h1>{{ pageTitle }}</h1>

{%- for recept in collections.recepten  -%}
    <h2><a href="/_site{{ recept.url }}">{{ recept.data.naam }}</a></h2>
    <p>Kooktijd: {{ recept.data.kooktijd }}  |  Koolhydraten: {{ recept.data.koolhydraten }}</p>
    <p>{{ recept.data.ingredienten }}</p>
{%- endfor -%}