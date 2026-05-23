# Desktop App

## Runtime model
Cliente pesado desktop-native. Ejecuta sesiones y operaciones localmente con latencia mínima y control OS-level.

## Protocol engine
Responsable de SSH/SFTP/SCP/FTP/FTPS y base para RDP/VNC/Telnet/Mosh/Serial. Expone abstraction layer para providers y plugins.

## Vault local
Gestiona secretos con cifrado fuerte, integración con secure storage del SO y políticas de desbloqueo por sesión.

## Sync agent
Sincroniza únicamente metadata permitida (perfiles, tags, políticas, preferencias) con control plane.

## UI architecture
React + TypeScript por módulos: session workspace, connection explorer, tunnel manager, file explorer, snippets/macros y multi-execution.

## IPC architecture
Canal Tauri IPC con contratos explícitos, validación de payload, controles de permisos y telemetría de errores.
