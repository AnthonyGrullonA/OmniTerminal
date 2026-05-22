# Control Plane

SaaS Control Plane basado en DjangoBlaze Pro.

## Responsabilidades
- Auth, organizaciones, equipos y RBAC.
- Licencias, suscripciones, seats y device registration.
- Sync metadata, gobierno y auditoría administrativa.

## Límites
- No ejecutar motores de SSH/RDP ni runtime de sesión.
- No renderizar terminal ni manejar túneles operativos.

## Stack
Django 6, DRF, PostgreSQL, Redis, Celery, WebSockets.

## Integración DjangoBlaze
Se adopta DjangoBlaze como base y se extiende por apps de dominio (licensing, governance, device trust) manteniendo convenciones del framework.

## Roadmap
MVP tenancy/licensing → políticas avanzadas → portal enterprise de cumplimiento.