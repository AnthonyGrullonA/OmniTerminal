# OmniTerminal Monorepo

OmniTerminal es una **Unified Operational Access Layer** desktop-native para operación enterprise con seguridad Zero Trust y capacidades AI-native.

## Propósito
- Centralizar en un solo monorepo el producto desktop, control plane SaaS y servicios AI.
- Mantener coherencia arquitectónica evitando sobreingeniería temprana.

## Arquitectura macro
- **apps/desktop**: runtime operacional en Tauri/Rust + React/TypeScript.
- **apps/control-plane**: DjangoBlaze Pro como plano de gobierno SaaS (auth, orgs, licencias, billing, sync metadata).
- **apps/ai-services**: FastAPI para inteligencia operacional desacoplada y stateless.

## Límites no negociables
1. Desktop-first: la ejecución operacional ocurre en cliente nativo.
2. Cloud-connected, no cloud-dependent: soporte offline/air-gapped.
3. Rust concentra engine de conexión y seguridad local.
4. No Electron.

## Mapa rápido
Ver `MONOREPO_MAP.md` para topología completa y `PROJECT_CONTEXT.md` para ruteo de lectura por tarea.

## Roadmap de inicialización
1. Definir contratos compartidos en `packages/contracts`.
2. Inicializar shell desktop y módulos SSH/SFTP MVP.
3. Integrar DjangoBlaze en `apps/control-plane` con extensiones mínimas.
4. Publicar API de AI assistant básico.
