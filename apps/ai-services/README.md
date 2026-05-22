# Ai Services

Servicios AI desacoplados para operational intelligence.

## Responsabilidades
- Explicación de comandos y asistente operacional.
- Correlación contextual básica de sesiones (sin acciones autónomas).

## Límites
- Stateless en MVP; sin almacenar secretos de operación.
- No reemplazar controles de seguridad/autoridad humana.

## Stack
FastAPI, Python, OpenRouter, Claude, GPT, Ollama.

## Relación
Consume contexto autorizado del control plane y del desktop para devolver recomendaciones.

## Roadmap
Chat básico → sugerencias de remediación → session intelligence avanzada.