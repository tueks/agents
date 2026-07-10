# Domain Pack: Aplicación CRUD de negocio

## Triggers

Usar para sistemas internos centrados en altas, consultas, cambios, bajas lógicas, estados y reportes operativos.

## Capacidades frecuentes

- Listado, detalle, creación y edición.
- Validación, duplicados y reglas condicionales.
- Estados, transiciones y permisos.
- Búsqueda, filtros, ordenamiento, exportación e importación.
- Auditoría, baja lógica e historial.
- Adjuntos, comentarios y notificaciones opcionales.

## Preguntas adicionales

- ¿Qué registros representan conceptos maestros y cuáles transacciones?
- ¿Qué campos son obligatorios, derivados, únicos o sensibles?
- ¿Quién puede crear, ver, editar, aprobar o desactivar?
- ¿Qué transiciones son válidas y cuáles requieren aprobación?
- ¿Se permite eliminar o solo desactivar?
- ¿Qué volumen, filtros y exportaciones se necesitan?
- ¿Qué cambios requieren auditoría completa?

## Riesgos

- Implementar pantallas antes de modelar reglas y estados.
- Usar permisos únicamente por pantalla y no por acción o recurso.
- Eliminar datos que deben conservar historial.
- Crear un framework genérico antes de validar el primer flujo real.

