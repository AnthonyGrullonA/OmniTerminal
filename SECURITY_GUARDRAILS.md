# Security Guardrails

## Base de seguridad
- Zero Trust por defecto: identidad + dispositivo + contexto + riesgo.
- Criptografía moderna para secretos locales y en tránsito.
- Auditoría trazable de acciones privilegiadas.

## Requisitos mínimos
- MFA/WebAuthn en control plane para roles privilegiados.
- Vault local cifrado con rotación y hardening de claves.
- Device fingerprinting para licencias y postura de confianza.
- Registro de eventos apto para SOC2/ISO27001/PCI DSS/GDPR.

## MVP security scope
- Session recording avanzada y SIEM profundo quedan fuera de implementación inicial, pero se deben dejar hooks arquitectónicos.
