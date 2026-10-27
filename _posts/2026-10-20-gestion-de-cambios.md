---
layout: post
title: "Aplicación web para la gestión de solicitudes de cambio"
date: 2026-10-20 09:00:00 -0500
category: Desarrollo de software
excerpt: "Implementación de un flujo de control de cambios con roles diferenciados, seguimiento de estados e historial de decisiones."
---

Este proyecto convierte un proceso de control de cambios en una aplicación web para registrar, revisar y dar seguimiento a solicitudes operativas y técnicas.

La solución utiliza **FastAPI** para la API, una interfaz web y **SQLite** para la persistencia. El modelo contempla perfiles de usuario, administrador y desarrollador, con permisos asociados a sus responsabilidades. Las solicitudes recorren estados de revisión, aprobación, implementación, pruebas y cierre; las decisiones relevantes quedan registradas en un historial.

Un aspecto central fue traducir las reglas del proceso a validaciones concretas: control de acceso a las solicitudes, requisitos para aprobar, asignación de responsables y conservación del contexto de cada petición. El diseño vincula interfaz, permisos y flujo de trabajo para mantener trazabilidad durante todo el ciclo.

**Áreas abordadas:** desarrollo backend, diseño de APIs, persistencia de datos, control de acceso, modelado de procesos y experiencia de usuario.
