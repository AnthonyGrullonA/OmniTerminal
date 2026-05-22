# PROJECT_CONTEXT.md

> Documento de contexto para asistentes (Codex, Claude u otros agentes) y para onboarding técnico-rápido.

## Objetivo de este archivo

Este archivo funciona como **router de contexto**: indica qué documentos leer según el tipo de tarea, evitando respuestas superficiales y manteniendo coherencia con la visión de OmniTerminal.

## Identidad del producto (no negociable)

OmniTerminal es:

- **AI-Native Operational Access Platform**.
- **Unified Operational Access Layer for Modern Infrastructure**.

OmniTerminal no es:

- un emulador de terminal genérico,
- un cliente SSH aislado,
- una suite fragmentada sin gobierno enterprise.

## Reglas de contextualización para agentes

Antes de proponer cambios:

1. Identifica el dominio de la tarea.
2. Lee guardrails raíz obligatorios.
3. Lee documentos core de producto/arquitectura/seguridad.
4. Lee documentos especializados por trigger.
5. Prioriza seguridad, cumplimiento y gobernanza de acceso privilegiado.

## Lectura obligatoria (siempre)

1. `ARCHITECTURE_GUARDRAILS.md`
2. `SECURITY_GUARDRAILS.md`
3. `PRODUCT_GUARDRAILS.md`
4. `CURRENT_PHASE.md`
5. `BUILD_STRATEGY.md`
6. `MONOREPO_MAP.md`

## Documentos core de plataforma

1. `docs/vision/vision-document.md`
2. `docs/product/product-requirements-document.md`
3. `docs/architecture/system-architecture.md`
4. `docs/security/security-architecture.md`
5. `docs/compliance/compliance-strategy.md`
6. `docs/engineering/engineering-handbook.md`

## Triggers por tipo de tarea

### 1) Estrategia de producto / roadmap
Leer:
- `docs/product/roadmap.md`
- `docs/product/feature-matrix.md`
- `docs/product/workflows-and-use-cases.md`
- `docs/business/go-to-market-strategy.md`
- `docs/business/market-analysis.md`

### 2) Arquitectura de plataforma / boundaries
Leer:
- `ARCHITECTURE_GUARDRAILS.md`
- `docs/architecture/high-level-design.md`
- `docs/architecture/low-level-design.md`
- `docs/architecture/plugin-system-architecture.md`
- `docs/architecture/multi-tenancy-architecture.md`
- `docs/architecture/desktop-client-architecture.md`
- `docs/architecture/saas-control-plane-architecture.md`

### 3) Seguridad, PAM, identidad y políticas
Leer:
- `SECURITY_GUARDRAILS.md`
- `docs/security/zero-trust-model.md`
- `docs/security/pam-architecture.md`
- `docs/security/identity-and-access-management.md`
- `docs/security/rbac-permission-matrix.md`
- `docs/security/policy-as-code.md`

### 4) Compliance y regulación
Leer:
- `docs/compliance/soc2-readiness.md`
- `docs/compliance/iso27001-alignment.md`
- `docs/compliance/pci-dss-alignment.md`
- `docs/compliance/gdpr-strategy.md`
- `docs/compliance/data-retention-policy.md`

### 5) AI operational copilot
Leer:
- `apps/ai-services/README.md`
- `docs/ai/ai-architecture.md`
- `docs/ai/ai-copilot-functional-design.md`
- `docs/ai/session-intelligence.md`
- `docs/ai/ai-governance-policy.md`

### 6) Control plane / tenancy / licensing
Leer:
- `apps/control-plane/README.md`
- `docs/architecture/saas-control-plane-architecture.md`
- `docs/licensing/desktop-licensing-flow.md`
- `docs/licensing/offline-activation-and-validation.md`
- `docs/licensing/enterprise-license-server.md`

### 7) Desktop runtime / protocolos
Leer:
- `apps/desktop/README.md`
- `docs/product/functional-requirements-specification.md`
- `docs/architecture/desktop-client-architecture.md`
- `docs/integrations/kubernetes-integration.md`
- `docs/integrations/vpn-integration.md`

### 8) Decisiones fundacionales
Leer:
- `docs/decisions/ADR-001-use-tauri-over-electron.md`
- `docs/decisions/ADR-003-djangoblaze-as-control-plane.md`
- `docs/decisions/ADR-005-rust-core-for-connection-engine.md`
- `docs/decisions/ADR-008-plugin-first-architecture.md`

## Criterios de calidad esperados

Toda salida debe ser:

- En español.
- Enterprise-grade y accionable.
- Coherente con arquitectura modular/plugin-first.
- Alineada a Zero Trust y PAM moderno.
- Compatible con operación híbrida, offline y air-gapped.
- Libre de microservicios prematuros sin justificación de escala.
