# Agents

Plantillas APDF para desarrollar productos de software con agentes especializados, skills reutilizables, bancos de preguntas y documentación versionada.

## Versiones

- [Plantilla para Codex](codex-template/)
- [Plantilla para Claude Code](claude-template/)

## Copiar una plantilla a un proyecto nuevo

Copiar siempre el contenido completo de la plantilla elegida a la raíz del repositorio destino. Usar `/.` al final de la ruta origen para incluir archivos y carpetas ocultas como `.claude/` o `.codex/`.

Claude Code:

```bash
cp -R agents/claude-template/. mi-nuevo-proyecto/
```

Codex:

```bash
cp -R agents/codex-template/. mi-nuevo-proyecto/
```

En cada plantilla, los archivos raíz como `START-HERE.md`, `METHODOLOGY.md`, `CATALOG.md`, `AGENT-CONTRACT.md` y `QUESTION-FACILITATION.md` son guías de operación de la metodología. La carpeta `docs/` es para la documentación viva del producto que se irá llenando durante el proyecto.

## Documentación principal

- [Guía de inicio](START-HERE.md)
- [Metodología APDF](METHODOLOGY.md)
- [Catálogo de agentes, skills y paquetes](CATALOG.md)

Cada plantilla incluye diez roles, dieciocho skills, 230 preguntas base, dieciocho paquetes de dominio, paquetes técnicos y cuestionarios DOCX/XLSX.

El Requirements Facilitator y la skill `explain-discovery-question` pueden reformular preguntas, explicar su intención y proporcionar ejemplos sin responder en nombre del usuario.
