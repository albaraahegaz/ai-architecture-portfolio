# AI Architecture Portfolio

Al-baraa Hegaz · [AI Architecture Design](https://github.com/albaraahegaz/ai-architecture-portfolio) with Eng. Sameh Amin · Oct–Dec 2026

My work for the course. I'm designing one AI system across the sessions, and by the end it becomes my capstone architecture.

## Scenario

A support assistant for an online retailer.

Customers write in Arabic or English to ask where their order is, how to return something, or what the warranty covers. Today, support agents answer these by hand, searching policy documents and checking the order system. Answers are slow and sometimes inconsistent.

The assistant answers policy questions using the company's own documents (RAG) and looks up order status through read-only tools. It always shows which source it used. It does not issue refunds, change orders, or make exceptions. Those cases go to a human agent with the conversation summary attached.

*Status: draft. I'll refine the scenario as the sessions go on.*

## Assumptions

- A mid-size online retailer selling in Egypt and Saudi Arabia (fictional company, made-up data)
- Customers write in Arabic (including dialects) and English
- Customer data stays in the region and follows local data protection rules
- The assistant can only read order data, never write to it
- A human agent handles every refund, complaint, and exception in the first version
- Answers should come back in a few seconds, since customers are waiting in a live chat

## Repo layout

| Folder | Contents |
|---|---|
| `docs/` | One note per session (`01-framing.md`, `02-building-blocks.md`, ...) |
| `diagrams/` | Exported PNG/SVG plus the editable source files |
| `adr/` | One Architecture Decision Record per decision (`0001-model-hosting.md`, ...) |
| `capstone/` | Final architecture PDF and slides |

## How to read this repo

1. Start with the scenario and assumptions above.
2. Follow `docs/` in order to see how the design grew.
3. Read `adr/` for the reasons and trade-offs behind each decision.
4. Look at `diagrams/` for the visual architecture.
5. Finish with `capstone/` for the complete design.

## Progress

- [x] Repo created
- [ ] Session 1: Architecture Views, Steps and Process (18 Oct)
- [ ] Session 2: AI System Building Blocks (25 Oct)
- [ ] Session 3: LLM & RAG Architecture (1 Nov)
- [ ] Midpoint Quiz + Capstone Part 1 (due 14 Nov)
- [ ] Session 4: Agentic AI Architecture (15 Nov)
- [ ] Session 5: Security, Governance, Evals (22 Nov)
- [ ] Session 6: Enterprise Case Studies (29 Nov)
- [ ] Final project (due 13 Dec)