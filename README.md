# AAX – Agent Action eXchange

**Versión fundacional – Julio 2025**  
**Creador:** Kevin Mera Vera (lemarc7k)

_AAX_ es un nuevo protocolo web diseñado específicamente para permitir que **agentes de inteligencia artificial autónomos**, debidamente autorizados por humanos, puedan ejecutar acciones reales en la web de forma **segura, trazable y estandarizada**.

---

## 🌐 ¿Qué es AAX?

**Agent Action eXchange (AAX)** es una infraestructura abierta que permite:

- Ejecutar acciones como `book`, `pay`, `confirm`, `cancel` de forma **declarativa y estructurada**.
- Establecer una **conexión segura entre la voluntad del humano y la acción del agente**.
- Proteger la autonomía humana con **trazabilidad, reversibilidad y control verificable**.

---

## 🔐 Filosofía

AAX no empodera a las IAs por sí mismas.  
**Empodera al ser humano mediante la delegación controlada.**  
Cada acción requiere una firma, una intención y un límite.

> _“La IA no decide por ti. Actúa contigo, bajo tu firma.”_

---

## 📄 Estructura del archivo `.agent.json`

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

💳 AgentPay – Pasarela de Pagos IA-first
AAX incluye una propuesta complementaria:
AgentPay, la primera pasarela de pagos diseñada para agentes IA autorizados.

Características:

Tokenización de métodos de pago

Límites, logs y firma de transacciones

Trazabilidad y reversibilidad garantizadas

📁 Contenido del repositorio
aax-protocol.md → Documento fundacional del protocolo

agent.json → Ejemplo de definición estándar de agente

/specs → Especificaciones ampliadas y diagramas (WIP)

README.md → Este archivo

LICENSE → Licencia MIT
