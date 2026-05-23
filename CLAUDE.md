# CLAUDE.md

## Contexto persistente
OmniTerminal prioriza un runtime desktop seguro, extensible y de baja latencia, gobernado por control plane SaaS y complementado por AI operational intelligence.

## Boundaries
- Desktop: protocolos, sesiones, vault local, túneles, ejecución multi-host.
- Control Plane: identidad, organizaciones, licencias, billing, policy governance.
- AI Services: copiloto y análisis operacional sin autoridad de ejecución autónoma.

## Prioridades
1. Entregar MVP desktop utilizable en operación real.
2. Licenciamiento robusto (online/offline/air-gapped).
3. Seguridad y cumplimiento by design.
4. Extensibilidad plugin-first sin sobre-abstracción.

## Restricciones técnicas
- No Electron.
- No mover runtime operativo al SaaS.
- No acoplar operación a conectividad cloud continua.
