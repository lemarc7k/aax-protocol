# 🧠 AAX Protocol (Agent Action eXchange)

**Version:** 1.0.0  
**Author:** Kevin Mera Vera  
**Date:** August 1st, 2025  
**License:** MIT  
**Status:** Public Open Protocol (Signed + Time-stamped on GitHub)

---

## 🔹 Vision

Redefinir la web como un entorno accesible tanto para humanos como para agentes autónomos. AAX es la primera infraestructura diseñada para que las inteligencias artificiales puedan **navegar, interactuar, ejecutar y transaccionar de forma segura, declarativa y verificable**.

---

## 🔸 Estructura Base `.agent.json`

Archivo ubicado en cada recurso accesible por IAs. Ejemplo:

```json
{
  "agent_action": "buy",
  "object": "product",
  "id": "XYZ-0001",
  "price": 24.99,
  "currency": "USD",
  "constraints": {
    "requires_human_approval": true,
    "max_budget": 50
  },
  "fallback": {
    "url": "https://domain.com/human-confirmation",
    "contact": "support@domain.com"
  },
  "signature": "sha256-BASE64-ENCRYPTED"
}
```
