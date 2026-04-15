# Operational Map

A structured operational knowledge surface that gives teams instant answers to three questions: **Who owns this client? What governs it? What's the current state?**

This replaces the current workflow of searching through email threads, static SharePoint folders, stale OneNote files, and asking teammates for information that should be queryable in seconds.

[![Live Demo](https://img.shields.io/badge/demo-Live%20Prototype-6D2077)](https://insight2night.github.io/OperationalMap/)

---

## Live Demo

**[https://insight2night.github.io/OperationalMap/](https://insight2night.github.io/OperationalMap/)**

Open the link in any browser. No install, no dependencies, no backend. This is the interactive prototype with hardcoded mock data — click through everything.

You can also open `demo.html` locally by double-clicking it.

---

## What Exists Today

This repo contains the **Stage 0 prototype**: a single self-contained HTML file (~940 lines) with inline CSS and JS. No frameworks, no build tools, no external dependencies.

### Views
- **Dashboard** — searchable client grid with status badges, staleness indicators, filter pills, and sorting
- **Client Detail** — tabbed layout: Overview, Contacts, Documents, Activity Log
- **Team View** — workload distribution across team members with clickable client lists
- **Stale Report** — clients not updated in 30+ days, sorted by staleness, with review actions
- **Documents** — all linked documents across clients

### Working Interactions
- Real-time search (filters by client name and owner)
- Status filter pills (Active / Onboarding / Winding Down / Stale)
- Sort by last updated, name, or status
- Click-through navigation: cards → detail → tabs → back via breadcrumbs
- Add Client modal with form fields
- Toast notifications on actions (Mark Reviewed, Edit, Link Document)
- Keyboard shortcuts (Esc closes modal, Ctrl+K focuses search)

### AI Placeholders (Directional Only)
- Dashboard: "AI Features Coming Soon" banner (Thread Summarization, Stale Detection, Smart Updates, Agent Integration)
- Client Detail: disabled "AI Assistant" panel with planned capabilities

These do not execute — they signal where the product goes next.

---

## Why This Matters for the Platform

Horizon has 20+ agents, but they all operate on siloed, unstructured data. No agent today can answer basic operational questions like "who owns Acme?" or "when was the last SOW updated?"

**This is the missing structured data layer.**

| Current State | Problem |
|---------------|---------|
| Email | Unsearchable, siloed per person |
| SharePoint | Static file storage, no relational context |
| OneNote | Becomes an unmaintainable graveyard |
| ServiceNow KB | Approval cycles too slow for fast-moving teams |
| SMART / InsightGPT | Only as good as the data they can access |

Operational Map creates the structured, maintained, attributable data surface that makes AI agents — including Horizon agents — actually useful for operations.

---

## Repository Structure

```
/OperationalMap
├── docs/
│   └── index.html       ← GitHub Pages (live demo)
├── demo.html             ← Prototype source (same file)
├── index.html            ← Placeholder for production app
├── README.md             ← This file
└── INTENT.md             ← Initiative strategy and vision
```

---

## Roadmap

| Stage | What | Status |
|-------|------|--------|
| **0** | Interactive prototype — validate UX and workflow | ✅ Complete (this repo) |
| **1** | Production web app — searchable dashboard with CRUD, auth, audit trail | 📋 Next |
| **2** | AI augmentation — thread summarization, stale detection, smart updates | 📋 Planned |
| **3** | Generalize — any team spins up their own map | 📋 Planned |
| **4** | Horizon integration — live as a native agent data layer | 📋 Future |

Each stage earns the next by proving value. No stage begins until the previous one demonstrates real adoption.

---

## What's Needed Next

| Resource | Purpose | Status |
|----------|---------|--------|
| GitHub Copilot access | Accelerate Stage 1 build | ⏳ Requested |
| LLM API access (internal) | Stage 2 AI features | ⏳ Discussing |
| Azure hosting (internal) | Deploy Stage 1 for team use | ⏳ Pending |
| Horizon integration pathway | Stage 4 agent/data layer | ⏳ Needs collaboration |

---

## Contact

**Neal Anderson** — Neal.Anderson@insight.com
Internal use only. Property of Insight Enterprises.