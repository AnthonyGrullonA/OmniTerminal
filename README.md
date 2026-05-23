# OmniTerminal

OmniTerminal es una **AI-Native Operational Infrastructure Platform** orientada a operación enterprise crítica. Su tesis es unificar acceso remoto, gobierno de identidad, seguridad, observabilidad contextual y asistencia AI en una sola experiencia **desktop-native**.

## Visión enterprise
- Convertirse en la capa unificada de acceso operacional para bancos, telcos, fintechs, healthcare, gobierno y MSSPs.
- Reducir fragmentación entre herramientas de terminal, APIs, Kubernetes, bases de datos, VPN y PAM.
- Proveer un modelo Zero Trust operativo con trazabilidad auditable y control de riesgo.

## Arquitectura de referencia
- **Desktop App (principal):** runtime operativo, protocol engine, vault local, terminal, túneles y UX de operación.
- **Control Plane SaaS (DjangoBlaze):** identidad, organizaciones, suscripciones, billing, licencias, governance, sync metadata y administración enterprise.
- **AI Services (FastAPI):** copilotos operacionales, explicación de comandos y análisis contextual desacoplado.

## Stack oficial
- Desktop: Tauri, Rust, React, TypeScript, TailwindCSS, xterm.js, Zustand, TanStack Query, SQLite cifrado.
- Control Plane: DjangoBlaze Pro, Django 6, DRF, PostgreSQL, Redis, Celery, WebSockets.
- AI: FastAPI, Python, OpenRouter, Claude, GPT, Ollama.

## Diferenciadores
1. Unified workspace: SSH/RDP/APIs/DB/K8s/VPN en una sola superficie.
2. AI operational intelligence: sugerencias contextualizadas y accionables.
3. PAM readiness: RBAC/SSO/SAML/OIDC/SCIM/MFA/WebAuthn/JIT/policy-as-code.
4. Cloud-connected sin cloud dependency operacional.

## MVP real
### Desktop MVP
SSH, SFTP, tabs, workspaces, local encrypted vault, secure settings, tunnel manager, remote file explorer, snippets/macros, multi-execution, sync básico y licensing.

### SaaS MVP
Auth, organizations, teams, subscriptions, billing, licensing, device registration, seat management y sync metadata.

### AI MVP
AI chat, command explanation y operational assistant básico.

## Estrategia cloud y desktop
- **Desktop-first:** toda ejecución crítica de sesión permanece local para latencia y control.
- **Cloud-connected:** control plane gobierna identidad, licencias y políticas sin secuestrar runtime.
- **Offline-capable:** activación/validación de licencias con escenarios offline y air-gapped.

## Estrategia AI
- AI asiste decisiones; no reemplaza controles de autorización.
- Guardrails de seguridad, auditabilidad y minimización de datos por diseño.

## Estrategia PAM
- Preparación desde fase fundacional para SOC2/ISO27001/PCI DSS/GDPR.
- Diseño por políticas, aprobación contextual y credenciales efímeras.

## Estructura monorepo
Ver `MONOREPO_MAP.md`.

## Quick Start documental
1. `PROJECT_CONTEXT.md`
2. `ARCHITECTURE_GUARDRAILS.md`
3. `SECURITY_GUARDRAILS.md`
4. `BUILD_STRATEGY.md`
5. `docs/decisions/`
