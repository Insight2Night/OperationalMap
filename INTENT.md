# INTENT — Operational Map

## Purpose

Build a structured operational knowledge surface that eliminates the time teams spend searching through fragmented email, SharePoint, OneNote, and tribal knowledge — starting with the ITAD Disposal team and designed to generalize across Insight.

The immediate goal: any team member can instantly answer **Who owns this client? What governs it? What's the current state?**

The long-term goal: create the foundational structured data layer that makes AI agents — including Horizon agents — actually useful for operations.

## Audience

**Primary (now):** ITAD Disposal project coordinators and project managers who currently operate through fragmented email workflows.

**Secondary (next):** Infrastructure teams — technicians needing diagrams, support reps needing canned responses, PMs needing cross-project visibility.

**Tertiary (future):** The Horizon platform team, as a data layer and potential native agent source. Any fast-moving team at Insight not yet in ServiceNow.

## Context

This matters now because:

1. **Horizon has 20+ agents but no structured operational data layer.** No agent can answer basic questions about client ownership or project state because the data lives in email threads and personal notebooks.

2. **The ITAD team is exploring a shift from role-based to client-based ownership.** There is no infrastructure to support that shift. Everything still lives in email.

3. **Existing tools don't solve this problem:**

   | Tool | Gap |
   |------|-----|
   | Email | Unsearchable, siloed per person |
   | SharePoint | Static file storage, no relational context |
   | OneNote | Becomes an unmaintainable graveyard |
   | ServiceNow KB | Approval cycles too slow for fast-moving teams |
   | SMART / InsightGPT | Only as good as the data they can access |

4. **Informal versions of this tool have been built before** — Figma diagrams for technicians, visual process maps, Power Apps interfaces, quick-reference systems. Teams used them. They worked. They didn't scale. This is the iteration that is designed to.

5. **There is active support from AI Champions in Infrastructure.** This is not a rogue side project.

## Method

**Stage 0 — Prototype (current):** Interactive single-file demo to validate UX, workflow, and stakeholder interest. No backend. Mock data. Clickable and demo-ready.

**Stage 1 — Production app:** Searchable client dashboard with full CRUD, role-based permissions, audit trail, stale content detection. Every edit logged with timestamps and attribution.

**Stage 2 — AI augmentation:** LLM integration via internal API. Paste email threads → auto-extract updates. Natural language queries. AI-drafted node updates with human approval. Proactive stale flagging.

**Stage 3 — Generalization:** Template system so any team can spin up their own Operational Map. Custom node types, fields, permissions. Multi-team dashboard.

**Stage 4 — Horizon integration:** Operational Map as a native Horizon agent or data source. Structured data feeds existing agents. Teams build agent-ready knowledge surfaces.

Each stage earns the next by proving value. No stage begins until the previous one demonstrates real adoption.

## Resources

| Resource | Status |
|----------|--------|
| Developer (Neal Anderson) | ✅ Available |
| Client data (ITAD Disposal) | ✅ Available — needs structuring |
| GitHub repository | ✅ Created (Insight2Night/OperationalMap) |
| GitHub Copilot access | ⏳ Requested |
| Azure hosting (internal) | ⏳ Needed for Stage 1 deployment |
| LLM API access (internal) | ⏳ Needed for Stage 2 |
| Horizon integration pathway | ⏳ Requires collaboration with Horizon team |

## Impact

**For the Disposal team (immediate):** Time spent searching for client info drops from minutes to seconds. Client ownership is clear, documented, and current. New team members onboard faster. The shift to client-based ownership has infrastructure to support it.

**For Infrastructure (medium-term):** Any team can spin up their own Operational Map. Cross-team visibility for leadership. Structured data ready for ServiceNow migration when the time comes.

**For Insight at large (long-term):** Every Horizon agent gains a structured, maintained data layer. The gap between "we have AI tools" and "AI tools are actually useful" closes. Client-facing agents become possible — trained on approved, structured content.

## Scope

**Included now:** Client status and ownership tracking, contact management, document linking, activity logging, stale content detection, search and filtering, team workload visibility.

**Not included now:** Real backend or persistence, authentication, email integration, replacing ServiceNow or any existing system, ticket management, mobile native app, external deployment.

## Strategy

```
Stage 0: Prototype → proves the workflow makes sense and stakeholders see value
    ↓
Stage 1: Production app → proves the team will use a structured tool daily
    ↓
Stage 2: AI augmentation → proves AI adds real value on structured data
    ↓
Stage 3: Generalize → proves the pattern scales beyond one team
    ↓
Stage 4: Horizon integration → proves this is infrastructure, not a side project
```

Key principles:
- **Structure before AI** — clean data first, intelligence layer second
- **Complement, never compete** — this makes ServiceNow, SMART, and Horizon better, not obsolete
- **Earn permission through results** — don't ask to build a platform; show a working tool and let others see the platform potential
- **Build to hand off** — clean code, clear docs, team ownership from day one

## Signals

**Stage 0–1 (Adoption):**
- Teammates bookmark the app
- Someone says "I checked the map" instead of "let me dig through email"
- A teammate asks "can we add [X] to this?"
- Time-to-answer for "who handles this client?" drops from minutes to seconds

**Stage 2 (AI Value):**
- AI-drafted updates are accurate enough to approve with minimal edits
- Team pastes email threads into the tool instead of manually summarizing
- Stale content gets flagged before it causes a problem

**Stage 3+ (Scale):**
- A second team adopts the tool without Neal building it for them
- The tool is discussed as infrastructure, not a side project
- Dan or the Horizon team initiates an integration conversation

## Risks

| Risk | Likelihood | Mitigation |
|------|-----------|------------|
| Perceived as distraction from core duties | Medium | Keep Stage 0–1 lightweight. Deliver on all current responsibilities first. |
| No dev tooling access approved | Medium | Prototype requires zero tooling. Escalate through AI Champions if needed. |
| Team doesn't adopt it | Low | Pain is real and validated. Informal tools were already used. |
| Overlaps with ServiceNow rollout | Medium | Position explicitly as a bridge. Structured data makes ServiceNow migration easier. |
| Scope creep | High | Each stage must prove value before the next begins. This document exists to enforce that. |
| Single point of failure (Neal) | High initially | Clean code, clear documentation, team co-ownership from Stage 1. |
| Horizon integration technically infeasible | Unknown | Demo to Dan first. Let him assess feasibility. |

## Values

1. **Clarity over cleverness** — if it's not immediately understandable, simplify it
2. **Structure before intelligence** — clean data first, AI second, always
3. **Team-built, not top-down** — the people who do the work build the knowledge
4. **Human-governed, AI-assisted** — AI drafts, humans approve, structure enforces
5. **Accountability is a feature** — timestamps, attribution, activity logs, stale flags

## Edge

1. **The gap is real and universal.** Every team at Insight has some version of this problem. No existing tool solves it.

2. **Horizon has 20+ agents but no structured operational data layer.** This is the missing foundation. Every agent gets smarter when it has clean, maintained, structured data to work with.

3. **The timing is right.** Insight is investing heavily in AI. Teams are being asked to adopt AI tools. But AI on unstructured email threads is theater. This creates the structured surface that makes AI adoption real.

4. **This has been validated informally across multiple roles.** Figma diagrams, Power Apps interfaces, process maps, quick-reference systems — teams used them. They worked. They didn't scale. This is the version designed to.

5. **The cost of inaction is invisible but massive.** Every day, every team member spends time searching for information that should take seconds. Multiply that across Infrastructure. The ROI is enormous — it's just distributed across thousands of small moments of friction.

---

_Last updated: April 15, 2026_
_Author: Neal Anderson (Insight2Night)_
