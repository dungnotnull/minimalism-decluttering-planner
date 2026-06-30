---
name: minimalism-decluttering-planner__sub-declutter-roadmap
description: Sub-skill of minimalism-decluttering-planner — Produce a scheduled, room-by-room plan with realistic session sizing.
---

## Purpose
Generate a realistic, achievable decluttering roadmap that translates method selection, decision heuristics, and maintenance systems into a concrete timeline with session-by-session action plans. This sub-skill ensures the plan fits household constraints while maximizing completion probability.

## Inputs
- **Intake record from `sub-household-intake`**: rooms, clutter density, time per session, frequency, deadlines, physical limitations
- **Method selection from `sub-declutter-method-selector`**: selected method, phases, sequencing
- **Decision heuristics from `sub-declutter-roadmap`**: decision framework per category
- **Maintenance system from `sub-maintenance-system`**: ongoing maintenance after roadmap completion

## Core Roadmap Principles

### Principle 1: Realistic Session Sizing
**Description**: Sessions must fit within stated time budget with buffer for fatigue.

**Evidence base**:
- Behavioral research: overestimation of capacity leads to abandonment
- Decluttering psychology: fatigue increases decision errors, resistance
- Project management: buffer time increases completion rates by 67%

#### Session Sizing Formula

**Base time calculation**:
```
Session scope (items or area) ÷ Processing rate × Decision complexity factor = Estimated time
Estimated time × 1.5 (buffer factor) = Realistic session time
```

**Processing rates** (average items per hour for typical household):
- **Low-attachment items** (clothes, kitchen tools): 40-60 items/hour
- **Medium-attachment items** (books, decor): 20-40 items/hour
- **High-attachment items** (sentimental, heirlooms): 5-15 items/hour
- **Complex decisions** (papers, photos): 10-20 items/hour

**Decision complexity factors**:
- **Low complexity** (obvious keep/discard): 1.0
- **Medium complexity** (some ambiguity): 1.5
- **High complexity** (emotional attachment): 2.5
- **Very high complexity** (grief items, inherited): 4.0

#### Buffer Guidelines
- **Standard buffer**: 1.5× estimated time (accounts for fatigue, distractions)
- **High-emotion buffer**: 2.0× estimated time (for sentimental categories)
- **First-session buffer**: 2.0× estimated time (learning curve, setup)
- **Physical limitation buffer**: 1.8× estimated time (mobility/energy constraints)

### Principle 2: Motivation-Sustaining Sequencing
**Description**: Order sessions to maximize early wins, build momentum, and prevent burnout.

**Evidence base**:
- Goal attainment research: early progress predicts completion
- Behavioral momentum: successes build motivation for continued effort
- Decluttering psychology: visible change reinforces continued participation

#### Sequencing Strategy

**Early-phase sequencing (sessions 1-3)**:
- **Target**: High-visual-impact, low-emotional-difficulty spaces
- **Examples**: Entryway, living room surfaces, bathroom countertops
- **Goal**: Visible progress, quick wins, confidence building
- **Success criteria**: User can see and feel difference immediately

**Mid-phase sequencing (sessions 4-8)**:
- **Target**: Moderate-difficulty spaces, core functional areas
- **Examples**: Kitchen cabinets, bedroom closets, home office
- **Goal**: Functional improvement, meaningful impact
- **Success criteria**: Space functions better daily

**Late-phase sequencing (sessions 9+)**:
- **Target**: High-difficulty, high-emotion categories
- **Examples**: Sentimental items, photos, heirlooms, memorabilia
- **Goal**: Completion of most difficult items, habit practice established
- **Success criteria**: All major categories processed

#### Motivation Maintenance

**Progress tracking embedded in roadmap**:
- **Session 1 milestone**: First space completed (celebrate)
- **Session 5 milestone**: Half of targeted spaces processed
- **Session completion milestone**: Final space/category done

**Visible progress documentation**:
- **Before/after photos**: Each session's space photographed
- **Item counts**: Track items removed per session
- **Time tracking**: Actual vs. estimated session times

### Principle 3: Deadline-Driven Prioritization
**Description**: When deadlines exist, roadmap prioritizes by deadline proximity and criticality.

**Evidence base**:
- Time management research: deadline proximity drives action prioritization
- Project management: critical path analysis identifies high-impact tasks
- Behavioral research: urgency increases but doesn't guarantee completion

#### Deadline Handling Protocol

**Urgent deadline (≤4 weeks)**:
1. **Prioritize by deadline-critical spaces**: Rooms/items involved in deadline event
2. **Triage mode**: Process only deadline-critical items first, defer non-critical
3. **Extended sessions**: Schedule longer or more frequent sessions within energy limits
4. **Accept trade-offs**: May need to defer non-deadline spaces to post-deadline phase

**Moderate deadline (1-3 months)**:
1. **Standard sequencing with deadline check-ins**: Regular assessment of progress vs. timeline
2. **Buffer sessions**: Schedule 1-2 bonus sessions for unexpected slowdowns
3. **Scope flexibility**: If behind, adjust scope (fewer items per session) not timeline

**No deadline**:
1. **Quality-over-speed focus**: Optimize for thoroughness, not speed
2. **Sustainable pacing**: Sessions sized to prevent burnout, maintain motivation
3. **Enjoyment integration**: Make process pleasant, not rushed

### Principle 4: Physical & Cognitive Capacity Respect
**Description**: Roadmap respects household's physical limitations and cognitive capacity.

**Evidence base**:
- Health psychology: pacing prevents injury and exhaustion
- Cognitive load research: decision fatigue degrades choices after extended sessions
- Decluttering safety: overexertion leads to abandonment and injury

#### Capacity-Based Adjustments

**Physical limitations**:
- **Mobility limitations**: Prefer horizontal processing (one area) over vertical (multiple rooms)
- **Energy limitations**: Shorter sessions (15-30 minutes) more frequently
- **Pain conditions**: Avoid bending, reaching heavy use; schedule rest breaks

**Cognitive limitations**:
- **Decision fatigue**: Schedule sessions during high-energy times of day
- **ADHD/executive function**: Shorter sessions, more frequent, external accountability
- **Anxiety/overwhelm**: Smaller scope sessions, more rest between

**Adjustment guidelines**:
- **Standard capacity**: 60-90 minute sessions, 2-3× per week
- **Reduced capacity**: 30-45 minute sessions, daily or every other day
- **Severe limitations**: 15-20 minute sessions, daily, micro-focused scope

## Roadmap Structure

### Phase 1: Preparation (Session 0)
**Duration**: 30-60 minutes
**Purpose**: Setup, supply gathering, space preparation

**Session 0 Tasks**:
1. **Supply setup** (15 minutes):
   - Acquire boxes/bags for sorting (keep, donate, trash, relocate)
   - Labels for boxes
   - Timer for decision-making
   - Cleaning supplies (for emptying spaces)

2. **Space preparation** (15-30 minutes):
   - Clear workspace in each area to be decluttered
   - Remove obvious trash first (quick win)
   - Set up donation box in permanent location
   - Identify "staging area" for keep items

3. **System setup** (15 minutes):
   - Setup tracking system (notebook, app, spreadsheet)
   - Review decision heuristics (have reference available)
   - Schedule first decluttering session
   - Inform household members of plan

**Success criteria**: All supplies ready, first session scheduled, household informed

### Phase 2: Implementation (Sessions 1-N)

#### Session Template

**Session Structure** (60-minute example):
- **0-5 minutes**: Setup, review decision heuristics, set timer
- **5-50 minutes**: Item processing (apply four-box/OHIO method)
- **50-55 minutes**: Box review (quick check for mis-sorted items)
- **55-60 minutes**: Cleanup, photograph progress, log stats

**Session Post-Processing**:
- **Empty boxes**: Donate to car, trash to outside, relocate items to homes
- **Update tracking**: Log items processed, time taken, observations
- **Celebrate**: Acknowledge completion, note progress visible
- **Schedule next**: Put next session on calendar before ending current

#### Session Examples

**Session 1: Entryway & Drop Zones**
- **Scope**: Entry table, coat area, shoe storage, mail surface
- **Estimated time**: 45 minutes × 1.5 (first-session buffer) = 67 minutes → 70 minutes
- **Target items**: 50-80 items
- **Decision complexity**: Low (mostly obvious keep/discard)
- **Success criteria**: All surfaces 80% clear, donation box full

**Session 2: Living Room Flat Surfaces**
- **Scope**: Coffee table, end tables, entertainment center surfaces
- **Estimated time**: 60 minutes × 1.5 (buffer) = 90 minutes
- **Target items**: 40-60 items
- **Decision complexity**: Low-Medium (some decor decisions)
- **Success criteria**: All surfaces clear, decor curated (≤3 items per surface)

**Session 3: Bathroom Countertops & Storage**
- **Scope**: Countertops, medicine cabinet, under-sink storage
- **Estimated time**: 45 minutes × 1.5 (buffer) = 67 minutes → 70 minutes
- **Target items**: 60-100 items (mostly small items)
- **Decision complexity**: Low (expiration dates clear criteria)
- **Success criteria**: Countertops clear, expired products removed

**Session 4: Kitchen Surfaces**
- **Scope**: Countertops, kitchen table, appliance storage
- **Estimated time**: 60 minutes × 1.5 (buffer) = 90 minutes
- **Target items**: 50-80 items
- **Decision complexity**: Medium (some appliance decisions)
- **Success criteria**: All surfaces clear, only daily-use items out

**Session 5-6: Bedroom Clothing - Category Pass 1**
- **Scope**: All clothing in home (KonMari style) or primary closet (room-by-room)
- **Estimated time**: 90-120 minutes × 1.5 (high-emotion buffer) = 135-180 minutes
- **Split across 2 sessions**: 70-90 minutes each
- **Target items**: 150-300 items
- **Decision complexity**: Medium-High (emotional attachment, identity items)
- **Success criteria**: All clothing processed, donation pile ready, closet organized

**Session 7-8: Papers & Mail**
- **Scope**: All accumulated papers, mail, documents
- **Estimated time**: 60 minutes × 1.5 (buffer) = 90 minutes per session
- **Target items**: 100-200 items
- **Decision complexity**: High (anxiety-provoking for many)
- **Success criteria**: All papers processed (file/shred/recycle), mail system established

**Session 9: Books & Media**
- **Scope**: All books, DVDs, magazines, media
- **Estimated time**: 60 minutes × 1.5 (buffer) = 90 minutes
- **Target items**: 50-150 items
- **Decision complexity**: Medium (identity attachment, aspirational reading)
- **Success criteria**: All books processed, donation pile ready, bookshelf organized

**Session 10-11: Kitchen Cabinets & Pantry**
- **Scope**: Food storage, appliances, dishes, cookware
- **Estimated time**: 90 minutes × 1.5 (buffer) = 135 minutes → split across 2 sessions
- **Target items**: 100-200 items
- **Decision complexity**: Medium (duplicate items, aspirational appliances)
- **Success criteria**: Expired food removed, duplicates consolidated, appliances evaluated

**Session 12-13: Bathroom Storage & Linens**
- **Scope**: Toiletries, towels, linens, cleaning supplies
- **Estimated time**: 60 minutes × 1.5 (buffer) = 90 minutes per session
- **Target items**: 80-150 items
- **Decision complexity**: Low-Medium (expiration dates, usage clarity)
- **Success criteria**: Expired products removed, linens organized, supplies consolidated

**Session 14-15: Sentimental Items**
- **Scope**: Photos, memorabilia, heirlooms, gifts
- **Estimated time**: 60 minutes × 2.0 (high-emotion buffer) = 120 minutes per session
- **Target items**: 30-80 items
- **Decision complexity**: Very High (emotional difficulty)
- **Success criteria**: All sentimental items processed, memory preservation tactics applied

**Session 16: Final Review & System Check**
- **Scope**: Walk-through of all spaces, identify remaining problem areas
- **Estimated time**: 60 minutes
- **Target items**: N/A (review, not processing)
- **Decision complexity**: N/A (assessment)
- **Success criteria**: All spaces reviewed, final adjustments made, maintenance system confirmed

### Phase 3: Maintenance Integration (Ongoing)
**Timing**: Begins after final decluttering session
**Purpose**: Transition from project to ongoing habits

**Maintenance Integration Tasks**:
1. **Maintenance habit launch** (Week 1 post-roadmap):
   - Begin daily micro-habits
   - Schedule first weekly maintenance session
   - Setup one-in-one-out tracking

2. **System verification** (Week 2 post-roadmap):
   - Verify all storage systems working
   - Adjust systems that aren't functioning
   - Confirm household members using systems

3. **Progress celebration** (Week 4 post-roadmap):
   - Photograph all maintained spaces
   - Count total items removed
   - Celebrate milestone

## Roadmap Customization Factors

### Small Space Roadmap (Studio/1-Bedroom)
**Characteristics**: Limited storage, high visual impact, rapid processing

**Roadmap adaptations**:
- **Fewer sessions**: 8-10 sessions vs. 16 for larger home
- **Smaller scope per session**: Can process multiple categories per session
- **Faster completion**: 2-4 weeks total timeline
- **Stricter one-in-one-out**: Essential for small space maintenance

### Large Space Roadmap (3+ Bedrooms)
**Characteristics**: Hidden clutter possible, multiple rooms, extended timeline

**Roadmap adaptations**:
- **More sessions**: 18-24 sessions
- **Room-by-room sequencing**: Complete one room before moving to next
- **Longer timeline**: 8-12 weeks total
- **Hidden space focus**: Closets, storage areas, garage require dedicated sessions

### High-Clutter Roadmap (Density 7-10)
**Characteristics**: Overwhelm risk, decision fatigue, physical exhaustion

**Roadmap adaptations**:
- **Smaller scope sessions**: 45-60 minutes maximum
- **Higher session frequency**: Daily or every other day for momentum
- **Extended timeline**: 12-16 weeks to prevent burnout
- **Professional support recommended**: Consider organizer for high-emotion categories

### Deadline-Driven Roadmap (≤4 Weeks)
**Characteristics**: Urgency, pressure, potential for burnout

**Roadmap adaptations**:
- **Triage sequencing**: Deadline-critical spaces first
- **Extended sessions**: 90-120 minutes when energy allows
- **High frequency**: Daily sessions or twice daily when possible
- **Accept imperfect completion**: Post-deadline phase for non-critical spaces

## Output Structure

### Decluttering Roadmap Report

```markdown
## Decluttering Roadmap

### Roadmap Overview
**Method**: [selected method]
**Total timeline**: [X weeks, Y sessions]
**Session frequency**: [X times per week]
**Estimated completion**: [date]
**Deadline alignment**: [on track / accelerated / extended from deadline]

### Session Schedule

#### Session 0: Preparation [Date, Time]
- **Duration**: [X minutes]
- **Tasks**: [supply setup, space preparation, system setup]
- **Success criteria**: [what marks completion]

#### Session 1: [Space Name] [Date, Time]
- **Duration**: [X minutes] (estimated: [Y minutes] × [buffer factor])
- **Scope**: [specific space and item categories]
- **Target items**: [estimated number]
- **Decision complexity**: [Low/Medium/High]
- **Decision heuristics**: [which framework to apply]
- **Success criteria**: [what marks completion]
- **Notes**: [special considerations for this session]

#### Session 2: [Space Name] [Date, Time]
[repeat structure for all sessions]

### Timeline Visualization

**Week 1**:
- Session 0: Preparation
- Session 1: [Space]
- Session 2: [Space]

**Week 2**:
- Session 3: [Space]
- Session 4: [Space]

[Continue for all weeks]

### Capacity Adjustments
- **Physical considerations**: [how roadmap accommodates limitations]
- **Cognitive considerations**: [session sizing for decision fatigue]
- **Energy management**: [rest periods, high-energy timing]
- **Household coordination**: [how members participate]

### Deadline Management
- **Primary deadline**: [date, if applicable]
- **Critical path**: [deadline-critical sessions]
- **Contingency**: [what if timeline slips]
- **Post-deadline phase**: [deferred sessions, if applicable]

### Progress Tracking
- **Session metrics**: [time taken, items processed, decision difficulty]
- **Cumulative metrics**: [total items removed, total time invested]
- **Visual documentation**: [before/after photo schedule]

### Quality Gates
- [ ] Every session sized within stated time budget
- [ ] Total timeline aligns with deadline (if applicable)
- [ ] Physical limitations accommodated
- [ ] Decision fatigue prevention included
- [ ] Success criteria measurable for each session
```

## Quality Gates

### Gate 1: Timeline Realism
- [ ] Every session duration fits within stated time budget
- [ ] Total timeline achievable with stated session frequency
- [ ] Buffer time included for fatigue, unexpected complications
- [ ] First session includes learning curve buffer

### Gate 2: Deadline Alignment
- [ ] Roadmap completion date meets or precedes deadline (if applicable)
- [ ] Critical path sessions prioritized when deadline present
- [ ] Contingency plan specified for timeline slippage
- [ ] Post-deadline phase planned for non-critical spaces (if applicable)

### Gate 3: Capacity Respect
- [ ] Physical limitations accommodated in session design
- [ ] Decision fatigue prevented through session sizing and breaks
- [ ] Energy management included in schedule
- [ ] Household coordination specified

### Gate 4: Measurable Success Criteria
- [ ] Every session has specific, measurable completion criteria
- [ ] Progress tracking defined (item counts, time, photos)
- [ ] Milestone celebrations included
- [ ] Final review session scheduled

### Gate 5: Maintenance Integration
- [ ] Maintenance habits scheduled to begin after roadmap completion
- [ ] System verification included in post-roadmap plan
- [ ] One-in-one-out rules integrated into ongoing routine
- [ ] Progress celebration planned

## Downstream Integration

**To main harness output**:
- Roadmap timeline → final report's implementation plan
- Session details → final report's step-by-step guidance
- Progress tracking → final report's success metrics
- Maintenance integration → final report's sustainability section
