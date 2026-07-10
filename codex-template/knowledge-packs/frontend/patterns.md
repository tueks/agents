# Technical Pack: Frontend

## Áreas de decisión

- Renderizado: SPA, SSR, SSG, híbrido o aplicación de escritorio/móvil.
- Organización: feature-based, route-based o capas por responsabilidad.
- Estado: local, URL, server state, shared client state y persisted state.
- Componentes: primitives, design system, feature components y page composition.
- Integración: clientes tipados, caché, invalidación, optimistic updates y errores.
- Calidad: accesibilidad, pruebas de componentes, integración y E2E.

## Patrones

- Presentational/container solo cuando separa responsabilidades reales.
- State machine para flujos con estados y transiciones complejas.
- Server-state library para caché remota; no duplicar datos remotos en stores globales.
- Adapter/anti-corruption layer para contratos externos inestables.
- Design tokens y componentes accesibles para coherencia visual.
- Progressive enhancement cuando resiliencia y accesibilidad lo justifican.

## Preguntas de selección

- ¿Qué debe indexarse o renderizarse antes de ejecutar JavaScript?
- ¿Qué estado debe sobrevivir navegación o recarga?
- ¿Qué comportamiento es compartido entre plataformas?
- ¿Qué presupuesto de rendimiento y accesibilidad existe?
- ¿Cómo se evita que el frontend dependa de detalles internos del backend?

