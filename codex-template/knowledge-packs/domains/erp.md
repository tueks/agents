# Domain Pack: ERP

## Triggers

Usar para productos que integran varios procesos empresariales y comparten datos maestros, contabilidad, inventario, compras, ventas, recursos o aprobaciones.

## Capacidades frecuentes

- Organizaciones, sucursales, periodos y monedas.
- Usuarios, roles, segregación de funciones y aprobaciones.
- Datos maestros y catálogos compartidos.
- Documentos con folios, estados y trazabilidad.
- Inventario, compras, ventas, cuentas y conciliación.
- Configuración por empresa y extensibilidad por módulos.
- Auditoría, cierres, correcciones y reversas.

## Preguntas adicionales

### Producto

- ¿Qué módulos componen el alcance y cuál es el proceso end-to-end prioritario?
- ¿Qué sistema es fuente de verdad para clientes, productos, precios y cuentas?
- ¿Se necesita multiempresa, multisucursal, multimoneda o consolidación?
- ¿Qué aprobaciones, cierres y segregación de funciones aplican?

### UX/UI

- ¿Qué usuarios realizan tareas repetitivas de alta densidad?
- ¿Qué vistas requieren tablas, filtros guardados, acciones masivas o exportación?

### Arquitectura y datos

- ¿Qué consistencia debe mantenerse entre módulos?
- ¿Qué procesos son transaccionales y cuáles pueden ser asíncronos?
- ¿Cómo se versionan reglas, impuestos, precios y configuraciones?

### QA y operación

- ¿Cómo se validan cierres, reversas, conciliación y auditoría?
- ¿Qué datos de prueba representan periodos y organizaciones diferentes?

## Riesgos

- Intentar incluir demasiados módulos en el MVP.
- Acoplar módulos mediante tablas compartidas sin propiedad clara.
- Confundir corrección con eliminación de documentos auditables.
- Permisos simples cuando se requiere segregación de funciones.

