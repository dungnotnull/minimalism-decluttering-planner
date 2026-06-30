# PROJECT-detail.md — Minimalism Decluttering Planner

## Executive Summary
`minimalism-decluttering-planner` is a harness skill in the **Lifestyle & Personal** cluster (idea #195). Plans and manages home decluttering with a staged method, decision criteria and habit systems to keep spaces minimal long-term. It executes a research-first, framework-grounded workflow that ends in a multi-dimensional score and a prioritized, effort/impact-ranked improvement roadmap.

> **Note:** Recommendations are evidence-based decision-support; validate against your specific context before acting.

## Problem Statement
People start decluttering but stall from decision fatigue and rebound clutter. This skill builds a staged, room-by-room plan using recognized decluttering methods, decision heuristics, and habit-maintenance systems tailored to the household.

## Target Users & Use Cases
- Practitioners, learners and small teams who need an expert-grade, evidence-based analysis without hiring a specialist.
- Trigger examples:
  - "My whole apartment is cluttered, where do I start?" → the skill runs its full harness and returns a scored deliverable.
  - "I can't let go of keepsakes" → the skill runs its full harness and returns a scored deliverable.
  - "I declutter but it comes back" → the skill runs its full harness and returns a scored deliverable.
  - "I live in a studio" → the skill runs its full harness and returns a scored deliverable.
  - "Moving to a smaller place in 4 weeks" → the skill runs its full harness and returns a scored deliverable.

## Harness Architecture
```
User input
   │
   ▼
[Stage 1 Intake]  sub-household-intake
   │
   ▼
[Stage 2 Research]  SECOND-KNOWLEDGE-BRAIN.md + WebSearch/WebFetch
   │
   ▼
[Stage 3 Gate]  requirement validation
   │
   ▼
[Stage 4 Scoring]  sub-declutter-method-selector  → score vs frameworks
   │
   ▼
[Stage 5 Challenge]  devil's-advocate review
   │
   ▼
[Stage 6 Synthesis]  sub-maintenance-system  → scored report + roadmap
```

## Full Sub-Skill Catalog
### `sub-household-intake`
- **Purpose:** Capture rooms, clutter hotspots, household members, time budget, emotional-attachment items and goals.
- **Inputs:** structured fields from prior stages / user.
- **Outputs:** structured record consumed by the next stage.
- **Tools:** Read, WebSearch/WebFetch (as needed).
- **Quality gate:** outputs are complete, evidence-linked, and assumptions are explicit.
### `sub-declutter-method-selector`
- **Purpose:** Select and sequence the appropriate method (KonMari category vs room-by-room) for the household.
- **Inputs:** structured fields from prior stages / user.
- **Outputs:** structured record consumed by the next stage.
- **Tools:** Read, WebSearch/WebFetch (as needed).
- **Quality gate:** outputs are complete, evidence-linked, and assumptions are explicit.
### `sub-decision-engine`
- **Purpose:** Apply decision heuristics to ambiguous items and reduce decision fatigue.
- **Inputs:** structured fields from prior stages / user.
- **Outputs:** structured record consumed by the next stage.
- **Tools:** Read, WebSearch/WebFetch (as needed).
- **Quality gate:** outputs are complete, evidence-linked, and assumptions are explicit.
### `sub-maintenance-system`
- **Purpose:** Design habit loops and one-in-one-out rules to prevent rebound clutter.
- **Inputs:** structured fields from prior stages / user.
- **Outputs:** structured record consumed by the next stage.
- **Tools:** Read, WebSearch/WebFetch (as needed).
- **Quality gate:** outputs are complete, evidence-linked, and assumptions are explicit.
### `sub-declutter-roadmap`
- **Purpose:** Produce a scheduled, room-by-room plan with realistic session sizing.
- **Inputs:** structured fields from prior stages / user.
- **Outputs:** structured record consumed by the next stage.
- **Tools:** Read, WebSearch/WebFetch (as needed).
- **Quality gate:** outputs are complete, evidence-linked, and assumptions are explicit.

## Evaluation Frameworks
1. **KonMari Method (Marie Kondo)** — Category-based tidying sequence with a keep/discard decision heuristic ('spark joy').
2. **Minimalism (The Minimalists / Essentialism)** — Philosophy and decision frameworks for reducing to the essential and resisting accumulation.
3. **Four-box / OHIO decision rules** — Operational sorting heuristics (keep/donate/trash/relocate; Only Handle It Once).
4. **Habit loop (Atomic Habits / Fogg Behavior Model)** — Cue-routine-reward design for maintenance habits and one-in-one-out rules.
5. **Swedish death cleaning (döstädning)** — Lifecycle-aware decluttering reducing future burden on others.

## Scoring Dimensions
- Clutter density baseline
- Decision-rule clarity
- Plan realism (time/effort)
- Maintenance-habit strength
- Emotional-attachment handling
- Sustainability

Each dimension is scored 0–100 (or 1–5) with an explicit rationale and at least one cited source or stated assumption. The composite score is a transparent weighted aggregate; weights are disclosed.

## Skill File Format Specification
- Frontmatter: `name` (= `minimalism-decluttering-planner`), `description` (one line).
- Required sections: Role & Persona, Workflow (Harness Flow), Sub-skills Available, Tools, Output Format, Quality Gates.

## E2E Execution Flow
1. Parse request; classify the task and detect missing inputs (ask targeted questions).
2. Run intake sub-skill → structured profile.
3. Sync evidence from the knowledge brain; refresh via WebSearch/WebFetch when available; otherwise signal degraded mode.
4. Run the validation gate — **halt and route out** on red flags.
5. Score against frameworks; record evidence per dimension.
6. Devil's-advocate pass: challenge weakest assumptions, seek disconfirming evidence.
7. Synthesize the deliverable: scored report + prioritized roadmap (effort × impact).
8. Run quality gates; only then present output.

## SECOND-KNOWLEDGE-BRAIN Integration
- Sources: ArXiv (cs.CY, econ.GN) + the authoritative domain sources listed in `CLAUDE.md`.
- Crawl config and append format are defined in `tools/knowledge_updater.py` and `SECOND-KNOWLEDGE-BRAIN.md`.

## Supporting Tools Spec — `knowledge_updater.py`
- **Inputs:** crawl query list (below), source URLs, last-run timestamp.
- **Outputs:** appended, de-duplicated, date-stamped entries in `SECOND-KNOWLEDGE-BRAIN.md`.
- **Schedule:** weekly cron.
- **Crawl queries:** `clutter wellbeing psychology study 2026`, `habit formation maintenance behavior change`, `decluttering intervention effectiveness`, `decision fatigue reduction heuristics`

## Quality Gates (must all pass before output)
- Every scored dimension cites a source or states an assumption.
- The applicable safety/compliance gate has passed.
- The devil's-advocate review has been performed and its objections addressed.
- The roadmap items are prioritized by effort × impact and are actionable.
- Evidence hierarchy respected (systematic review > meta-analysis > RCT/standard > expert opinion > blog).

## Test Scenarios
1. **Whole-home overwhelm** — *User:* "My whole apartment is cluttered, where do I start?" → *Skill:* Selects method, builds room-by-room schedule sized to time budget. (**Gate:** Sessions sized to stated time.)
2. **Sentimental items** — *User:* "I can't let go of keepsakes" → *Skill:* Applies decision heuristics + memory-preservation tactics. (**Gate:** Emotional items handled with low-pressure rules.)
3. **Rebound clutter** — *User:* "I declutter but it comes back" → *Skill:* Designs one-in-one-out + habit-loop maintenance system. (**Gate:** Maintenance system included before completion.)
4. **Tiny space** — *User:* "I live in a studio" → *Skill:* Optimizes plan for small-space constraints. (**Gate:** Plan respects spatial limits.)
5. **Downsizing for a move** — *User:* "Moving to a smaller place in 4 weeks" → *Skill:* Builds deadline-driven, prioritized plan. (**Gate:** Plan fits the deadline.)

## Key Design Decisions
1. Research-first: no scored claim without a citation or explicit assumption.
2. Framework-grounded: scoring uses only the named world-renowned frameworks above.
3. Composable sub-skills (≥3) with explicit gates between stages.
4. Self-improving knowledge brain via the crawl pipeline.
5. Graceful degradation when WebSearch/WebFetch are unavailable.
