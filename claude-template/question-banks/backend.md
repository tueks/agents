# Banco de preguntas: Backend Engineer

## Contrato y casos de uso

1. ¿Qué casos de uso y criterios de aceptación implementará el backend?
2. ¿Qué actores o sistemas invocan cada operación?
3. ¿Qué protocolo y formato se utilizará: REST, gRPC, eventos, SOAP u otro?
4. ¿Qué compatibilidad y versionado requieren los contratos?
5. ¿Qué errores de negocio y técnicos debe distinguir el consumidor?

## Dominio y reglas

6. ¿Qué entidades, valores, agregados o estados participan?
7. ¿Qué invariantes deben preservarse?
8. ¿Qué operaciones requieren idempotencia?
9. ¿Qué transacciones necesitan atomicidad?
10. ¿Qué concurrencia o condiciones de carrera son posibles?

## Datos

11. ¿Qué información se persiste y durante cuánto tiempo?
12. ¿Qué motor y esquema existen o son candidatos?
13. ¿Qué consultas y volúmenes críticos se esperan?
14. ¿Se requiere migración, seed, importación o reconciliación?
15. ¿Qué datos son sensibles y cómo deben protegerse?

## Integraciones

16. ¿Qué APIs, colas, archivos o servicios externos se consumen?
17. ¿Qué límites, timeouts y políticas de reintento aplican?
18. ¿Cómo se evitan duplicados o inconsistencias?
19. ¿Qué fallback o compensación existe ante fallas?

## Seguridad y observabilidad

20. ¿Cómo se autentica y autoriza cada operación?
21. ¿Qué validación y sanitización se requiere?
22. ¿Qué eventos deben auditarse?
23. ¿Qué logs, métricas y trazas necesita soporte?
24. ¿Qué información no debe aparecer en errores o logs?

## Implementación y pruebas

25. ¿Qué lenguaje, versión, framework y convenciones utiliza el proyecto?
26. ¿Qué patrones existentes deben seguirse?
27. ¿Qué pruebas unitarias, integración, contrato y rendimiento aplican?
28. ¿Cómo se ejecuta localmente y en CI?
29. ¿Qué cambios requieren feature flag o despliegue coordinado?

## Criterios de salida

- Casos de uso y contratos definidos.
- Modelo, invariantes, persistencia y consistencia entendidos.
- Integraciones y fallas tratadas explícitamente.
- Seguridad y observabilidad incluidas.
- Estrategia de pruebas y despliegue acordada.
- Decisiones técnicas alineadas con arquitectura.

