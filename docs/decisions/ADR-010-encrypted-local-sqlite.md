# ADR-010-encrypted-local-sqlite

## Estado
Aceptado

## Contexto
OmniTerminal requiere decisiones estructurales para escalar sin romper el MVP ni degradar seguridad.

## Decisión
Se adopta SQLite cifrado local en desktop para metadata operativa, cache segura y soporte offline.

## Consecuencias
- Alinea producto, arquitectura y seguridad.
- Reduce riesgo operativo y técnico.
- Mejora mantenibilidad y escalabilidad incremental.
