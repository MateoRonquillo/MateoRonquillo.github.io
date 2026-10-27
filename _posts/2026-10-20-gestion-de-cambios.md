---
layout: post
title: "Diseño de una aplicación para la gestión de cambios"
date: 2026-10-20 09:00:00 -0500
category: Proyectos
excerpt: "Implementación de un flujo digital para registrar solicitudes de cambio, gestionar responsabilidades y conservar un historial de decisiones."
---

El desarrollo de una aplicación para la **gestión de cambios** requiere traducir un proceso organizacional en reglas, responsabilidades y estados comprensibles. El objetivo del proyecto fue estructurar un flujo que permita registrar solicitudes, evaluarlas y dar seguimiento a su resolución.

La implementación utiliza FastAPI para la API, una interfaz web y SQLite para la persistencia de solicitudes. Los perfiles de usuario, administrador y desarrollador cuentan con permisos diferenciados. El flujo contempla revisión, aprobación, implementación, pruebas y cierre, con registro de las decisiones asociadas.

Una parte central del trabajo consistió en representar las reglas del proceso en el sistema: determinar el acceso a cada solicitud, definir la información necesaria para evaluarla, establecer las condiciones de asignación y conservar la trazabilidad. La consistencia entre permisos, datos y estados es esencial para que la aplicación refleje correctamente el procedimiento.

Este proyecto reforzó la importancia de modelar primero las responsabilidades y transiciones del proceso. Esa base ayuda a diseñar una interfaz más clara y una implementación más mantenible.
