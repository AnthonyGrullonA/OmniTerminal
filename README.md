# OmniTerminal Monorepo

OmniTerminal es una **AI-Native Operational Access Platform** y **Unified Operational Access Layer** con enfoque **desktop-first** para operación de infraestructura crítica enterprise.

## Propuesta de valor

OmniTerminal unifica en una sola plataforma:

- Acceso operacional remoto (SSH, SFTP, SCP, RDP, VNC, túneles, serial).
- Integraciones API y datos (REST, GraphQL, gRPC, WebSockets, SOAP, MQTT; DBs principales).
- Operación cloud-native (Kubernetes, contenedores y proveedores cloud).
- Gobierno de identidad, PAM moderno, auditoría y licenciamiento enterprise.
- Copiloto operacional con inteligencia de sesión y análisis contextual.

## Propósito del monorepo

- Centralizar Desktop, Control Plane y AI Services bajo guardrails comunes.
- Reducir deriva arquitectónica y evitar sobreingeniería temprana.
- Acelerar entrega de MVP real con límites claros por dominio.

## Arquitectura macro

- **apps/desktop**: runtime operacional en Tauri/Rust + React/TypeScript.
- **apps/control-plane**: DjangoBlaze Pro como plano de gobierno SaaS (auth, orgs, suscripciones, licencias, billing, sync metadata, auditoría administrativa).
- **apps/ai-services**: FastAPI para inteligencia operacional desacoplada y stateless en fase inicial.

## Límites no negociables

1. **Desktop-first**: ejecución operacional en cliente nativo.
2. **Cloud-connected, no cloud-dependent**: soporte offline/air-gapped.
3. **Rust core** para engine de conexión y seguridad local.
4. **No Electron** como núcleo de producto.
5. **DjangoBlaze no ejecuta runtime SSH/RDP/túneles**.

## Estructura principal

- `apps/`
- `packages/`
- `infrastructure/`
- `docs/`
- `tools/`
- `.github/`
- `scripts/`

## Punto de entrada recomendado

1. `PROJECT_CONTEXT.md` (router de lectura por tarea).
2. `ARCHITECTURE_GUARDRAILS.md`.
3. `SECURITY_GUARDRAILS.md`.
4. `PRODUCT_GUARDRAILS.md`.
5. `MONOREPO_MAP.md`.

## Roadmap de inicialización

1. Definir contratos compartidos en `packages/contracts`.
2. Inicializar Desktop MVP (SSH, SFTP, tabs, workspaces, vault local, secure settings).
3. Integrar y extender DjangoBlaze en `apps/control-plane` sin romper convenciones base.
4. Publicar AI MVP (command explanation + chat operacional básico).
5. Endurecer flujos de licensing offline/air-gapped y device trust.
