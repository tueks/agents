# Knowledge Pack: Documentación y plataformas

## Principio

Mantener en el repositorio las decisiones y especificaciones necesarias para construir, revisar y operar el producto. Usar una plataforma adicional cuando mejore colaboración, búsqueda o publicación para una audiencia concreta.

## Opciones

| Opción | Útil para | Consideración |
| --- | --- | --- |
| Markdown en repositorio | Ingeniería, versionado y trabajo de agentes | Requiere estructura e índices claros |
| MkDocs | Portal técnico ligero generado desde Markdown | Añade build y publicación |
| Docusaurus | Documentación de producto o desarrolladores con mayor personalización | Mayor mantenimiento frontend |
| GitHub/GitLab Wiki | Colaboración cercana al repositorio | Puede separar decisiones del mismo flujo de revisión |
| Confluence o Notion | Audiencias de negocio y edición colaborativa | Mantener enlaces estables y evitar fuentes de verdad duplicadas |
| Google Docs | Talleres, comentarios y aprobación narrativa | Consolidar decisiones finales en artefactos versionados |

## Regla de decisión

- Repositorio como fuente primaria para arquitectura, contratos, planes, runbooks y estado.
- Plataforma externa como vista publicada o espacio colaborativo cuando existe propietario.
- Registrar propietario, audiencia, fuente primaria y frecuencia de revisión.
- Si se duplica contenido, automatizar publicación o identificar explícitamente cuál copia es autoritativa.

