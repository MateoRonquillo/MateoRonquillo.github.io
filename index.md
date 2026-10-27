---
layout: default
title: Inicio
---

<section class="hero">
  <p class="eyebrow">DESARROLLO · APRENDIZAJE · TECNOLOGÍA</p>
  <h1>Hola, soy Mateo.<br><span>Construyo, aprendo y comparto.</span></h1>
  <p class="intro">Este es mi espacio para documentar ideas, proyectos y lecciones que voy encontrando en el camino: desde aplicaciones académicas hasta redes y desarrollo de software.</p>
  <a class="button" href="{{ '/sobre-mi/' | relative_url }}">Un poco sobre mí <span aria-hidden="true">↗</span></a>
  <div class="hero-note"><span class="spark">✳</span><span>Aprender haciendo, mejorar en cada iteración.</span></div>
</section>

<section class="posts-section" id="bitacora">
  <div class="section-heading"><div><p class="eyebrow">LA BITÁCORA</p><h2>Ideas en proceso</h2></div><span class="muted">Proyectos, aprendizajes y notas</span></div>
  <div class="post-grid">
    {% for post in site.posts %}
    <article class="post-card">
      <div class="card-meta"><span>{{ post.category | default: 'Notas' }}</span><time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: '%d.%m.%Y' }}</time></div>
      <h3><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
      <p>{{ post.excerpt | strip_html | truncate: 145 }}</p>
      <a class="read-link" href="{{ post.url | relative_url }}">Leer nota <span aria-hidden="true">→</span></a>
    </article>
    {% endfor %}
  </div>
</section>

<section class="about-strip"><div><p class="eyebrow">LO QUE ME MUEVE</p><h2>La tecnología cobra sentido cuando ayuda a alguien.</h2></div><p>Me interesa resolver problemas reales con software, entender cómo funcionan las cosas y explicar lo aprendido con claridad. Aquí voy guardando parte de ese recorrido. ;D</p></section>
