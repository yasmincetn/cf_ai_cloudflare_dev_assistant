# Cloudflare AI Troubleshooting Agent

An AI-powered assistant designed to help developers troubleshoot Cloudflare-related issues using structured outputs and product-aware reasoning.

---

## 🚀 Overview

This project is a Cloudflare-focused AI assistant that analyzes developer queries and provides structured, actionable responses.

Instead of generic chatbot answers, the system:

* Identifies the type of request (troubleshooting, explanation, recommendation)
* Detects the relevant Cloudflare product
* Returns clear summaries, root causes, and recommended steps

---

## ✨ Features

* 🧠 LLM-powered reasoning (Cloudflare Workers AI)
* 💬 Chat-based interface
* 🛠 Troubleshooting-focused responses
* 📦 Cloudflare product awareness (Workers, KV, R2, D1, etc.)
* 📊 Structured JSON output:

  * Summary
  * Likely cause
  * Recommended steps
* 🎨 Clean developer-friendly UI
* 🔀 Multi-product comparison support

---

## 🧱 Tech Stack

* Cloudflare Workers
* Workers AI
* Agents SDK
* React + TypeScript
* Tailwind CSS

---

## 🧪 Example

**User Input:**

> My Cloudflare Worker returns 500 error on fetch

**Agent Output:**

* Issue Type: Troubleshooting
* Product: Workers
* Summary: Runtime error during fetch handling
* Cause: Incorrect handler or missing response return
* Steps:

  1. Verify request handler
  2. Check response return
  3. Inspect logs via Wrangler

---

## 🧠 How It Works

1. User submits a query via chat
2. The system analyzes intent and context
3. The model generates structured output
4. UI parses and displays results in a readable format

---

## 🔄 In Progress

This project is currently being extended with a **Retrieval-Augmented Generation (RAG)** pipeline to:

* Integrate Cloudflare documentation
* Improve response grounding
* Provide context-aware troubleshooting

---

## 🛠 Run Locally

```bash
npm install
npm run dev
```

Then open:

```
http://localhost:5173
```

---

## 🎯 Goal

To build a documentation-aware AI assistant tailored specifically for Cloudflare developers, focusing on real-world debugging and developer experience.

---

## 🙌 Acknowledgements

Built using Cloudflare Workers AI and Agents SDK.

---

## 📄 License

MIT License
Copyright (c) 2025 Cloudflare Inc.
Copyright (c) 2026 Yasmin Cetin
