---
tagline: "A self-hosted, AI-integrated personal intelligence platform and automated portfolio synchronization engine."
role: "Principal Software Engineer / Architect"
status: "active"
stack:
  - Svelte
  - TypeScript
  - Python
  - PLpgSQL
  - Docker
  - GitHub Actions
highlights:
  - "Architected a modular, self-hosted personal intelligence dashboard (selfhost) unifying multi-domain telemetry with local AI agent execution."
  - "Designed and implemented an automated, event-driven portfolio synchronization pipeline using GitHub Actions to dynamically compile and deploy system metrics."
  - "Engineered a highly concurrent task-scheduling engine (roommatesTasker) utilizing TypeScript and robust state-synchronization patterns."
description: "A highly integrated, self-hosted ecosystem designed to centralize personal telemetry, execute local AI-driven workflows, and automate professional portfolio synchronization with zero-overhead CI/CD pipelines."
---

## 🌟 Architectural Vision & System Design

The core architectural philosophy of this ecosystem is **local-first, decentralized intelligence**. Rather than relying on fragmented, third-party SaaS platforms that compromise data privacy, this system unifies fitness, nutrition, location intelligence, and task management into a single, self-hosted modular monolith. 

By decoupling the ingestion pipelines from the presentation layer, the architecture ensures high availability, low latency, and offline-first capabilities even when running on resource-constrained, self-hosted hardware (e.g., single-board computers).

```
┌─────────────────────────────────────────────────────────────────────────┐
│                           Svelte Client (UI)                            │
└────────────────────────────────────┬────────────────────────────────────┘
                                     │ (REST / WebSockets)
                                     ▼
┌─────────────────────────────────────────────────────────────────────────┐
│                     TypeScript / Python API Gateway                     │
└──────┬─────────────────────────────┬─────────────────────────────┬──────┘
       │                             │                             │
       ▼                             ▼                             ▼
┌──────────────┐              ┌──────────────┐              ┌──────────────┐