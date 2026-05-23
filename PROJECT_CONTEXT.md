# PROJECT_CONTEXT.md

## Source of Truth Central
Este documento es la referencia principal para agentes y equipos sobre alcance, límites, prioridades y rutas de lectura.

## Identidad no negociable
OmniTerminal es una Unified Operational Access Platform desktop-first con arquitectura modular, AI-native, Zero Trust y foco enterprise/PAM.

## Guardrails obligatorios
1. Desktop runtime local para sesiones/protocolos/túneles.
2. DjangoBlaze solo control plane (auth, billing, licensing, governance, sync).
3. AI desacoplada, inicialmente stateless y con trazabilidad.
4. Sin microservicios complejos tempranos ni service mesh/CQRS/event sourcing.

## Orden de lectura mínima
- `README.md`
- `ARCHITECTURE_GUARDRAILS.md`
- `SECURITY_GUARDRAILS.md`
- `PRODUCT_GUARDRAILS.md`
- `BUILD_STRATEGY.md`
- `CURRENT_PHASE.md`
- `MONOREPO_MAP.md`

## Triggers de trabajo
- Arquitectura: `docs/architecture/*` + `docs/decisions/*`.
- Desktop: `apps/desktop/README.md` + `packages/protocols/README.md`.
- Control Plane: `apps/control-plane/README.md` + `packages/licensing/README.md`.
- AI: `apps/ai-services/README.md` + `docs/ai/*`.
- Seguridad/compliance: `docs/security/*`, `docs/compliance/*`, `SECURITY_GUARDRAILS.md`.

## Criterios de aceptación
- Español, enterprise-grade, accionable y auditable.
- Coherencia de boundaries.
- Evolución incremental con máxima velocidad sostenible.
