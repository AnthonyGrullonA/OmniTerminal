# Architecture Guardrails

## Boundaries obligatorios
- **Desktop App (Tauri/Rust)**: ejecución operacional, protocolos, vault local, session runtime.
- **Control Plane (DjangoBlaze)**: identidad, tenancy, licensing, billing, governance, sync metadata, auditoría.
- **AI Services (FastAPI)**: inferencia y asistencia operacional, sin estado crítico persistente en MVP.

## Anti-patrones prohibidos
- Microservicios por protocolo sin necesidad de escala real.
- Acoplar UI desktop a disponibilidad constante del cloud.
- Centralizar secretos de sesión activa en servicios remotos sin controls de minimización.

## Principios de evolución
- Modularidad por capacidades (connection, identity, policy, telemetry).
- Contratos explícitos en `packages/contracts`.
- Diseño plugin-first con control de permisos por plugin.
