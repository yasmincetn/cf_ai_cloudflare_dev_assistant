# PROMPTS.md

This file documents the AI-assisted coding prompts used during the development of this project.

ChatGPT was used as an assistant tool during development, primarily for ideation, prompt refinement, and debugging support. The final system design, logic, and implementation were independently completed and verified.

The prompts were used iteratively to design the architecture, implement features, and refine the behavior of the system.

---

## Prompt 1 — Project idea and architecture

Let’s design an AI assistant specifically tailored for Cloudflare’s ecosystem and products. The goal is to build a system that can help Cloudflare users and developers troubleshoot issues effectively.

The assistant should:
- Understand Cloudflare-specific problems
- Identify the relevant Cloudflare product (e.g., Workers, KV, R2, D1, etc.)
- Classify the request type (troubleshooting, explanation, or recommendation)
- Provide structured, actionable guidance to resolve user issues

Suggest an appropriate architecture for this system.

---

## Prompt 2 — Cloudflare setup

Help me set up a Cloudflare Agents project using Node.js, npm, and Wrangler. Guide me step by step to run the project locally and connect it to Workers AI.

---

## Prompt 3 — Agent behavior design

Given my Cloudflare Agents server code, help me design a system prompt so the assistant behaves as a Cloudflare troubleshooting agent. It should classify user requests (troubleshooting, explanation, recommendation) and detect the related Cloudflare product.

---

## Prompt 4 — Structured output

Modify the assistant so that it always returns valid JSON with the following fields:
issue_type, related_product, summary, likely_cause, recommended_steps, confidence.

Add rules for different types of requests and ensure no text is returned outside JSON.

---

## Prompt 5 — Frontend integration

Given my React app, help me parse the JSON response from the assistant and display it as a structured UI instead of raw JSON. The UI should show summary, cause, and steps clearly.

---

## Prompt 6 — UI refinement and UX improvements

Improve the UI rendering of the assistant responses. Hide likely_cause when it is null, hide recommended_steps when empty, display readable labels for issue types, and support multi-product outputs such as "Multiple Products" for comparison cases.

---

## Note

AI tools were used to assist development, but the final system design, integration, and modifications were implemented and validated manually.
