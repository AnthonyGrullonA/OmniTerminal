# Desktop

Desktop app Tauri/Rust responsable del runtime operacional (SSH/SFTP/túneles/vault local).

## Responsabilidades
- Gestión de sesiones y workspaces.
- Rendering terminal e interacción de operador.
- Ejecución local segura y offline parcial.

## Límites
- No implementar billing/tenancy aquí.
- No depender de cloud para operar funciones core MVP.

## Stack
Tauri, Rust, React, TypeScript, xterm.js, Zustand, TanStack Query.

## Relación
Consume contratos de `packages/contracts` y sincroniza metadata con `apps/control-plane`.

## Roadmap
MVP SSH/SFTP → vault endurecido → plugins de protocolos adicionales.