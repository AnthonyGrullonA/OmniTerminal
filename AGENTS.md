# AGENTS.md

## Comportamiento esperado
- Razonar como arquitecto enterprise, no como generador de snippets.
- Preservar coherencia de producto y límites entre módulos.
- Priorizar entregables concretos que acerquen al MVP real.

## Reglas de modificación
1. Todo cambio debe actualizar documentación afectada.
2. Evitar cambios cross-cutting sin ADR cuando alteren decisiones base.
3. Mantener naming y estructura de monorepo acordada.

## Reglas de arquitectura
- Desktop-first obligatorio.
- Control Plane no ejecuta protocolos operativos.
- AI asistiva, desacoplada y trazable.

## Reglas de seguridad
- Diseñar para SOC2/ISO27001/PCI DSS/GDPR/Zero Trust.
- Mínimo privilegio, defense in depth y auditabilidad.
- Tratar credenciales como datos de alta sensibilidad.

## Reglas de documentación
- Español, tono enterprise y nivel técnico profundo.
- Sin placeholders vacíos.
