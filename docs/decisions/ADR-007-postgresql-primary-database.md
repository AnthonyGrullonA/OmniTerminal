# ADR-007-postgresql-primary-database

## Estado
Aceptado

## Contexto
OmniTerminal requiere decisiones fundacionales para evitar deriva técnica y proteger la visión de plataforma enterprise desktop-native.

## Decisión
PostgreSQL como base primaria del control plane por madurez transaccional, ecosistema y cumplimiento enterprise.

## Consecuencias
- Mejora coherencia entre equipos de producto, plataforma y seguridad.
- Define límites explícitos para MVP y escalamiento posterior.
- Reduce riesgo de sobreingeniería temprana.
