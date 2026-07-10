# Technical Pack: Plataforma y entrega

## Topologías

- Plataforma administrada/PaaS para reducir operación del MVP.
- Contenedores cuando se necesita empaquetado consistente o portabilidad.
- Kubernetes cuando escala organizacional y operativa lo justifican, no como requisito automático.
- Serverless para eventos o carga variable con límites compatibles.
- Máquinas virtuales para compatibilidad o control específico.

## Estrategias de despliegue

- Recreate: simple, acepta indisponibilidad.
- Rolling: reemplazo gradual con compatibilidad entre versiones.
- Blue/Green: cambio rápido y rollback a costa de duplicación temporal.
- Canary: exposición progresiva con señales confiables.
- Feature flags: separar despliegue de liberación; gobernar eliminación de flags.

## Controles mínimos

- Build reproducible y artefacto inmutable.
- Escaneo de dependencias, secretos e infraestructura.
- Configuración separada del artefacto.
- Migraciones compatibles y estrategia de rollback.
- Logs estructurados, métricas, trazas y alertas accionables.
- Backups probados, RTO/RPO y runbooks.
- Principio de mínimo privilegio y auditoría.

