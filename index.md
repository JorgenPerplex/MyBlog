---
layout: layout.njk
pageTitle: Welkom!

---

<h1>{{ pageTitle }}</h1>

Met een beetje tekst **bold** of _italic_ of gewone tekst?

{%- for recept in collections.recepten  -%}
    <h2><a href="/_site{{ recept.url }}">{{ recept.data.title }}</a></h2>
    <p>{{ recept.data.intro }}</p>
    <p>{{ recept.data.ingredienten }}</p>
{%- endfor -%}