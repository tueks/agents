# Domain Pack: Punto de venta

## Triggers

Usar para venta presencial, caja, pedidos, cobro, tickets, turnos, sucursales e inventario operativo.

## Capacidades frecuentes

- Apertura y cierre de caja o turno.
- Catálogo, modificadores, precios, promociones e impuestos.
- Carrito, pedido, cobro y ticket.
- Pagos divididos, propinas, descuentos, cancelaciones y devoluciones.
- Inventario por sucursal y movimientos.
- Operación sin conexión o conectividad intermitente.
- Dispositivos: impresora, escáner, cajón, terminal y pantalla de cocina.
- Arqueo, auditoría y conciliación.

## Preguntas adicionales

### Producto

- ¿Qué tipos de venta, pago, devolución y cancelación se permiten?
- ¿Qué sucede si el pago se procesa pero el sistema no confirma la venta?
- ¿Quién autoriza descuentos, cancelaciones y retiros?
- ¿Se requiere facturación fiscal o integración con proveedores de pago?

### UX/UI

- ¿Cuántos toques y cuánto tiempo son aceptables por venta?
- ¿Se operará con pantalla táctil, teclado, escáner o ambos?
- ¿Qué información debe ser visible durante horas pico?

### Arquitectura y backend

- ¿Cómo se generan folios y se conserva idempotencia?
- ¿Cómo se sincronizan ventas e inventario sin conexión?
- ¿Cómo se reconcilian respuestas tardías del proveedor de pagos?

### QA y plataforma

- Probar doble clic, reintentos, desconexiones y respuestas ambiguas.
- Probar apertura/cierre, diferencias de caja y reversas.
- Validar impresión, dispositivos y latencia en sitio.

## Riesgos

- Tratar una operación de pago como un CRUD simple.
- No diseñar idempotencia y reconciliación.
- Depender completamente de conexión estable.
- No conservar evidencia de operaciones anuladas.

