# ADR-003-djangoblaze-as-control-plane

## Estado
Aceptado

## Contexto
OmniTerminal requiere decisiones fundacionales para evitar deriva técnica y proteger la visión de plataforma enterprise desktop-native.

## Decisión
DjangoBlaze se adopta como base del control plane SaaS para acelerar auth/tenancy/subscriptions sin invadir runtime operacional.

## Consecuencias
- Mejora coherencia entre equipos de producto, plataforma y seguridad.
- Define límites explícitos para MVP y escalamiento posterior.
- Reduce riesgo de sobreingeniería temprana.
