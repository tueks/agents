---
name: conduct-role-interview
description: Realiza una entrevista adaptativa para cerrar el alcance de un rol de producto, UX/UI, arquitectura, backend, frontend, QA, plataforma o documentación. Usar cuando faltan decisiones o se necesita validar si un área está suficientemente definida.
---

# Conduct Role Interview

1. Identificar rol, objetivo, versión y artefacto de salida.
2. Leer el banco correspondiente en `question-banks/` y las respuestas ya documentadas.
3. Seleccionar preguntas por riesgo y dependencia, no en el orden del archivo.
4. Preguntar de 1 a 5 elementos relacionados por turno.
5. Si el usuario no comprende una pregunta, invocar `explain-discovery-question` antes de continuar.
6. Permitir que el usuario solicite reformulación, ejemplo, opciones o una estructura de respuesta.
7. Marcar respuestas como confirmed, assumed, unknown o conflicting.
8. Resumir la interpretación y pedir confirmación cuando una respuesta sea ambigua o de alto impacto.
9. Si hay más de 12 preguntas relevantes o el usuario desea responder después, invocar `create-guided-questionnaire`.
10. Detener la entrevista cuando se satisfagan los criterios de salida.
11. Entregar resumen de decisiones, huecos y siguiente acción.

No repetir preguntas resueltas ni exigir respuestas opcionales para cerrar una fase.
