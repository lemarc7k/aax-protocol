# AAX – Agent Action eXchange

**Foundational Release – July 2025**  
**Created by:** Kevin Mera Vera (lemarc7k)

_AAX_ is a new web protocol designed to enable **autonomous AI agents**, properly authorized by humans, to perform real-world actions online in a **secure, traceable, and standardized** way.

---

## 🌐 What is AAX?

**Agent Action eXchange (AAX)** is an open infrastructure that enables:

- Declarative and structured actions like `book`, `pay`, `confirm`, `cancel`
- A secure link between human intent and agent execution
- Human-centered autonomy with traceability, reversibility, and control

---

## 🔐 Philosophy

AAX does not empower AI on its own.  
It **empowers humans through controlled delegation**, backed by intent and verifiable consent.

> _“AI doesn’t decide for you. It acts with you, under your signature.”_

---

## 📄 Structure of a `.agent.json` File

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

💳 AgentPay – The First AI-First Payment Gateway
AAX introduces a complementary system:
AgentPay, the first payment gateway designed for AI agents acting on behalf of humans.

Features:

Tokenized payment methods

Transaction limits, logs, and signatures

Traceable and reversible payments

📁 Repository Contents
aax-protocol.md → Protocol’s foundational document

agent.json → Standardized agent definition example

/specs → Technical specifications and diagrams (WIP)

README.md → Main file (Spanish)

README.en.md → English version

LICENSE → MIT License

📖 License
This protocol is released under the MIT License, promoting adoption, extension, and open innovation.
🛡️ AAX Protocol is protected by public authorship proof — see PROOF-OF-AUTHORSHIP.docx and PROOF_AAX_Whitepaper.ots.

🪶 Founder
Kevin Mera Vera
Creator of AAX – lemarc7k
Perth, Australia – 2025
