---
name: review-question-bank
description: Audita y mejora bancos de preguntas de producto, UX/UI, arquitectura, backend, frontend, QA, plataforma o documentación. Usar cuando las preguntas son ambiguas, redundantes, demasiado técnicas, incompletas, están mal secuenciadas o se necesita adaptarlas a un dominio o perfil de usuario.
---

# Review Question Bank

1. Identificar banco, audiencia, etapa, artefacto de salida y paquetes de dominio aplicables.
2. Revisar cada pregunta con estos criterios:
   - propósito claro;
   - una sola decisión principal;
   - lenguaje apropiado al perfil;
   - respuesta accionable;
   - momento correcto del lifecycle;
   - obligatoriedad proporcional;
   - ausencia de duplicación;
   - cobertura de riesgos y excepciones.
3. Clasificar hallazgos: unclear, duplicate, leading, premature, missing-context, too-broad, too-narrow o missing-question.
4. Proponer para cada cambio:
   - redacción original;
   - problema;
   - nueva redacción;
   - motivo;
   - rol y momento recomendado;
   - required-now, required-before-close u optional.
5. Aplicar `QUESTION-FACILITATION.md` para añadir explicación, guía y ejemplo cuando la pregunta lo requiera.
6. Verificar que los criterios de salida puedan satisfacerse con el banco resultante.
7. Mantener IDs estables cuando una pregunta conserva su intención; crear nuevos IDs cuando cambia materialmente.
8. Entregar un changelog del banco y actualizar el cuestionario maestro cuando se aprueben cambios.

No aumentar el número de preguntas sin demostrar qué riesgo o decisión adicional cubren.

