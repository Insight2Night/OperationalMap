# Operational Map

A living org map — browse by people or by client, see every connection, verify ownership, trace every change. Not an agent. The connective tissue underneath all agents.

[![Live Demo](https://img.shields.io/badge/demo-Live%20Prototype-6D2077)](https://insight2night.github.io/OperationalMap/)

---

## Live Demo

**[https://insight2night.github.io/OperationalMap/](https://insight2night.github.io/OperationalMap/)**

Open in any browser. No install, no dependencies. Click through everything — toggle views, expand nodes, drill into assignments, verify connections.

To run locally: open `demo-map.html` in a browser.

---

## What This Is

One search. Two views. Every connection.

- **Client View** — expand any client to see every person connected to it, their role, and verification status
- **People View** — expand any person to see every client they're assigned to
- **Drill down** — click any connection to see who assigned it, when, and who verified it
- **Verify / Edit / Request** — anyone can suggest changes, approvers verify, everything traceable

### The Core Idea

> Anyone can update. Only certain people verify. Everything is traceable.

This is how you get company-wide participation without chaos.

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
│   └── index.html          ← GitHub Pages (live demo)
├── demo-map.html            ← Map prototype source
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