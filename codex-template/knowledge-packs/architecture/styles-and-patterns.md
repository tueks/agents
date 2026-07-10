# Technical Pack: Estilos y patrones de arquitectura

## Selección por drivers

No seleccionar por popularidad. Comparar simplicidad, cambio esperado, escala, autonomía, consistencia, operación y capacidades del equipo.

## Estilos

| Estilo | Útil cuando | Riesgo frecuente |
| --- | --- | --- |
| Monolito modular | MVP y equipos pequeños con dominios separables | Convertirse en monolito sin límites |
| Arquitectura en capas | Dominio relativamente simple y flujo estable | Dependencias hacia infraestructura |
| Hexagonal / Ports and Adapters | Dominio importante y múltiples adaptadores | Abstracciones ceremoniales sin necesidad |
| Clean / Onion | Se necesita proteger reglas de negocio | Exceso de capas y mapeos |
| Microservicios | Equipos y capacidades necesitan autonomía real | Complejidad distribuida prematura |
| Event-driven | Productores y consumidores desacoplados, reacción asíncrona | Contratos débiles y difícil observabilidad |
| Serverless | Carga variable y operación administrada | Lock-in, límites y depuración distribuida |

## Patrones de sistema distribuido

- API Gateway cuando se necesita un punto controlado de entrada, no para ocultar contratos incoherentes.
- CQRS cuando modelos de lectura y escritura tienen necesidades realmente distintas.
- Event Sourcing cuando el historial de eventos es parte central del dominio, no solo para auditoría.
- Saga para coordinar consistencia entre límites sin transacción global.
- Outbox para publicar eventos de manera consistente con cambios locales.
- Strangler Fig para migración incremental de sistemas existentes.
- Circuit Breaker, timeout, retry con jitter y bulkhead para resiliencia; definir idempotencia antes de reintentar.

## Preguntas de selección

- ¿Cuál es el cambio más probable durante los próximos 12 meses?
- ¿Qué límites requieren despliegue o escalado independiente?
- ¿Qué consistencia exige el negocio?
- ¿Qué fallas distribuidas puede operar el equipo?
- ¿Qué decisión puede posponerse hasta tener evidencia?

