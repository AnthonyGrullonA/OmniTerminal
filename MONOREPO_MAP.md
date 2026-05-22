# Monorepo Map

## Topología
- `apps/desktop`: cliente principal y runtime operacional.
- `apps/control-plane`: DjangoBlaze extendido como SaaS de gobierno.
- `apps/ai-services`: capa AI desacoplada.
- `packages/*`: contratos, SDKs, tipos y capacidades compartidas.
- `infrastructure/*`: assets de plataforma y despliegue.
- `docs/*`: documentación estratégica, técnica y ADRs.

## Flujos de relación
- Desktop consume contratos/tipos compartidos y sincroniza metadata con control plane.
- Control plane emite políticas/licencias y expone APIs para desktop/ai.
- AI services consumen metadata autorizada y devuelven recomendaciones contextualizadas.
