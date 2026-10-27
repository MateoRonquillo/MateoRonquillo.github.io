---
layout: default
title: Inicio
---

<section class="hero">
  <p class="eyebrow">PORTAFOLIO <span>/</span> DESARROLLO DE SOFTWARE <span>/</span> SISTEMAS</p>
  <h1>Mateo Ronquillo<span class="title-period">.</span><br><span class="hero-subtitle">Desarrollo de soluciones digitales.</span></h1>
  <p class="intro">Estudiante y desarrollador enfocado en aplicaciones web, integración de servicios y sistemas para el análisis académico. Este portafolio reúne proyectos, áreas de trabajo y aprendizajes técnicos.</p>
  <div class="hero-actions"><a class="button" href="{{ '/sobre-mi/' | relative_url }}">Perfil profesional <span aria-hidden="true">↗</span></a><a class="text-link" href="#proyectos">Explorar proyectos <span aria-hidden="true">↓</span></a></div>
  <div class="hero-note"><span class="spark">MR</span><span>Ingeniería de software · integración · análisis de datos</span></div>
</section>

<section class="posts-section" id="proyectos">
  <div class="section-heading"><div><p class="eyebrow">01 / SELECCIÓN</p><h2>Proyectos destacados</h2></div><span class="muted">Diseño, desarrollo y formación técnica</span></div>
  <div class="post-grid">
    {% for post in site.posts %}
    <article class="post-card">
      <div class="card-meta"><span>{{ post.category | default: 'Proyectos' }}</span><time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: '%d.%m.%Y' }}</time></div>
      <h3><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
      <p>{{ post.excerpt | strip_html | truncate: 145 }}</p>
      <a class="read-link" href="{{ post.url | relative_url }}">Detalles del proyecto <span aria-hidden="true">↗</span></a>
    </article>
    {% endfor %}
  </div>
</section>

<section class="about-strip" id="enfoque"><div><p class="eyebrow">02 / ENFOQUE</p><h2>Soluciones de software con atención al contexto y a quienes las utilizan.</h2></div><p>Mi trabajo combina análisis de requisitos, desarrollo de aplicaciones, integración de sistemas y documentación técnica. Me interesa construir soluciones mantenibles que respondan a necesidades concretas.</p></section>
