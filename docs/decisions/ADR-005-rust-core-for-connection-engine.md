# ADR-005-rust-core-for-connection-engine

## Estado
Aceptado

## Contexto
OmniTerminal requiere decisiones fundacionales para evitar deriva técnica y proteger la visión de plataforma enterprise desktop-native.

## Decisión
Rust como core de conexión para SSH/túneles/crypto por seguridad y performance determinista.

## Consecuencias
- Mejora coherencia entre equipos de producto, plataforma y seguridad.
- Define límites explícitos para MVP y escalamiento posterior.
- Reduce riesgo de sobreingeniería temprana.
