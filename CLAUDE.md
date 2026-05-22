# CLAUDE Contexto Persistente

## Identidad del producto
OmniTerminal es una plataforma de acceso operacional unificado, no un simple terminal emulator.

## Prioridades del MVP
- Desktop: SSH, SFTP, tabs, workspaces, local vault, licensing, secure settings.
- Control Plane: auth, organizations, subscriptions, seats, device registration, sync metadata.
- AI: explicación de comandos, chat operacional básico.

## Reglas de diseño
- Preservar boundaries claros desktop/control-plane/ai.
- Evitar acoplar runtime SSH al SaaS.
- Priorizar estabilidad, seguridad y extensibilidad pragmática.
