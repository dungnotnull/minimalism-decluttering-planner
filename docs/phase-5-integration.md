# Phase 5 Integration & Cross-Skill Wiring

**Minimalism Decluttering Planner** — Integration with Lifestyle & Personal Cluster

## Overview

This document defines the shared interfaces, reusable patterns, and integration protocols for the `minimalism-decluttering-planner` skill within the `lifestyle-personal` cluster. These standards enable sibling skills to reuse intake patterns, scoring frameworks, and maintenance systems without duplication.

---

## Cluster Definition: Lifestyle & Personal

### Cluster Members (Current and Planned)
1. **`minimalism-decluttering-planner`** (idea #195) — Plans and manages home decluttering
2. **`habit-building-coach`** (future) — Builds and tracks personalized habit formation
3. **`wellness-routine-optimizer`** (future) — Designs daily routines for physical and mental health
4. **`personal-budget-optimizer`** (future) — Analyzes spending and recommends reductions
5. **`time-management-system`** (future) — Creates personalized scheduling and productivity systems

### Shared Domain Concepts
- **Behavior change**: All skills involve helping users change ingrained behaviors
- **Goal setting**: All skills require clarifying aspirations and success criteria
- **Habit formation**: All skills benefit from sustainable habit systems
- **Progress tracking**: All skills need motivation through visible progress
- **Maintenance design**: All skills must address relapse/rebound prevention

---

## Shared Sub-Skill Interfaces

### Interface 1: Universal Intake Schema

**Purpose**: Standardized intake fields common across all lifestyle-personal skills.

**Core Field Groups** (required for all cluster skills):

#### FG1: User Profile
- **Household type**: single, couple, family, multi-generational
- **Primary stakeholder**: who benefits from the intervention
- **Decision authority**: who has control over changes
- **Household alignment**: level of agreement on desired change

#### FG2: Current State Assessment
- **Baseline metric**: quantitative measure of current state (e.g., clutter density 1-10)
- **Problem areas**: specific spaces/aspects causing difficulty
- **Past attempts**: what user has tried before, what worked/failed
- **Current pain points**: specific frustrations driving the request

#### FG3: Goal Definition
- **Primary motivation**: why this change now (deadline, life transition, overwhelm)
- **Success criteria**: measurable definition of "done"
- **Aspiration level**: one-time fix vs. sustainable lifestyle change
- **Vision statement**: how user wants to feel/function after change

#### FG4: Constraints & Resources
- **Time budget**: available time per session/week
- **Frequency capability**: how often user can engage with process
- **Deadline constraints**: any time pressure (moving, events, transitions)
- **Physical limitations**: mobility, energy, cognitive constraints
- **Budget**: financial resources available for tools/solutions

#### FG5: Barriers & Resistance
- **Emotional barriers**: anxiety, guilt, attachment, identity issues
- **Cognitive barriers**: decision fatigue, overwhelm, executive function
- **Environmental barriers**: space limitations, other people's stuff, structural constraints
- **Past failures**: patterns of abandonment, rebound, resistance

#### FG6: Learning Style & Preferences
- **Information processing**: visual, auditory, kinesthetic
- **Decision style**: analytical, intuitive, somatic, collaborative
- **Motivation type**: internal (values) vs. external (deadlines, accountability)
- **Feedback needs**: progress tracking, celebration preferences

#### FG7: Maintenance Readiness
- **Past maintenance experience**: what systems have worked or failed
- **Habit existing foundation**: any existing habits to build on
- **Support system**: available accountability partners, professional help
- **Long-term commitment**: stated intention for ongoing change vs. one-time fix

**Implementation note**: All cluster skills MUST collect these 7 field groups. Skills may add skill-specific fields after these core groups.

---

### Interface 2: Scoring Framework Standard

**Purpose**: Common scoring dimensions applicable across lifestyle-personal skills.

#### Dimension Template

**Each skill defines 6-8 dimensions, each scored 0-100, following this structure**:

**Dimension Name**: [Clear, concise label]
- **What it measures**: [What aspect of user situation this dimension assesses]
- **Scoring criteria**:
  - **100 points**: [Ideal state, evidence-based benchmark]
  - **75 points**: [Good state with minor gaps]
  - **50 points**: [Moderate state, needs significant work]
  - **25 points**: [Poor state, major challenges]
  - **0 points**: [Critical state, fundamental blocker]
- **Weight in composite score**: [0.05-0.30, total weights sum to 1.0]
- **Evidence base**: [Research/framework supporting this dimension]
- **Household factors**: [Which intake fields affect this score]

**Composite score calculation**: Weighted sum of dimension scores.

**Confidence level**: High/Moderate/Low based on:
- Completeness of intake data
- Strength of evidence base
- Level of assumption required

---

### Interface 3: Habit Loop Design Pattern

**Purpose**: Standard habit loop structure for maintenance systems across cluster.

**Habit Loop Template**:

```markdown
### Habit: [Habit Name]

**Purpose**: [What this habit accomplishes in maintenance system]

**Cue (Trigger)**:
- **Type**: [Time-based / Context-based / Action-based]
- **Specific trigger**: [Exact time, situation, or preceding action]
- **Reliability**: [How consistent this cue occurs in daily life]

**Routine (Behavior)**:
- **Specific action**: [Exact behavior, not ambiguous]
- **Duration**: [How long the behavior takes]
- **Complexity**: [Simple/Moderate/Complex - affects adherence]

**Reward (Reinforcement)**:
- **Immediate reward**: [Intrinsic satisfaction or external marker]
- **Delayed reward**: [Long-term benefit or milestone celebration]
- **Identity reinforcement**: [How this habit expresses desired identity]

**Implementation Protocol**:
1. **Week 1-2**: [Startup phase, what to do to establish habit]
2. **Week 3-4**: [Consolidation phase, how to strengthen habit]
3. **Month 2**: [Integration phase, how to make habit automatic]
4. **Ongoing**: [Maintenance phase, how to sustain long-term]

**Quality Gates**:
- [ ] Cue occurs reliably in user's environment
- [ ] Routine fits within stated time/cognitive capacity
- [ ] Reward provides immediate reinforcement
- [ ] Implementation protocol allows gradual strengthening
```

**Shared Habit Library** (available to all cluster skills):

**Daily Micro-Habits** (<5 minutes):
- Morning intention setting
- Evening progress reflection
- Micro-session on target behavior (2-3 minutes)

**Weekly Maintenance Sessions** (15-30 minutes):
- Weekly review and planning
- Progress tracking and adjustment
- System troubleshooting

**Monthly Reviews** (30-60 minutes):
- Goal progress assessment
- System effectiveness review
- Adjustment and optimization

---

### Interface 4: Maintenance System Pattern

**Purpose**: Standard maintenance system design for all cluster skills.

**Maintenance System Template**:

```markdown
## Maintenance System Design

### System Overview
**Maintenance aspiration level**: [minimal care / sustainable systems / lifestyle integration]
**Primary maintenance framework**: [Habit loops / Environmental design / Scheduling / Accountability]
**Evidence base**: [Cited frameworks and research]

### Habit-Based Maintenance
[Implement Interface 3: Habit Loop Design Pattern for 3-5 core habits]

### Environmental Design Interventions
**Strategy 1**: [Cue enhancement - making desired behavior easy]
- **Implementation**: [Specific changes to physical/digital environment]
- **Evidence**: [Environmental psychology or nudge theory research]

**Strategy 2**: [Friction enhancement - making undesired behavior hard]
- **Implementation**: [Specific barriers to undesired behaviors]
- **Evidence**: [Friction research or behavioral economics]

### Scheduling & Accountability
**Maintenance frequency**: [Daily/weekly/monthly requirements]
**Tracking method**: [How user monitors adherence]
**Accountability system**: [External support, progress sharing, professional help]

### Relapse/Rebound Prevention
**High-risk scenarios**: [Specific situations likely to trigger regression]
**Prevention protocols**: [What to do in each high-risk scenario]
**Recovery planning**: [How to return to baseline after lapse]

### Implementation Timeline
**Week 1-2**: [Foundation setup]
**Week 3-6**: [Habit establishment]
**Month 2-3**: [System integration]
**Month 4+**: [Ongoing maintenance with quarterly reviews]
```

---

### Interface 5: Roadmap Generation Pattern

**Purpose**: Standard roadmap structure for all cluster skills.

**Roadmap Template**:

```markdown
## Implementation Roadmap

### Roadmap Overview
**Method/Approach**: [Selected intervention strategy]
**Total timeline**: [X weeks, Y sessions]
**Session frequency**: [X times per week]
**Estimated completion**: [date]

### Phase 1: Foundation [Week 1]
**Session 0: Preparation** [Duration]
- **Tasks**: [Supply setup, environment preparation, baseline measurement]
- **Success criteria**: [What marks completion]

### Phase 2: Core Intervention [Weeks 2-N]
**Session 1: [Focus Area]** [Date, Time, Duration]
- **Scope**: [Specific target]
- **Target metrics**: [Expected outcomes]
- **Decision/action framework**: [Rules/heuristics to apply]
- **Success criteria**: [Measurable completion]
- **Notes**: [Special considerations]

[Continue sessions...]

### Phase 3: Integration & Maintenance [Month 2+]
**Ongoing tasks**: [What continues after roadmap completion]
**Maintenance habits**: [Link to maintenance system]
**Review cadence**: [How often to assess and adjust]

### Capacity Adjustments
- **Time constraints**: [How roadmap accommodates limited time]
- **Cognitive capacity**: [Session sizing for mental energy]
- **Physical limitations**: [Accommodations for mobility/health]
- **Household coordination**: [How others participate]

### Timeline Visualization
[Week-by-week breakdown showing sessions and milestones]
```

---

## Reusable Components from Minimalism Decluttering Planner

### Component 1: Decision Heuristics Engine

**Reusable for**: Any skill requiring decision frameworks (budgeting, habit selection, prioritization)

**Core structure**:
- Universal decision tree (applicable to any item/choice)
- Category-specific decision flows
- Decision fatigue management protocol
- Special category handling (gifts, emotional items, aspirational choices)

**Adaptation for other skills**:
- **Budget optimizer**: Replace "keep/donate" with "spend/save"; categories become budget categories
- **Habit builder**: Replace "keep/donate" with "adopt/skip"; categories become habit types
- **Time management**: Replace "keep/donate" with "schedule/delegate"; categories become task types

### Component 2: One-In-One-Out Rule System

**Reusable for**: Any skill addressing resource management (budget, time, energy)

**Core structure**:
- Standard rule: For every addition, one subtraction
- Strict rule: For every addition, two subtractions (for reduction phase)
- Category-specific adaptations
- Purchase/entry decision protocols
- Tracking systems

**Adaptation for other skills**:
- **Budget optimizer**: One-in-one-out for spending categories (buy clothes, donate one)
- **Habit builder**: One-in-one-out for habit slots (adopt new habit, release one)
- **Time management**: One-in-one-out for commitments (accept new project, decline one)

### Component 3: Progress Tracking & Motivation System

**Reusable for**: All skills requiring sustained engagement

**Core structure**:
- Session-by-session metrics (time, items processed, decisions made)
- Cumulative metrics (total volume reduced, time invested)
- Visual documentation (before/after photos, progress charts)
- Milestone celebrations (specific points to acknowledge progress)
- Motivation maintenance strategies (what to do when energy flags)

**Adaptation for other skills**:
- **Habit builder**: Track habit consistency, streak length, automaticity progression
- **Budget optimizer**: Track spending reduction, savings accumulation, debt payoff
- **Time management**: Track productive hours, distraction reduction, goal completion

### Component 4: Devil's Advocate Review Protocol

**Reusable for**: All skills producing scored or analytical outputs

**Core structure**:
1. Identify weakest assumptions
2. Challenge each dimension with counter-evidence
3. Seek disconfirming evidence (via WebSearch when available)
4. Adjust scores downward when uncertainty high
5. Document challenges and resolutions

**Adaptation for other skills**:
- Apply to any scoring system (budget health, habit strength, time efficiency)
- Apply to any recommendation (which habits to build, which expenses to cut)
- Apply to any roadmap (is this timeline realistic? are these priorities correct?)

---

## Integration Examples

### Example 1: Habit-Building Coach Reusing Intake Schema

**Habit-Building Coach** intake would use the Universal Intake Schema with skill-specific additions:

**Core FG1-FG7**: Identical to decluttering planner
**FG8 (Habit-Specific)**: Target behaviors, desired habit outcomes, current habit patterns

**Benefit**: No need to redesign intake structure; proven field groups work; cluster consistency.

### Example 2: Budget Optimizer Reusing Decision Engine

**Budget Optimizer** would adapt the Decision Heuristics Engine:

**Universal decision tree**: Adapt "keep/donate" → "spend/cut"
**Category-specific flows**: Adapt "clothes, books, papers" → "groceries, dining, entertainment, subscriptions"
**Decision fatigue protocol**: Identical structure, applied to spending decisions
**Special category handling**: Adapt "gifts, heirlooms" → "gift spending, aspirational subscriptions"

**Benefit**: Decision fatigue management proven; habit loop structure accelerates learning.

### Example 3: Time Management Reusing Maintenance System

**Time Management** would adapt the Maintenance System Pattern:

**Habit loops**: Daily planning, weekly review, quarterly reset
**Environmental design**: Calendar setup, notification management, focus environment
**Relapse prevention**: Distraction scenarios, overload scenarios, vacation disruptions
**Implementation timeline**: Foundation → Core habits → Advanced systems

**Benefit**: Maintenance system design proven; relapse prevention applicable to time like clutter.

---

## Cluster-Wide Quality Standards

### Standard 1: Evidence-Based Recommendations
- All material claims cite sources or state assumptions
- Evidence hierarchy respected (systematic review > meta-analysis > RCT > standard > expert opinion)
- Confidence levels disclosed when uncertainty present

### Standard 2: Household-Specific Adaptation
- Recommendations adapted to household profile from intake
- Constraints (time, budget, physical limitations) respected
- No one-size-fits-all solutions without adaptation notes

### Standard 3: Implementation Feasibility
- Roadmaps realistic for stated constraints
- Daily/weekly habits fit within time/cognitive capacity
- Environmental changes achievable (not full remodel)

### Standard 4: Relapse/Rebound Prevention
- All skills identify high-risk scenarios for regression
- Prevention protocols specified for each risk
- Recovery plans outlined for system breakdowns

### Standard 5: Quality Gates Enforcement
- All gates documented and checked before output
- No output path bypasses validation
- Devil's advocate review performed on analytical outputs

---

## Future Cluster Integration Points

### Integration Point 1: Shared Knowledge Brain
**Opportunity**: Create cluster-wide knowledge brain with cross-domain research
**Content**: Behavior change, habit formation, decision fatigue, motivation research
**Benefit**: All skills access same evidence base; reduced duplication

### Integration Point 2: Cross-Skill Progress Tracking
**Opportunity**: Unified dashboard showing progress across lifestyle domains
**Content**: Clutter reduction, habit consistency, spending reduction, time efficiency
**Benefit**: User sees holistic lifestyle improvement; skills reinforce each other

### Integration Point 3: Master Maintenance System
**Opportunity**: Unified maintenance system that integrates habits from all skills
**Content**: Daily habits that address clutter, budget, time, wellness together
**Benefit**: Reduced cognitive load; integrated lifestyle design

---

## Implementation Status

**Current Phase**: Phase 5 — Integration & Cross-Skill Wiring

**Completed**:
- [✓] Universal Intake Schema defined (7 field groups)
- [✓] Scoring Framework Standard specified
- [✓] Habit Loop Design Pattern documented
- [✓] Maintenance System Pattern specified
- [✓] Roadmap Generation Pattern standardized
- [✓] Reusable Components identified
- [✓] Integration Examples documented
- [✓] Cluster-Wide Quality Standards defined

**Pending** (awaiting sibling skills):
- [ ] Shared Knowledge Brain implementation
- [ ] Cross-Skill Progress Tracking system
- [ ] Master Maintenance System integration
- [ ] Cluster testing with multiple skills

**Success criteria**:
- Sibling skills can reuse intake schemas without modification
- Scoring frameworks applicable across domains with dimension adaptation
- Habit patterns transferable between skills
- Maintenance systems consistent in structure
- Quality gates enforce cluster standards

---

## Conclusion

The Minimalism Decluttering Planner establishes integration standards for the lifestyle-personal cluster. By defining shared interfaces for intake, scoring, habits, maintenance, and roadmaps, sibling skills can adopt proven patterns without reinvention. This accelerates skill development, improves consistency, and enables cross-skill synergies that enhance user outcomes.

**Phase 5 Status**: ✅ Complete (standards defined; awaiting sibling skills for implementation testing)
