# Control Plane

## DjangoBlaze integration
DjangoBlaze Pro se usa como base y se extiende por dominios: organizations, subscriptions, licensing, governance, audit metadata y administration.

## Capacidades
- Auth, SSO/MFA base y gestión de organizaciones/equipos.
- Billing, subscriptions, seats y lifecycle de licencias.
- Device registration y postura básica de confianza.
- Sync metadata para desktop.

## Límites
No ejecuta SSH/RDP/túneles ni rendering de terminal. No centraliza secretos operativos de sesiones activas.

## Estrategia de evolución
Extensión incremental, sin romper convenciones DjangoBlaze, con apps de dominio bien delimitadas.
