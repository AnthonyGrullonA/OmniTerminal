# MONOREPO_MAP.md

## Árbol oficial
- `apps/desktop`
- `apps/control-plane`
- `apps/ai-services`
- `packages/sdk`
- `packages/contracts`
- `packages/shared-types`
- `packages/ui`
- `packages/security`
- `packages/observability`
- `packages/protocols`
- `packages/licensing`
- `packages/plugins`
- `infrastructure/docker`
- `infrastructure/terraform`
- `infrastructure/kubernetes`
- `infrastructure/ansible`
- `infrastructure/monitoring`
- `infrastructure/postgres`
- `infrastructure/redis`
- `infrastructure/scripts`
- `docs`
- `tools`
- `scripts`
- `.github`

## Contratos de relación
- Desktop consume `packages/*` y sincroniza con control-plane.
- Control-plane emite políticas/licencias y metadatos.
- AI consume contexto autorizado para análisis y recomendaciones.
