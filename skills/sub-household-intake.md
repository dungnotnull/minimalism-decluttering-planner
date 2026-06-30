---
name: minimalism-decluttering-planner__sub-household-intake
description: Sub-skill of minimalism-decluttering-planner — Capture rooms, clutter hotspots, household members, time budget, emotional-attachment items and goals.
---

## Purpose
Capture comprehensive household context through structured intake, enabling evidence-based decluttering method selection and roadmap generation. This sub-skill ensures no critical assumptions are made about the household situation before analysis proceeds.

## Inputs
- Direct user responses to intake questions
- Any pre-existing household context provided in initial request
- Relevant framework constraints from `SECOND-KNOWLEDGE-BRAIN.md`

## Core Intake Fields

### 1. Household Profile
- **Household type**: single individual, couple, family with children, multi-generational, shared housing
- **Total household members**: number and ages (relevant for item volume, safety, shared spaces)
- **Primary decision-maker**: who makes final keep/discard decisions (critical for execution)
- **Household agreement level**: all members aligned, partial alignment, conflict present (affects method selection)

### 2. Spatial Inventory
- **Dwelling type**: studio, 1-bedroom, 2-bedroom, house, multi-room space
- **Total square footage**: approximate (affects session sizing and storage capacity)
- **Rooms requiring decluttering**: list each room/space
- **Clutter hotspots**: specific problem areas identified by user (e.g., "kitchen counters", "bedroom closet floor")
- **Storage systems present**: closet organizers, shelving, bins, garage storage (affects method sequencing)

### 3. Clutter Assessment
For each room/hotspot, capture:
- **Clutter density score**: user self-assessment 1-10 (1=minimal, 10=overwhelming)
- **Primary clutter categories**: clothes, papers, sentimental items, hobbies, kitchen items, duplicates, "just in case" items, unfinished projects
- **Estimated item volume**: rough count (e.g., "200+ items in closet") or visual description
- **Last major declutter**: when space was last thoroughly cleared (affects rebound analysis)

### 4. Time & Resource Constraints
- **Available time per session**: minutes/hours user can dedicate (realistic, not aspirational)
- **Session frequency**: daily, weekly, bi-weekly, monthly (affects roadmap timeline)
- **Deadline constraints**: moving, selling, hosting events, lifestyle changes (affects prioritization)
- **Physical limitations**: mobility issues, health constraints (affects method safety and pacing)
- **Budget constraints**: can invest in storage solutions, need to donate/sell (affects disposal recommendations)

### 5. Emotional Attachment Profile
- **High-attachment categories**: items user struggles to release (sentimental, gifts, expensive purchases, aspirational items)
- **Emotional barriers identified**: guilt, "someday" thinking, loss aversion, identity attachment, inherited items
- **Past discard regret**: items previously discarded that user missed (informs tolerance thresholds)
- **Memory preservation tactics**: photography, digitization, memory boxing (already used or needed)

### 6. Goals & Success Criteria
- **Primary motivation**: why declutter now (moving, overwhelm, lifestyle change, mental clarity)
- **Success definition**: what "done" looks like (all surfaces clear, everything has a home, can find things in 30 seconds)
- **Maintenance aspiration**: want to maintain long-term vs. one-time project (affects habit system design)
- **Space usage vision**: how user wants to use each space (informs keep decisions)

### 7. Past Decluttering History
- **Previous attempts**: methods tried (KonMari, room-by-room, minimalist game, professional help)
- **What worked**: past successes to build on
- **What failed**: patterns of rebound, decision fatigue, abandonment points
- **Current pain points**: specific frustrations driving this request

## Intake Procedure

### Step 1: Request Classification
Parse the user's initial request to identify:
- **Trigger type**: overwhelm, specific problem area, maintenance failure, life transition
- **Urgency level**: immediate deadline vs. ongoing project vs. aspirational
- **Scope clarity**: specific room/space vs. whole-home vs. unclear

**Ask targeted questions for missing scope**:
- "Are you looking to declutter a specific room or your entire home?"
- "What's driving this now—a deadline, growing frustration, or lifestyle change?"
- "Have you tried decluttering before? What worked or didn't?"

### Step 2: Progressive Field Gathering
Collect the core intake fields through **targeted questions, not assumptions**:

**Start with household basics** (if not evident):
- "Who lives in your home and shares the items we'll be evaluating?"
- "What type of space are you working in—apartment, house, specific rooms?"

**Move to clutter assessment**:
- "Which rooms or areas feel most cluttered right now?"
- "On a scale of 1-10, how overwhelmed do you feel by each space?"

**Understand constraints**:
- "How much time can you realistically dedicate to decluttering per session?"
- "Any deadlines we should know about—moving, events, changes?"

**Probe emotional barriers** (if indicated):
- "Are there specific types of items you find hardest to let go of?"
- "Any past attempts to declutter that didn't stick? What happened?"

### Step 3: Validation & Normalization
For each field, apply validation rules:

**Completeness checks**:
- Household members: must have count and primary decision-maker
- Rooms: must have at least one specific space identified
- Time budget: must have realistic session duration and frequency
- Goals: must have at least one success criterion

**Consistency checks**:
- Square footage vs. room count (flag if unrealistic)
- Session time vs. clutter volume (flag mismatch)
- Deadline vs. scope (flag if timeline impossible)
- Household agreement vs. method suitability (warn if conflict likely)

**Normalization rules**:
- Time budgets: convert "whenever I can" to specific commitment
- Clutter density: normalize subjective descriptions to 1-10 scale
- Room names: standardize (e.g., "master bedroom closet" not "my closet")
- Item categories: map to KonMari categories where applicable

### Step 4: Framework Application Notes
Document which frameworks apply to this intake:

**KonMari applicability**:
- Category-based sequencing viable if household aligned on process
- "Spark joy" decision heuristic suitable if emotional attachment moderate
- Sequential room closure viable if household has control over shared spaces

**Minimalism applicability**:
- Essentialism framework relevant if user values reduction over organization
- "Just in case" patterns identified in intake → targeted intervention
- Accumulation prevention needed if past rebound noted

**Decision-rule applicability**:
- Four-box sorting viable if clutter density >5 (need structure)
- OHIO rules critical if user has limited time budget
- Decision fatigue indicated by past abandonment → need heuristics

**Habit-loop applicability**:
- Maintenance system required if "one-time project" not stated
- Cue-routine-reward design needed if rebound patterns identified
- One-in-one-out rules essential if storage capacity is limited

**Swedish death cleaning applicability**:
- Lifecycle awareness relevant if household includes aging members
- Downscaling indicated if moving to smaller space
- Legacy reduction relevant if inherited items prominent

### Step 5: Structured Output Generation
Produce a structured intake record for downstream processing:

```markdown
## Household Intake Profile

### Household Context
- Type: [single/couple/family/etc.]
- Members: [count with ages]
- Primary decision-maker: [who]
- Agreement level: [unified/partial/conflict]
- Dwelling: [type, square footage]

### Spatial Inventory
- Rooms requiring work: [list]
- Clutter hotspots: [prioritized list with 1-10 density scores]
- Storage systems: [present/absent, type]

### Clutter Assessment (by space)
- [Space name]: [density score], [primary categories], [item volume estimate]
- [Repeat for each space]

### Constraints
- Time per session: [duration]
- Session frequency: [daily/weekly/etc.]
- Deadlines: [specific dates or none]
- Physical limitations: [yes/no with details]
- Budget: [can invest in storage/break-even/none]

### Emotional Attachment Profile
- High-attachment categories: [list]
- Emotional barriers: [guilt/someday/loss aversion/etc.]
- Past discard regret: [yes/no with examples]
- Memory preservation needed: [yes/no, tactics]

### Goals & Success Criteria
- Primary motivation: [move/overwhel/lifestyle/etc.]
- Success definition: [specific measurable outcome]
- Maintenance aspiration: [long-term/one-time]
- Space usage vision: [how each space should function]

### Past History
- Previous attempts: [methods tried]
- What worked: [successes to build on]
- What failed: [patterns of rebound/abandonment]
- Current pain points: [specific frustrations]

### Framework Applicability Notes
- KonMari: [suitability assessment]
- Minimalism: [suitability assessment]
- Decision rules: [suitability assessment]
- Habit loops: [suitability assessment]
- Swedish death cleaning: [suitability assessment]

### Critical Assumptions (if any)
- [Any assumptions made due to missing input, explicitly stated]
```

## Quality Gates

### Gate 1: Completeness
- [ ] All 7 core intake field groups captured
- [ ] No critical missing fields (household members, rooms, time budget, goals)
- [ ] At least one specific space identified with clutter assessment
- [ ] Time budget is realistic (not "whenever I can")

### Gate 2: Consistency
- [ ] Square footage aligns with room count
- [ ] Session time aligns with clutter volume (flag if mismatched)
- [ ] Deadline vs. scope is feasible (warn if timeline impossible)
- [ ] Household agreement vs. method selection is compatible

### Gate 3: Evidence Linkage
- [ ] Framework applicability notes cite specific intake fields
- [ ] Method selection rationale references household context
- [ ] Emotional attachment recommendations link to identified barriers

### Gate 4: No Fabrication
- [ ] Missing inputs requested, not assumed
- [ ] Estimates labeled as estimates (not asserted as facts)
- [ ] User self-assessments preserved (not overridden)

## Output Downstream Uses

**To `sub-declutter-method-selector`**:
- Household type and agreement level → method selection (category vs. room-by-room)
- Clutter density scores → sequencing priority
- Time constraints → session sizing in roadmap
- Deadline constraints → method urgency factor

**To `sub-decision-engine`**:
- Emotional attachment profile → decision heuristic selection
- High-attachment categories → specialized handling rules
- Past discard regret → tolerance threshold calibration
- Memory preservation needs → tactics recommendation

**To `sub-maintenance-system`**:
- Past rebound patterns → maintenance habit design
- Storage capacity → one-in-one-out rule design
- Household member count → shared responsibility systems
- Maintenance aspiration → habit loop complexity

**To `sub-declutter-roadmap`**:
- Rooms and clutter density → session sequencing
- Time per session and frequency → realistic timeline
- Deadline constraints → prioritization adjustments
- Physical limitations → safety accommodations

## Example Intake Session

**User**: "My whole apartment is cluttered, where do I start?"

**Skill** (progressive intake):
1. "Let me understand your situation first. Who lives in your home and shares these items?"
2. "What type of space are you in—apartment, house, how many rooms?"
3. "Which rooms feel most cluttered right now? Rate each 1-10."
4. "How much time can you realistically dedicate per session?"
5. "Any deadlines or particular frustrations driving this now?"
6. "Are there types of items you've struggled to let go of before?"

[After responses, generates structured intake record as shown above]

## Edge Cases & Fallbacks

**User provides minimal information**:
- Ask targeted questions for each missing field group
- Do not proceed until minimum viable intake is complete
- Explicitly state what's needed before analysis can proceed

**User resists detailed intake**:
- Offer "quick-start" option: capture only rooms + time + goals
- Warn that reduced detail may affect recommendation quality
- Present trade-offs clearly

**Household disagreement on method**:
- Flag in intake record for downstream consideration
- Recommend conflict-resolution strategies in roadmap
- Adjust method selection to accommodate resistance

**Physical/health limitations**:
- Flag for safety accommodations in roadmap
- Adjust session sizing for fatigue management
- Recommend adaptive tools/techniques

**Extremely tight deadline**:
- Flag urgency in intake record
- Adjust method toward triage vs. comprehensive
- Warn about sustainability trade-offs
