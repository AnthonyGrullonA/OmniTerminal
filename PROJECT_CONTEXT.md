# PROJECT_CONTEXT

## Objetivo
Router de contexto para agentes IA (Codex/Claude) y equipos técnicos. Define qué leer según tarea y qué límites respetar.

## Lectura obligatoria
1. `ARCHITECTURE_GUARDRAILS.md`
2. `SECURITY_GUARDRAILS.md`
3. `PRODUCT_GUARDRAILS.md`
4. `CURRENT_PHASE.md`
5. `BUILD_STRATEGY.md`

## Triggers por dominio
- **Desktop runtime / protocolos** → `apps/desktop/README.md`, `docs/product/functional-requirements-specification.md`, `docs/architecture/desktop-client-architecture.md`.
- **Control plane / tenancy / licensing** → `apps/control-plane/README.md`, `docs/architecture/saas-control-plane-architecture.md`, `docs/licensing/*.md`.
- **AI operational copilot** → `apps/ai-services/README.md`, `docs/ai/*.md`.
- **Seguridad/compliance** → `docs/security/*.md`, `docs/compliance/*.md`.
- **Decisiones de arquitectura** → `docs/decisions/*.md`.

## Criterio de calidad
Toda propuesta debe ser en español, enterprise-grade, sin microservicios prematuros y con foco en MVP real: SSH/SFTP/workspaces/licensing/sync básico.
