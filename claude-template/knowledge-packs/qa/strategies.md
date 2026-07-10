# Knowledge Pack: QA y estrategia de pruebas

## Enfoque basado en riesgo

Priorizar por probabilidad, impacto, detectabilidad y frecuencia de uso.

## Tipos de prueba

- Unitarias: reglas y comportamiento aislado.
- Integración: base de datos, colas, archivos y dependencias reales controladas.
- Contrato: compatibilidad entre consumidores y proveedores.
- Componentes: interfaz y servicios en un límite útil.
- E2E: pocos journeys críticos de extremo a extremo.
- Exploratorias: aprendizaje, usabilidad y fallos no anticipados.
- Accesibilidad: automático y manual.
- Seguridad: SAST, dependencias, secretos, DAST y pruebas de autorización.
- Rendimiento: baseline, load, stress, spike y soak según riesgo.
- Resiliencia: timeouts, dependencias fallidas, reintentos y recuperación.

## Release gate sugerido

- Criterios de aceptación cumplidos.
- Sin defectos críticos o altos no aceptados.
- Regresión crítica aprobada.
- Migración y rollback verificados cuando aplican.
- Seguridad y observabilidad revisadas.
- Riesgos residuales con propietario y aceptación.

