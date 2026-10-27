---
layout: default
title: Inicio
---

<section class="hero">
  <p class="eyebrow">PORTAFOLIO · DESARROLLO DE SOFTWARE · SISTEMAS</p>
  <h1>Mateo Ronquillo<br><span>Desarrollo de soluciones digitales.</span></h1>
  <p class="intro">Estudiante y desarrollador enfocado en aplicaciones web, integración de servicios y sistemas orientados al análisis académico. Presento aquí una selección de proyectos, áreas de trabajo y aprendizajes técnicos.</p>
  <a class="button" href="{{ '/sobre-mi/' | relative_url }}">Perfil profesional <span aria-hidden="true">↗</span></a>
  <div class="hero-note"><span class="spark">MR</span><span>Ingeniería de software · integración · análisis de datos</span></div>
</section>

<section class="posts-section" id="bitacora">
  <div class="section-heading"><div><p class="eyebrow">PROYECTOS Y EXPERIENCIA</p><h2>Trabajo seleccionado</h2></div><span class="muted">Desarrollo, arquitectura y aprendizaje técnico</span></div>
  <div class="post-grid">
    {% for post in site.posts %}
    <article class="post-card">
      <div class="card-meta"><span>{{ post.category | default: 'Proyectos' }}</span><time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: '%d.%m.%Y' }}</time></div>
      <h3><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
      <p>{{ post.excerpt | strip_html | truncate: 145 }}</p>
      <a class="read-link" href="{{ post.url | relative_url }}">Ver proyecto <span aria-hidden="true">→</span></a>
    </article>
    {% endfor %}
  </div>
</section>

<section class="about-strip" id="enfoque"><div><p class="eyebrow">ENFOQUE</p><h2>Diseño y desarrollo con atención al contexto y a las personas usuarias.</h2></div><p>Mi trabajo combina análisis de requisitos, construcción de software, integración de sistemas y documentación técnica. Me interesa crear soluciones mantenibles que respondan a necesidades concretas.</p></section>

