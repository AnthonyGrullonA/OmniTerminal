# PROJECT_CONTEXT.md

> Documento de contexto para asistentes (Codex, Claude u otros agentes) y para onboarding técnico-rápido.

## Objetivo de este archivo

Este archivo funciona como **router de contexto**: indica qué documentos leer según el tipo de tarea, para evitar respuestas superficiales y alinear cualquier contribución con la visión de OmniTerminal.

---

## Identidad del producto (no negociable)

OmniTerminal es una:

- **AI-Native Operational Access Platform**
- **Unified Operational Access Layer for Modern Infrastructure**

No es:

- un emulador de terminal “bonito”
- un cliente SSH aislado
- una herramienta puntual de APIs o Kubernetes

La plataforma debe integrar acceso, identidad, seguridad, observabilidad, PAM, auditoría, colaboración y copiloto AI en un workspace unificado.

---

## Reglas de contextualización para agentes

Antes de proponer cambios:

1. Identifica el dominio de la tarea.
2. Lee primero los documentos “core”.
3. Lee luego los documentos “especializados” del dominio.
4. Mantén consistencia con enfoque **desktop-first**, **Zero Trust**, **AI-native** y **enterprise/PAM**.

---

## Documentos core (leer siempre)

1. `docs/vision/vision-document.md`
2. `docs/vision/executive-summary.md`
3. `docs/product/product-requirements-document.md`
4. `docs/architecture/system-architecture.md`
5. `docs/security/security-architecture.md`
6. `docs/compliance/compliance-strategy.md`
7. `docs/engineering/engineering-handbook.md`

---

## Triggers por tipo de tarea

### 1) Estrategia de producto o roadmap
**Trigger:** “roadmap”, “priorización”, “módulos”, “go-to-market técnico”.

Leer:
- `docs/product/roadmap.md`
- `docs/product/feature-matrix.md`
- `docs/product/workflows-and-use-cases.md`
- `docs/business/go-to-market-strategy.md`
- `docs/business/market-analysis.md`

### 2) Arquitectura de plataforma
**Trigger:** “arquitectura”, “HLD”, “LLD”, “multi-tenant”, “plugin”.

Leer:
- `docs/architecture/high-level-design.md`
- `docs/architecture/low-level-design.md`
- `docs/architecture/plugin-system-architecture.md`
- `docs/architecture/multi-tenancy-architecture.md`
- `docs/architecture/desktop-client-architecture.md`
- `docs/architecture/saas-control-plane-architecture.md`

### 3) Seguridad, PAM, identidad y políticas
**Trigger:** “RBAC”, “SSO”, “PAM”, “JIT”, “vault”, “policy-as-code”, “audit”.

Leer:
- `docs/security/zero-trust-model.md`
- `docs/security/pam-architecture.md`
- `docs/security/identity-and-access-management.md`
- `docs/security/rbac-permission-matrix.md`
- `docs/security/policy-as-code.md`
- `docs/security/session-recording-and-audit.md`

### 4) Compliance y regulación
**Trigger:** “SOC2”, “ISO27001”, “PCI-DSS”, “GDPR”, “retención”.

Leer:
- `docs/compliance/soc2-readiness.md`
- `docs/compliance/iso27001-alignment.md`
- `docs/compliance/pci-dss-alignment.md`
- `docs/compliance/gdpr-strategy.md`
- `docs/compliance/data-retention-policy.md`
- `docs/compliance/incident-response-plan.md`

### 5) IA operacional y session intelligence
**Trigger:** “copilot”, “análisis de comandos”, “riesgo AI”, “knowledge graph”.

Leer:
- `docs/ai/ai-architecture.md`
- `docs/ai/ai-copilot-functional-design.md`
- `docs/ai/session-intelligence.md`
- `docs/ai/operational-knowledge-graph.md`
- `docs/ai/ai-governance-policy.md`
- `docs/ai/ai-risk-analysis.md`

### 6) Integraciones técnicas
**Trigger:** “Kubernetes”, “VPN”, “SIEM”, “observabilidad”, “DB”, “API”.

Leer:
- `docs/integrations/kubernetes-integration.md`
- `docs/integrations/vpn-integration.md`
- `docs/integrations/observability-integrations.md`
- `docs/integrations/siem-integrations.md`
- `docs/integrations/database-integrations.md`
- `docs/integrations/api-integrations.md`
- `docs/integrations/enterprise-identity-integrations.md`

### 7) Licenciamiento enterprise y air-gapped
**Trigger:** “offline activation”, “license server”, “floating license”, “air-gapped”.

Leer:
- `docs/licensing/desktop-licensing-flow.md`
- `docs/licensing/offline-activation-and-validation.md`
- `docs/licensing/enterprise-license-server.md`
- `docs/licensing/floating-license-model.md`
- `docs/licensing/air-gapped-licensing.md`

### 8) Despliegue y resiliencia
**Trigger:** “on-prem”, “DR”, “backup”, “escalabilidad”, “performance”.

Leer:
- `docs/deployment/on-premise-deployment.md`
- `docs/deployment/air-gapped-deployment.md`
- `docs/deployment/cloud-deployment.md`
- `docs/deployment/disaster-recovery-plan.md`
- `docs/deployment/backup-and-recovery.md`
- `docs/deployment/scalability-and-performance.md`

### 9) Ejecución de ingeniería y entrega
**Trigger:** “CI/CD”, “branching”, “QA”, “estándares”, “ADR”.

Leer:
- `docs/engineering/coding-standards.md`
- `docs/engineering/branching-strategy.md`
- `docs/engineering/release-strategy.md`
- `docs/engineering/ci-cd-architecture.md`
- `docs/engineering/qa-and-testing-strategy.md`
- `docs/engineering/adr-index.md`

### 10) Operación, soporte y éxito de cliente
**Trigger:** “runbooks”, “SLA”, “onboarding enterprise”, “MSSP”.

Leer:
- `docs/operations/operational-runbooks.md`
- `docs/operations/support-and-sla.md`
- `docs/operations/enterprise-onboarding.md`
- `docs/operations/mssp-strategy.md`
- `docs/operations/customer-success-playbook.md`

---

## Criterios de calidad esperados para cualquier propuesta

Toda salida debe ser:

- En español.
- Enterprise-grade y accionable.
- Coherente con arquitectura modular/plugin-based.
- Alineada a Zero Trust y PAM moderno.
- Compatible con operación híbrida, offline y air-gapped.
- Trazable en seguridad, auditoría y cumplimiento.

Si hay conflicto entre propuestas, priorizar siempre seguridad, cumplimiento y gobernanza de acceso privilegiado.
