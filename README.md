# Skin-Tech Knowledge Hub – SSOT Operations Demo

> A single-page interactive demo showcasing how a **Single Source of Truth (SSOT)** system can govern content creation, validation, and lifecycle management in a regulated industry.

**[Live Demo](https://shaitamam-80.github.io/knowledge-ops-demo/)**

## The Problem

In skincare/pharma companies, product knowledge lives in scattered documents. Marketing writes claims that haven't been approved, training materials go out of sync with regulatory updates, and when regulations change — no one knows which live assets are affected.

**The result:** compliance violations, brand risk, and operational chaos.

## The Solution: SSOT-Driven Content Operations

This demo presents an operational architecture where:

1. **Knowledge Briefs (SSOT)** — A centralized, read-only repository of approved product claims, red lines, and clinical context. No one can edit the source of truth except authorized SMEs.

2. **Content Creation with Guardrails** — Creators (marketing/training) generate assets *from* the brief. The system enforces that all content traces back to an approved source.

3. **Automated Validation Gate** — Before any asset reaches the SME for factual review, an operational gate scans for forbidden claims and red-line violations. Hard stops prevent non-compliant content from progressing.

4. **Lifecycle & Cascade Management** — When a regulation changes, the system traces all downstream assets linked to the affected brief and triggers a surgical update cascade — freezing live assets and dispatching versioned update tasks.

## Key Concepts Demonstrated

| Concept | Where in Demo |
|---|---|
| SSOT as single source of truth | Brief cards (read-only, locked) |
| RBAC (Role-Based Access Control) | View-Only badges, Ops Admin role |
| Automated compliance gate | Forbidden word detection on submit |
| SLA tracking | Timer on validation pipeline |
| Metadata traceability | Brief ID → Asset ID linkage |
| Regulatory cascade | Lifecycle tab → freeze & update flow |
| Audit trail | Timestamped action log after cascade |

## Tech Stack

Single HTML file, zero dependencies to install:
- **Tailwind CSS** (CDN) — Utility-first styling
- **Font Awesome** — Icons
- **Vanilla JS** — All logic, no framework overhead

## Running Locally

Just open `index.html` in a browser. No build step required.

---

Built as a product-thinking demonstration for Knowledge Operations.
