# AGENTS

## Reglas operacionales para agentes IA
1. No convertir OmniTerminal en una web app; mantener enfoque desktop-first.
2. No introducir Electron.
3. No mover ejecución de SSH/RDP/túneles al control plane.
4. Evitar overengineering: sin service mesh/CQRS/event bus complejo en fase inicial.
5. Toda propuesta debe incluir impacto en seguridad, licenciamiento y compliance.
6. Documentar decisiones relevantes en `docs/decisions/` mediante ADR.

## Convenciones
- Documentación en español, tono enterprise.
- Cada nuevo módulo debe declarar responsabilidades y límites en su README local.
