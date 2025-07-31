# AAX – Agent Action eXchange

**Versión fundacional – Julio 2025**

_AAX_ es un nuevo protocolo web diseñado específicamente para permitir que **agentes de inteligencia artificial autónomos**, debidamente autorizados por humanos, puedan ejecutar acciones reales en la web de forma **segura, trazable y estandarizada**.

## 🌐 ¿Qué es AAX?

AAX (Agent Action eXchange) es una infraestructura abierta que permite:

- Ejecutar acciones como `book`, `pay`, `confirm`, `cancel` de forma declarativa y estructurada.
- Establecer una conexión segura entre la voluntad del humano y la acción del agente.
- Proteger la autonomía humana con trazabilidad, reversibilidad y control.

## 🔐 Filosofía

AAX no empodera a las IAs por sí mismas.  
**Empodera al ser humano mediante la delegación controlada**, con trazabilidad y autorización explícita.

> "La IA no decide por ti. Actúa contigo, bajo tu firma."

## 📄 Estructura de un archivo `.agent.json`

```json
{
  "actions": {
    "pay": {
      "required_fields": ["amount", "recipient", "card_token"],
      "requires_consent": true
    },
    "book_flight": {
      "required_fields": ["from", "to", "date", "name"],
      "requires_consent": true
    }
  },
  "agent_requirements": {
    "verified_agent_id": true,
    "signature_required": true
  }
}
```

## 💳 AgentPay

AAX incluye una propuesta de **pasarela de pago IA-first**, llamada **AgentPay**, con:
- Tokenización de métodos de pago.
- Límite y control de acciones IA.
- Logs firmados y reversibles.

## 📚 Licencia

Este protocolo está publicado bajo licencia MIT.  
Kevin Mera Vera, 2025.

