# ADR-011-protocol-abstraction-layer

## Estado
Aceptado

## Contexto
OmniTerminal requiere decisiones estructurales para escalar sin romper el MVP ni degradar seguridad.

## Decisión
Se adopta una Protocol Abstraction Layer modular para desacoplar providers/protocolos y habilitar extensibilidad plugin-first.

## Consecuencias
- Alinea producto, arquitectura y seguridad.
- Reduce riesgo operativo y técnico.
- Mejora mantenibilidad y escalabilidad incremental.
