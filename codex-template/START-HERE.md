# Plantilla APDF para desarrollo de productos con agentes

Esta entrega contiene dos plantillas equivalentes:

- `codex-template/`: configuración nativa para Codex.
- `claude-template/`: configuración nativa para Claude Code.

Ambas incluyen la misma metodología, skills, bancos de preguntas, paquetes de conocimiento, documentos iniciales y plantillas de cuestionario. Solo cambia la definición de los agentes y la ubicación nativa de las skills.

## Cómo comenzar un proyecto

1. Copiar el contenido completo de esta plantilla a la raíz de un repositorio nuevo o existente.
2. Iniciar Codex o Claude Code en la raíz.
3. Solicitar: `Inicia el proyecto usando orchestrate-product-development`.
4. Responder el perfil de comunicación.
5. Completar la entrevista de Product Owner o solicitar cuestionario DOCX/XLSX.
6. Aprobar explícitamente el alcance del MVP antes de pasar a diseño y arquitectura.

Para copiar esta plantilla de Codex:

```bash
cp -R agents/codex-template/. mi-nuevo-proyecto/
```

El punto final en `codex-template/.` es intencional: copia también carpetas ocultas como `.codex/`.

## Cómo queda el repositorio destino

```text
mi-nuevo-proyecto/
├── AGENTS.md
├── START-HERE.md
├── METHODOLOGY.md
├── CATALOG.md
├── AGENT-CONTRACT.md
├── QUESTION-FACILITATION.md
├── .codex/
│   └── agents/
├── .agents/
│   └── skills/
├── docs/
├── knowledge-packs/
└── question-banks/
```

Los archivos raíz son guías de operación de la metodología y de los agentes. La carpeta `docs/` contiene la documentación viva del producto: alcance, arquitectura, UX, QA, operaciones, versiones y estado.

Si una pregunta no se entiende, solicitar que se reformule, explique, ejemplifique o estructure. El orquestador puede usar `explain-discovery-question` o delegar al Requirements Facilitator.

## Extender el catálogo

- Nuevo procedimiento reutilizable: crear una skill.
- Nuevo especialista con contexto o permisos propios: crear un agente.
- Nueva familia de producto, patrón o lenguaje: crear un knowledge pack.
- Nueva decisión importante: crear un ADR.
- Nueva versión: copiar `docs/templates/version-specification.md`.

## Importante

Los paquetes de ERP, POS, catálogo y CRUD son ayudas de descubrimiento. No convierten sus capacidades comunes en requisitos automáticos.
