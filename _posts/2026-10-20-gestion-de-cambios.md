---
layout: post
title: "Del formulario al flujo: diseñar una app para gestionar cambios"
date: 2026-10-20 09:00:00 -0500
category: Proyectos
excerpt: "Lo que aprendí al llevar un proceso de control de cambios a una aplicación con roles, estados e historial."
---

Un formulario puede parecer sencillo hasta que varias personas necesitan usarlo, revisarlo y tomar decisiones sobre él. En una aplicación de **gestión de cambios**, el reto fue convertir ese proceso en un flujo claro.

La solución que desarrollé usa una API con FastAPI, una interfaz web y SQLite para conservar las solicitudes. Los perfiles de usuario, administrador y desarrollador tienen responsabilidades distintas. Las solicitudes avanzan por estados —revisión, aprobación, implementación, pruebas y cierre— y las decisiones quedan registradas en un historial.

Lo más interesante fue traducir reglas del proceso a comportamiento concreto: quién puede ver cada solicitud, qué información necesita una aprobación, cuándo se puede asignar una persona y cómo se mantiene el contexto de una petición. La interfaz importa, pero la coherencia entre permisos, datos y flujo es lo que hace confiable la herramienta.

Me quedo con una idea práctica: antes de construir pantallas, conviene dibujar el recorrido de las personas y las decisiones que toman.
