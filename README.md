# OmniTerminal

OmniTerminal es una **AI-Native Operational Access Platform** con enfoque **desktop-first** para operación de infraestructura crítica en entornos enterprise.

## Propuesta de valor

OmniTerminal unifica, en una sola plataforma:

- Acceso operacional remoto (SSH/RDP/VNC/Túneles).
- Integraciones API y bases de datos.
- Operación cloud-native (Kubernetes, contenedores y nubes públicas).
- Observabilidad contextual durante sesiones.
- Gobierno de identidad, PAM moderno y auditoría continua.
- Copiloto operacional con inteligencia de sesión y análisis de riesgo.

## Principios del producto

- **Desktop-first**: el cliente de escritorio es el producto principal.
- **Zero Trust by Design**: identidad, dispositivo y contexto se verifican continuamente.
- **AI-native**: la IA asiste decisiones operativas con trazabilidad.
- **Enterprise-ready**: cumplimiento, resiliencia, control y modo air-gapped.
- **Arquitectura modular**: plataforma extensible y orientada a plugins.

## Arquitectura objetivo (alto nivel)

- **Cliente Desktop**: Tauri + Rust + React + TypeScript + Tailwind + xterm.js.
- **SaaS Control Plane**: Django/DRF + PostgreSQL.
- **Servicios complementarios**: FastAPI, Celery, Redis, NATS y WebSockets.
- **Telemetría**: OpenTelemetry y evolución a almacenamiento analítico.

## Estructura de documentación

Toda la documentación está centralizada en `docs/` y organizada por dominio:

- `docs/vision/`
- `docs/business/`
- `docs/product/`
- `docs/architecture/`
- `docs/security/`
- `docs/compliance/`
- `docs/ai/`
- `docs/integrations/`
- `docs/licensing/`
- `docs/deployment/`
- `docs/engineering/`
- `docs/operations/`
- `docs/investor/`
- `docs/api/`

## Punto de entrada recomendado

Para asistentes de ingeniería (Codex/Claude) y nuevos integrantes, leer primero:

1. `PROJECT_CONTEXT.md` (mapa de contexto y prioridades de lectura).
2. `docs/vision/vision-document.md`.
3. `docs/product/product-requirements-document.md`.
4. `docs/architecture/system-architecture.md`.
5. `docs/security/security-architecture.md`.

## Estado actual

El repositorio contiene una base documental enterprise en español para alinear estrategia, producto, arquitectura, seguridad, compliance y ejecución.

## Licenciamiento y operación offline

La plataforma está diseñada para modelos enterprise con validación periódica de licencias, soporte offline y operación en entornos air-gapped.
