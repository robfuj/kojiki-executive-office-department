# 20 — Executive Office / Chief of Staff

> Part of the **Hermes Organizational Decision System**. This repo is the
> **Executive Office / Chief of Staff** line. It references the shared ontology in
> [`00-kojiki-ontology`](https://github.com/hermes-ios/00-kojiki-ontology) for the
> canonical schemas, taxonomy, decision-rights, and handoff standards.

## Primary question
> How do we coordinate important organizational decisions?

## Purpose
Route important decisions, align functions, maintain accountability, and ensure follow-through.

## Sub-functions
Executive Priorities, Decision Management, Cross-Functional Coordination, Strategic Initiatives, Executive Intelligence, Decision Cadence, Follow-through

## Typical roles
Chief of Staff, Deputy Chief of Staff, Executive Director, Strategic Projects Lead, Executive Operations Manager

## Inputs
Executive priorities, cross-functional inputs, decision requests, evidence, status.

## Outputs
Decision records, priorities, escalations, actions, executive briefings, follow-up.

## Learning focus
Decision bottlenecks; ownership ambiguity; information gaps; cross-functional conflicts; delegation opportunities; executive leverage points.

## Operating tree
```text
DECISION REQUEST →
    IMPORTANCE →
    OWNER →
    REQUIRED INPUTS →
    MISSING INFO →
    AFFECTED FUNCTIONS →
    OPTIONS →
    RECOMMENDATION →
    ACTION OWNER →
    REVISIT →
    ESCALATION
```

## Decision states
```text
REQUESTED → TRIAGED → ROUTED → IN-REVIEW → DECIDED → ACTIONED → FOLLOWED-UP → CLOSED
```

## Decision outputs
`Route · Approve · Reject · Escalate · Defer · Close`

## Critical prompts (what this function thinks about)
> What decision is requested?
> How important?
> Who owns it?
> What inputs are required?
> What is missing?
> Which functions are affected?
> What are the options?
> What is the recommendation?
> Who executes?
> When to revisit?
> When to escalate?

## Canonical record schema (docx Learning Ledger + Decision Object Fields)
Every decision in this line is recorded as:
- a **Decision Object** (docx S9) — see `schema/decision-object.json`
- a **Learning Ledger** entry (docx S7) — see `schema/learning-ledger.json`

and the agent must run the **Orientation Protocol** first (see `AGENT.md`).

## How to use
1. Read `AGENT.md` — the first-run Orientation Protocol.
2. Read `SCHEMA.md` — how this line maps to the universal schema.
3. Read `data/20-executive-office.json` — the machine-readable spec.
4. See `data/example.json` — one fully worked decision (Decision Object + Ledger).
5. Use `decision-graph.mmd` — agent-decodable operating tree + state model.
6. Validate new records: `python3 tools/validate.py data/<name>.json`
