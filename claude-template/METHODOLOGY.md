# Agentic Product Development Framework (APDF)

## Estado y propósito

APDF es una metodología propuesta para desarrollar productos de software con agentes de IA. No pretende ser un estándar oficial. Integra prácticas existentes para cubrir descubrimiento, definición del MVP, evolución por versiones, diseño, arquitectura, desarrollo, calidad, documentación y entrega.

Sus fundamentos son:

1. **Product discovery y entrega iterativa:** validar primero el problema, el usuario y el alcance mínimo.
2. **Spec-Driven Development:** convertir intención en especificación, plan, tareas, implementación y aceptación.
3. **Docs as Code:** mantener conocimiento, decisiones y estado dentro del proyecto y bajo control de versiones.
4. **Harness engineering:** combinar instrucciones con verificaciones deterministas y ciclos de autocorrección.
5. **DevSecOps y calidad continua:** probar seguridad, calidad y desplegabilidad durante todo el ciclo.

## Modelo de composición

APDF separa seis conceptos:

| Concepto | Pregunta que responde | Ejemplo |
| --- | --- | --- |
| Agente | ¿Quién realiza o revisa el trabajo? | Product Owner, Arquitecto, QA |
| Skill | ¿Qué procedimiento completo debe seguir? | Definir MVP, escribir ADR, preparar release |
| Banco de preguntas | ¿Qué debe conocer el rol para cerrar su alcance? | Preguntas de arquitectura o UX |
| Paquete de dominio | ¿Qué particularidades tiene el tipo de producto? | ERP, POS, catálogo web, CRUD |
| Paquete técnico | ¿Qué conocimientos técnicos complementan el rol? | Hexagonal, CQRS, .NET, React |
| Artefacto | ¿Dónde queda registrada la decisión o resultado? | Product brief, ADR, guía UX, plan QA |

### Regla de diseño

- Crear un **agente** cuando se necesite contexto separado, revisión independiente, permisos distintos o trabajo paralelo.
- Crear una **skill** cuando exista un procedimiento reutilizable con entrada, pasos, validación y salida.
- Crear un **paquete de conocimiento** cuando solo cambie el conocimiento aplicado, pero no el procedimiento.
- Crear una **verificación automática** cuando una regla pueda evaluarse determinísticamente.

No crear una skill por cada patrón o lenguaje. Utilizar una skill de selección y aplicar uno o varios paquetes técnicos. Convertir un paquete en skill independiente únicamente cuando introduzca un workflow diferente.

## Roles

| Rol | Responsabilidad principal | Artefactos principales |
| --- | --- | --- |
| Product Development Orchestrator | Interactuar con el usuario, adaptar la comunicación y coordinar el ciclo | Estado, decisiones y handoffs |
| Product Owner | Definir problema, usuarios, valor, MVP, roadmap y aceptación | Product brief, MVP scope, version brief |
| UX/UI Designer | Diseñar experiencia, flujos, interfaz y guía visual | UX brief, user flows, UI guidelines |
| Software Architect | Definir atributos de calidad, límites y decisiones significativas | Architecture overview, ADRs |
| Backend Engineer | Diseñar e implementar dominio, API, datos e integraciones | Backend design y contratos |
| Frontend Engineer | Diseñar e implementar interfaz, estado e integración | Frontend design y componentes |
| Platform Engineer | Diseñar ambientes, CI/CD, observabilidad y operación | Deployment plan y runbooks |
| QA Engineer | Diseñar pruebas, trazabilidad, regresión y release gate | Test strategy y quality report |
| Project Documentarian | Mantener una visión ligera y coherente del producto | Product overview y documentación indexada |
| Requirements Facilitator | Traducir preguntas, facilitar respuestas y revisar claridad | Explicaciones, guías y mejoras de bancos |

## Perfil de comunicación

El orquestador mantiene un perfil configurable:

- `knowledge_level`: novice, intermediate, advanced, expert.
- `perspective`: business, technical, mixed.
- `detail_level`: executive, standard, detailed.
- `decision_style`: recommendation-first, alternatives-first.
- `language`: idioma preferido.

Si el perfil no existe, debe preguntarlo antes de una explicación compleja. No debe confundir el nivel técnico general con el conocimiento de un dominio concreto.

## Ciclo del MVP

1. **Intake:** registrar idea, perfil de comunicación y restricciones conocidas.
2. **Discovery:** entender problema, usuarios, contexto, valor y riesgos.
3. **MVP framing:** definir resultados, alcance incluido, exclusiones y señales de validación.
4. **Experience definition:** definir journeys, flujos, contenido y guía visual mínima.
5. **Architecture framing:** definir atributos de calidad, límites, datos, integraciones y ADRs iniciales.
6. **Delivery planning:** dividir el MVP en incrementos verificables y priorizados.
7. **Implementation:** backend, frontend e infraestructura ejecutan las especificaciones aprobadas.
8. **Continuous quality:** QA participa desde criterios de aceptación hasta regresión.
9. **Release readiness:** comprobar funcionalidad, seguridad, operación, observabilidad y rollback.
10. **Learning:** registrar resultados, feedback y cambios candidatos para la siguiente versión.

## Ciclo de evolución por versión

Toda versión posterior comienza con uno o varios cambios deseados:

1. Registrar change request.
2. Clasificarlo: feature, enhancement, defect, technical, security, infrastructure o debt.
3. Analizar valor, impacto UX, arquitectura, backend, frontend, datos, calidad y operación.
4. Definir alcance de versión y exclusiones.
5. Actualizar especificaciones y criterios de aceptación.
6. Implementar en incrementos pequeños.
7. Ejecutar regresión y release gate.
8. Publicar, observar y actualizar el estado.

Un cambio menor puede omitir fases no afectadas, pero debe dejar evidencia de por qué no aplican.

## Política de entrevistas y cuestionarios

Cada rol posee un banco de preguntas y criterios de salida. El agente debe:

1. Reutilizar respuestas existentes y no preguntar lo ya documentado.
2. Preguntar primero solo lo bloqueante.
3. Realizar entrevistas en grupos de 1 a 5 preguntas relacionadas.
4. Explicar por qué una pregunta es importante cuando no sea evidente.
5. Distinguir `required-now`, `required-before-build` y `optional`.
6. Detectar contradicciones y presentar la decisión pendiente.
7. Cerrar la entrevista cuando se satisfagan los criterios de salida, no cuando se agote el banco.

Cuando el usuario no comprenda una pregunta, el orquestador o Requirements Facilitator debe reformularla, explicar qué decisión informa, mostrar cómo responder y proporcionar un ejemplo ficticio. La explicación nunca se registra como respuesta del usuario.

Generar un cuestionario guiado cuando ocurra cualquiera de estas condiciones:

- haya más de 12 preguntas relevantes;
- el usuario solicite responder después;
- se necesite consultar a varias personas;
- las respuestas requieran tablas, inventarios o priorización;
- se necesite evidencia o aprobación formal.

Formatos:

- DOCX para respuestas narrativas, discusión y aprobación.
- XLSX para inventarios, listas, priorización, responsables o respuestas de varios participantes.
- Markdown para trabajo directo dentro del repositorio.

Todo cuestionario debe incluir propósito, instrucciones, ejemplo de respuesta, obligatoriedad, responsable sugerido y guía para preguntas desconocidas.

## Documentación mínima

La documentación es progresiva. El MVP no requiere una enciclopedia.

- `docs/product/product-overview.md`: visión transversal del producto.
- `docs/product/mvp-scope.md`: alcance del MVP.
- `docs/product/roadmap.md`: evolución prevista sin comprometer fechas no aprobadas.
- `docs/versions/<version>/`: especificación, criterios, impacto y release.
- `docs/ux/`: flujos y guía UX/UI.
- `docs/architecture/`: visión y ADRs.
- `docs/engineering/`: contratos y diseños técnicos necesarios.
- `docs/quality/`: estrategia, trazabilidad y resultados.
- `docs/operations/`: despliegue, observabilidad y runbooks.
- `docs/status/product-status.md`: estado operativo y siguiente decisión.

El Project Documentarian mantiene índices, coherencia, enlaces y resumen. No sustituye a los especialistas como propietarios del contenido técnico.

## Definition of Ready

Un incremento está listo para planificarse cuando contiene:

- problema u oportunidad;
- usuario o actor afectado;
- resultado esperado;
- alcance y exclusiones;
- criterios de aceptación verificables;
- dependencias y restricciones conocidas;
- decisiones pendientes explícitas;
- riesgos proporcionales al cambio.

## Definition of Done

Un incremento está terminado cuando:

- cumple los criterios de aceptación;
- compila y pasa verificaciones aplicables;
- incluye pruebas proporcionales al riesgo;
- no viola límites arquitectónicos;
- actualiza contratos y documentación afectados;
- puede desplegarse y revertirse de forma conocida;
- registra limitaciones y trabajo diferido;
- QA emite un resultado de release gate.

## Gobernanza de los paquetes de conocimiento

Cada paquete debe declarar:

- propósito y triggers;
- supuestos;
- capacidades frecuentes;
- riesgos y preguntas adicionales;
- decisiones típicas;
- artefactos afectados;
- fuentes o versiones cuando sean relevantes.

Los paquetes no toman decisiones automáticamente. Aportan criterios al rol que sigue siendo responsable de contrastarlos con el producto real.

## Fuentes metodológicas

- OpenAI, Harness engineering: https://openai.com/index/harness-engineering/
- Anthropic, Building effective agents: https://www.anthropic.com/engineering/building-effective-agents
- Anthropic, Effective harnesses for long-running agents: https://www.anthropic.com/engineering/effective-harnesses-for-long-running-agents
- GitHub Spec Kit: https://github.com/github/spec-kit
- AWS, Architectural Decision Records: https://docs.aws.amazon.com/prescriptive-guidance/latest/architectural-decision-records/adr-process.html
- DORA, Continuous delivery: https://dora.dev/capabilities/continuous-delivery/
- DORA, Test automation: https://dora.dev/capabilities/test-automation/
