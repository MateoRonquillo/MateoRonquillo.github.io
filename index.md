---
layout: default
title: Inicio
---

<section class="hero">
  <p class="eyebrow">DESARROLLO DE SOFTWARE · SISTEMAS · APRENDIZAJE</p>
  <h1>Soy Mateo Ronquillo.<br><span>Desarrollo soluciones tecnológicas.</span></h1>
  <p class="intro">Este sitio reúne proyectos, experiencias de aprendizaje y reflexiones sobre el desarrollo de software, la integración de sistemas y las tecnologías aplicadas a la educación.</p>
  <a class="button" href="{{ '/sobre-mi/' | relative_url }}">Perfil profesional <span aria-hidden="true">↗</span></a>
  <div class="hero-note"><span class="spark">✳</span><span>Diseño centrado en necesidades concretas y mejora continua.</span></div>
</section>

<section class="posts-section" id="bitacora">
  <div class="section-heading"><div><p class="eyebrow">PUBLICACIONES</p><h2>Proyectos y aprendizajes</h2></div><span class="muted">Notas sobre tecnología y desarrollo</span></div>
  <div class="post-grid">
    {% for post in site.posts %}
    <article class="post-card">
      <div class="card-meta"><span>{{ post.category | default: 'Notas' }}</span><time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: '%d.%m.%Y' }}</time></div>
      <h3><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
      <p>{{ post.excerpt | strip_html | truncate: 145 }}</p>
      <a class="read-link" href="{{ post.url | relative_url }}">Leer publicación <span aria-hidden="true">→</span></a>
    </article>
    {% endfor %}
  </div>
</section>

<section class="about-strip"><div><p class="eyebrow">ENFOQUE</p><h2>Tecnología orientada a resolver problemas.</h2></div><p>Me interesa diseñar e implementar soluciones útiles, comprender los sistemas que las hacen posibles y documentar con rigor las decisiones y los aprendizajes de cada proyecto.</p></section>
