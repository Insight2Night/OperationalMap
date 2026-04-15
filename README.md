# Operational Map

The living map of everything Insight — people, clients, teams, projects, knowledge — searchable, verifiable, permission-based, and always current. Not an agent. The connective tissue underneath all agents.

**Stop hunting. Start knowing.**

[![Live Demo](https://img.shields.io/badge/demo-Live%20Prototype-6D2077)](https://insight2night.github.io/OperationalMap/)

---

## Live Demo

**[https://insight2night.github.io/OperationalMap/](https://insight2night.github.io/OperationalMap/)**

Open in any browser. No install, no dependencies. Switch between four views, filter by category, drill into any node, verify connections.

To run locally: open `demo-v4.html` in a browser.

---

## What This Is

A universal knowledge surface for everyone at Insight — not just operations.

### Universal Node Types
- **People** — any employee, any department
- **Clients** — active, onboarding, historical
- **Teams & Groups** — org units, distribution groups
- **Projects** — active engagements tied to clients and people
- **Documents** — SOWs, contracts, process docs, references

### Four Views, Same Data
- 🕸️ **Graph** — Obsidian-style force-directed constellation. Drag, zoom, explore. Stale nodes fade. Verified nodes glow.
- 🃏 **Cards** — visual grid for quick scanning
- 📋 **Table** — sortable columns for data people
- 🏗️ **Tree** — collapsible hierarchy grouped by type

### Interactions
- **Category tabs** filter by node type (People, Clients, Teams, Projects, Docs)
- **Status filters** narrow within any category
- **Search** across everything — the graph flies to matching nodes
- **Click any node** — detail panel with connections, verification, tags
- **Verify / Edit** — anyone suggests changes, approvers verify, everything traceable

### The Core Idea

> Anyone at any level finds what they need in seconds. Anyone can update. Only certain people verify. Everything is traceable.

---

## Why This Matters for the Platform

Horizon has 20+ agents, but they all operate on siloed, unstructured data. No agent can answer "who owns Acme?" because that answer lives in email threads and personal notebooks.

**This is the missing structured data layer.**

| What Exists | The Gap |
|-------------|---------|
| Email | Unsearchable, siloed per person |
| SharePoint | Static file storage, no relational context |
| OneNote | Unmaintainable graveyard |
| ServiceNow KB | Approval cycles too slow for fast-moving teams |
| Org charts (Workday) | Reporting structure — not who works on what client |
| CRM (Salesforce) | Sales relationships — not operational ownership |

**None of these answer:** "Show me every person connected to this client and their role — verified and current."

The map does. Agents read from it. Humans maintain it. AI assists with authoring.

### Two Layers, Separated by Design

| Layer | What Lives Here | Who Maintains It |
|-------|----------------|-----------------|
| **The Map** | People, clients, roles, assignments, verification | Humans — anyone edits, approvers verify |
| **Agent Layer** | Notes, summaries, documents, authored content | AI drafts, humans approve |

The map stays clean. The agents handle the messy stuff.

---

## Repository Structure

```
/OperationalMap
├── docs/
│   └── index.html          ← GitHub Pages (live demo — v4)
├── demo-v4.html             ← Current prototype (4 views, universal nodes)
├── demo-graph.html          ← Graph-only prototype (earlier iteration)
├── demo-map.html            ← List-based map prototype
├── demo-dashboard.html      ← Full dashboard demo (vision reference)
├── demo.html                ← Original dashboard prototype
├── index.html               ← Placeholder for production app
├── README.md                ← This file
└── INTENT.md                ← Initiative strategy and vision
```

---

## How It Would Live in Horizon

Not as an agent. As a **map button** — infrastructure that every agent can read from.

```
┌──────────────────────────────────────────┐
│  HORIZON                                 │
│                                          │
│  [InsightGPT] [AskHR] [AskGTM] [OpsIQ]  │
│                                          │
│  ┌────────────────────────────────────┐  │
│  │  🗺️ MAP                            │  │
│  │  People ↔ Clients ↔ Roles         │  │
│  │  Ownership ↔ Verification         │  │
│  │  Traceable. Accountable. Live.    │  │
│  └────────────────────────────────────┘  │
│                                          │
│  Agents READ from the map.               │
│  Humans MAINTAIN the map.                │
│  AI ASSISTS with authoring.              │
│  Approvers VERIFY accuracy.              │
└──────────────────────────────────────────┘
```

---

## Roadmap

| Stage | What | Status |
|-------|------|--------|
| **0** | Interactive prototype — validate the map concept | ✅ Complete (this repo) |
| **1** | Production app — search, browse, verify, edit with auth and audit trail | 📋 Next |
| **2** | AI agent layer — summarize activity, auto-extract from threads, flag stale | 📋 Planned |
| **3** | Generalize — any team spins up their own map | 📋 Planned |
| **4** | Horizon integration — live as a native map button / data layer | 📋 Future |

Each stage earns the next by proving value.

---

## What's Needed Next

| Resource | Purpose | Status |
|----------|---------|--------|
| GitHub Copilot access | Accelerate Stage 1 build | ⏳ Requested |
| LLM API access (internal) | Stage 2 agent layer | ⏳ Discussing |
| Azure hosting (internal) | Deploy Stage 1 for team use | ⏳ Pending |
| Horizon integration pathway | Stage 4 map button | ⏳ Needs collaboration |

---

## Contact

**Neal Anderson** — Neal.Anderson@insight.com
Internal use only. Property of Insight Enterprises.