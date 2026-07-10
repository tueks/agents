# Banco de preguntas: Software Architect

## Contexto y restricciones

1. ¿Qué alcance funcional y flujos ya están aprobados?
2. ¿Es greenfield, evolución o integración con un sistema existente?
3. ¿Qué tecnologías, proveedores o ambientes son obligatorios?
4. ¿Qué restricciones de equipo, presupuesto, plazo o licenciamiento existen?
5. ¿Qué decisiones están fuera del control del proyecto?

## Atributos de calidad

6. ¿Qué disponibilidad necesita el MVP y las versiones futuras?
7. ¿Qué latencia o tiempo de respuesta es aceptable en los flujos críticos?
8. ¿Qué volumen inicial y crecimiento se espera?
9. ¿Qué nivel de consistencia, durabilidad y recuperación requieren los datos?
10. ¿Qué objetivos existen para seguridad, privacidad y auditoría?
11. ¿Qué tan importante es portabilidad, extensibilidad o integración?
12. ¿Qué atributos son prioritarios y qué trade-offs se aceptan?

## Dominio y límites

13. ¿Cuáles son las capacidades y conceptos centrales del negocio?
14. ¿Qué reglas cambian juntas y cuáles deben aislarse?
15. ¿Qué módulos, bounded contexts o servicios se anticipan?
16. ¿Qué datos posee cada límite?
17. ¿Qué contratos cruzan límites?

## Integraciones y datos

18. ¿Qué sistemas externos participan y quién es su propietario?
19. ¿Las integraciones son síncronas, asíncronas, por archivos o manuales?
20. ¿Qué sucede si una dependencia externa falla?
21. ¿Qué datos son maestros y dónde reside su fuente de verdad?
22. ¿Se requiere migración, retención, anonimización o eliminación?

## Seguridad y operación

23. ¿Cómo se autentican usuarios y servicios?
24. ¿Cómo se autoriza el acceso por rol, recurso o acción?
25. ¿Qué amenazas y abusos deben mitigarse desde el diseño?
26. ¿Qué logs, métricas y trazas permiten operar el producto?
27. ¿Qué objetivos de recuperación y continuidad existen?

## Decisiones

28. ¿Qué estilos arquitectónicos son candidatos y por qué?
29. ¿Qué decisiones requieren ADR?
30. ¿Qué riesgos necesitan un spike o prototipo?
31. ¿Qué complejidad puede diferirse después del MVP?
32. ¿Qué límites pueden verificarse automáticamente?

## Criterios de salida

- Drivers y atributos de calidad priorizados.
- Contexto, límites, datos e integraciones descritos.
- Estilo arquitectónico justificado proporcionalmente al MVP.
- Riesgos, spikes y ADRs identificados.
- Seguridad, observabilidad y recuperación contempladas.
- Restricciones verificables traducidas a controles.

