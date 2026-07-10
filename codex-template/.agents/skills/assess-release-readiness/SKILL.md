---
name: assess-release-readiness
description: Consolida evidencia de producto, ingeniería, QA y plataforma para decidir si un MVP o versión puede liberarse. Usar antes de despliegue, piloto, publicación o promoción entre ambientes.
---

# Assess Release Readiness

1. Confirmar versión y alcance aprobado.
2. Verificar criterios de aceptación y reporte QA.
3. Verificar build, pruebas, seguridad, migraciones y documentación.
4. Verificar despliegue, configuración, observabilidad, smoke tests y rollback.
5. Enumerar riesgos residuales con impacto, mitigación, propietario y aceptación.
6. Emitir:
   - `pass`: sin bloqueadores;
   - `conditional-pass`: riesgos aceptados explícitamente;
   - `fail`: existe al menos un bloqueador.
7. No desplegar; entregar decisión y evidencia al responsable autorizado.

