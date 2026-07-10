# Technical Pack: Seguridad transversal

## Aplicación

Usar cuando el producto maneja identidad, pagos, datos personales, información sensible, integraciones externas o acciones privilegiadas.

## Áreas

- Threat modeling proporcional al flujo y activos.
- Autenticación y gestión de sesión.
- Autorización por acción y recurso, con denegación por defecto.
- Validación de entrada y codificación de salida.
- Protección de datos en tránsito, reposo, logs y respaldos.
- Gestión de secretos y rotación.
- Auditoría de acciones sensibles.
- Dependencias, cadena de suministro y artefactos.
- Aislamiento, mínimo privilegio y superficie de red.
- Respuesta a incidentes y divulgación.

## Preguntas transversales

- ¿Qué activos y acciones serían más valiosos para un atacante?
- ¿Qué fronteras de confianza cruza el flujo?
- ¿Cómo se comprueba autorización en cada operación?
- ¿Qué datos no deben almacenarse o registrarse?
- ¿Qué abuso sigue siendo posible aunque el usuario esté autenticado?
- ¿Cómo se detecta, contiene y audita un incidente?

## Controles

Convertir controles deterministas en análisis estático, pruebas de autorización, escaneo de dependencias/secretos, políticas de infraestructura y gates de CI. Mantener revisión humana para riesgos de negocio y amenazas contextuales.

