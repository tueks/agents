---
name: create-guided-questionnaire
description: Genera cuestionarios guiados en DOCX, XLSX o Markdown cuando delimitar un producto o un rol requiere muchas preguntas, varios participantes, inventarios o respuesta diferida. Usar cuando una entrevista supera 12 preguntas relevantes o el usuario pide un archivo para llenar con calma.
---

# Create Guided Questionnaire

1. Reunir solo preguntas relevantes no respondidas del banco del rol.
2. Para cada pregunta incluir: ID, sección, pregunta, motivo, obligatoriedad, guía, ejemplo, responsable sugerido y respuesta.
3. Incluir portada o introducción con propósito, versión, fecha y método de devolución.
4. Incluir instrucciones:
   - usar `Desconocido` si no se conoce la respuesta;
   - usar `No aplica` con justificación;
   - identificar supuestos;
   - no borrar IDs;
   - adjuntar evidencia mediante enlaces o referencias.
5. Elegir formato:
   - DOCX para respuestas narrativas y aprobación;
   - XLSX para inventarios, priorización o múltiples responsables;
   - ambos cuando convivan narrativa y tablas.
6. Usar los assets `questionnaire-template.docx` y `questionnaire-template.xlsx` si están disponibles.
7. Verificar visualmente el archivo generado y asegurar que no haya texto cortado.
8. Al recibirlo completado, validar respuestas y preguntar solo contradicciones o bloqueos.

