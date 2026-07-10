# Technical Pack: Backend

## Patrones de diseño y aplicación

- Application Service / Use Case para coordinar una intención del usuario.
- Repository cuando el dominio necesita una abstracción de persistencia; evitarlo como envoltorio mecánico sin valor.
- Unit of Work cuando varias operaciones locales comparten transacción.
- Specification para reglas de consulta o selección reutilizables, con atención a traducción y rendimiento.
- Strategy para políticas intercambiables.
- Factory para construcción que protege invariantes.
- Decorator o middleware para preocupaciones transversales.
- Result para errores esperados; excepciones para condiciones excepcionales según convención.
- Domain Events para comunicar hechos dentro o fuera del límite, distinguiendo eventos internos e integración.

## Selección por lenguaje

| Ecosistema | Fortalezas típicas | Preguntas adicionales |
| --- | --- | --- |
| .NET / C# | APIs, dominio empresarial, tooling y rendimiento | Versión, ASP.NET Core, EF/Dapper, DI, hosting |
| Java / Kotlin | Ecosistema empresarial y JVM | Spring/Quarkus/Micronaut, build, persistencia |
| Python | Automatización, datos y APIs rápidas | Framework, typing, concurrencia, packaging |
| Node.js / TypeScript | I/O, integración y stack compartido | Runtime, framework, validación, async |
| Go | Servicios simples, concurrencia y despliegue | Librerías, manejo de errores, contratos |
| PHP | Web y ecosistemas maduros | Framework, runtime, workers y deployment |

## Reglas

- Registrar versiones exactas en el proyecto, no en este paquete.
- Consultar documentación oficial cuando una API o comportamiento dependa de versión.
- Seguir primero los patrones ya demostrados en el repositorio.
- Introducir una abstracción solo si protege un límite, invariantes o cambio esperado.

