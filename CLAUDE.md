# CLAUDE.md — Minimalism Decluttering Planner

**Skill name:** `minimalism-decluttering-planner`
**Source idea:** #195 (ideas.md)
**Cluster:** Lifestyle & Personal (`lifestyle-personal`)
**Tagline:** Plans and manages home decluttering with a staged method, decision criteria and habit systems to keep spaces minimal long-term.
**Current phase:** Phase 4 — Testing & Validation (initial build complete)

## Problem This Skill Solves
People start decluttering but stall from decision fatigue and rebound clutter. This skill builds a staged, room-by-room plan using recognized decluttering methods, decision heuristics, and habit-maintenance systems tailored to the household.

## Harness Flow Summary
1. **Intake** → `sub-household-intake` gathers structured inputs.
2. **Research / evidence sync** → consult `SECOND-KNOWLEDGE-BRAIN.md`; refresh via WebSearch/WebFetch when available.
3. **Gate** → requirement validation runs before analysis.
4. **Analysis / scoring** → `sub-declutter-method-selector` scores against the named frameworks.
5. **Challenge** → devil's-advocate review stress-tests assumptions and evidence.
6. **Synthesize** → `sub-maintenance-system` produces the scored deliverable + prioritized roadmap.

**Quality gate:** the devil's-advocate review (`sub` quality step) MUST pass before output; every scored claim must trace to a cited source or stated assumption.

## Sub-skills
- `skills/sub-household-intake.md` — Capture rooms, clutter hotspots, household members, time budget, emotional-attachment items and goals.
- `skills/sub-declutter-method-selector.md` — Select and sequence the appropriate method (KonMari category vs room-by-room) for the household.
- `skills/sub-decision-engine.md` — Apply decision heuristics to ambiguous items and reduce decision fatigue.
- `skills/sub-maintenance-system.md` — Design habit loops and one-in-one-out rules to prevent rebound clutter.
- `skills/sub-declutter-roadmap.md` — Produce a scheduled, room-by-room plan with realistic session sizing.

## Evaluation Frameworks (world-renowned, citable)
- **KonMari Method (Marie Kondo)** — Category-based tidying sequence with a keep/discard decision heuristic ('spark joy').
- **Minimalism (The Minimalists / Essentialism)** — Philosophy and decision frameworks for reducing to the essential and resisting accumulation.
- **Four-box / OHIO decision rules** — Operational sorting heuristics (keep/donate/trash/relocate; Only Handle It Once).
- **Habit loop (Atomic Habits / Fogg Behavior Model)** — Cue-routine-reward design for maintenance habits and one-in-one-out rules.
- **Swedish death cleaning (döstädning)** — Lifecycle-aware decluttering reducing future burden on others.

## Tools Required
- `WebSearch`, `WebFetch` — live evidence and trend updates (graceful degradation to the knowledge brain when unavailable).
- `Read`, `Write` — load the knowledge brain; emit the deliverable.
- `Bash` — run `tools/knowledge_updater.py` (crawl4ai pipeline).

## Knowledge Sources
- **ArXiv / academic categories:** cs.CY, econ.GN
- [Journal of Environmental Psychology](https://www.sciencedirect.com/journal/journal-of-environmental-psychology) — Research on clutter, well-being and space.
- [APPO (professional organizers)](https://www.napo.net/) — Professional decluttering standards.
- [Atomic Habits resources](https://jamesclear.com/) — Habit-formation frameworks.
- [The Minimalists](https://www.theminimalists.com/) — Minimalism methodology.
- [Behavioral science (BJ Fogg)](https://behaviormodel.org/) — Behavior-design model.

## Supporting Tools
- `tools/knowledge_updater.py` — crawl4ai + WebSearch pipeline that grows `SECOND-KNOWLEDGE-BRAIN.md` (recommended weekly cron).

## Active Development Tasks
- [x] Scaffold all required deliverables
- [x] Define frameworks, sub-skills and scoring dimensions
- [x] Author knowledge brain v1 and crawl pipeline
- [ ] Expand knowledge brain via first scheduled crawl
- [ ] Add adversarial/edge-case test scenarios beyond the initial 5

## Related Root Docs
- `PROJECT-detail.md` — full technical spec
- `PROJECT-DEVELOPMENT-PHASE-TRACKING.md` — phase roadmap
- `SECOND-KNOWLEDGE-BRAIN.md` — living domain knowledge base
