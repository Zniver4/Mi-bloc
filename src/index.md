---
layout: base.njk
title: Sobre mi
---

# {{ title }}

Hola mi nombre es Jonathan Zavala Acosta me gusta muchos editar vikdeos y programar vieojuegos soy fan de muchos animes 

[Acerca]({{ '/acerca' | url }})

## Artículos de mi Blog

### Categoría mis animes favoritos

{% for anime in collections.anime %}

- [{{anime.data.title}}]({{ anime.url | url }})

{% endfor %}

### Categoría de mis videojuegos favoritos

{% for videojuegos in collections.videojuegos %}

- [{{videojuegos.data.title}}]({{ videojuegos.url | url }})

{% endfor %}

### Categoría de mis peliculas favoritas

{% for peliculas in collections.peliculas %}

- [{{peliculas.data.title}}]({{ peliculas.url | url }})

{% endfor %}