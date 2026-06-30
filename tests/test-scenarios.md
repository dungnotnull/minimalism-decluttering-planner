# tests/test-scenarios.md — Minimalism Decluttering Planner

Scenario-based tests for `minimalism-decluttering-planner` (idea #195). Production-grade test suite with detailed walkthroughs, input/output validation, and edge case coverage.

---

## Scenario 1: Whole-Home Overwhelm

### User Input
**Initial request**: "My whole apartment is cluttered, where do I start?"

### Intake Session Walkthrough

**Skill questions** (progressive intake):
1. "Let me understand your situation first. Who lives in your home and shares these items?"
   - **User response**: "Just me, in a 2-bedroom apartment, about 1,200 sq ft."

2. "Which rooms or areas feel most cluttered right now? Rate each 1-10."
   - **User response**: "Living room 8, bedroom 7, kitchen 6, second bedroom/office 9"

3. "How much time can you realistically dedicate to decluttering per session?"
   - **User response**: "Maybe an hour on weekends, so 4-5 hours total per month"

4. "Any deadlines or particular frustrations driving this now?"
   - **User response**: "No deadline, just feeling overwhelmed and anxious about the mess"

5. "Are there types of items you find hardest to let go of?"
   - **User response**: "Clothes I might wear someday, books I haven't read yet"

### Structured Intake Output

**Household Context**:
- Type: Single-person household
- Members: 1
- Primary decision-maker: User
- Agreement level: Unified (only one person)
- Dwelling: 2-bedroom apartment, 1,200 sq ft

**Spatial Inventory**:
- Rooms requiring work: Living room, bedroom, kitchen, second bedroom/office
- Clutter hotspots (by density):
  - Second bedroom/office: 9/10 (highest)
  - Living room: 8/10
  - Bedroom: 7/10
  - Kitchen: 6/10

**Clutter Assessment**:
- Primary clutter categories: Clothes, books, papers, miscellaneous items
- Estimated volume: 800-1,200 items across all spaces
- Last major declutter: Never (first time)

**Constraints**:
- Time per session: 60 minutes
- Session frequency: Weekly (4-5 sessions per month)
- Deadlines: None
- Physical limitations: None stated
- Budget: Can invest in basic storage solutions

**Emotional Attachment Profile**:
- High-attachment categories: Clothes (aspirational), books (aspirational)
- Emotional barriers: "Someday" thinking, loss aversion
- Past discard regret: None stated
- Memory preservation needs: None stated

**Goals & Success Criteria**:
- Primary motivation: Overwhelm, anxiety reduction
- Success definition: Can relax in living spaces; can find things when needed
- Maintenance aspiration: Long-term clutter-free living
- Space usage vision: Living room for relaxing, bedroom for sleeping, office for work

### Method Selection Analysis

**KonMari Category-Based**: Score 72/100
- Household alignment: 85/100 (unified household, ideal for category method)
- Clutter profile fit: 65/100 (moderate-high clutter, some spaces very dense)
- Time constraint alignment: 60/100 (category method takes longer initially)
- Psychological readiness: 70/100 (motivated but some anxiety)
- Maintenance compatibility: 80/100 (high long-term sustainability)

**Room-by-Room**: Score 68/100
- Household alignment: 85/100 (suitable for single-person)
- Clutter profile fit: 75/100 (good for visible progress in dense spaces)
- Time constraint alignment: 75/100 (faster early wins)
- Psychological readiness: 70/100 (motivated)
- Maintenance compatibility: 65/100 (good but less comprehensive than KonMari)

**Selected**: Room-by-room with KonMari-style decision heuristics
**Rationale**: User needs visible progress quickly (overwhelm) → room-by-room provides early wins. KonMari decision heuristics (spark joy for clothes, essentialism for books) handle aspirational attachment.

### Expected Output Structure

**Summary & Headline Score**:
- Composite score: 65/100 (moderate clutter, decision fatigue from aspirational items)
- Confidence: Moderate (some uncertainty about emotional attachment depth)
- Timeline: 12 weeks (12 sessions)

**Dimension Scores**:
- Clutter density baseline: 75/100 (moderate-high density, 800-1,200 items)
- Decision-rule clarity: 50/100 (low clarity, aspirational "someday" items)
- Plan realism: 80/100 (timeline fits time budget; no deadline pressure)
- Maintenance-habit strength: 40/100 (no current maintenance systems)
- Emotional-attachment handling: 60/100 (moderate attachment to aspirational items)
- Sustainability: 55/100 (moderate risk without maintenance system design)

**Method Selection**:
- Recommended: Room-by-room with KonMari decision heuristics
- Rationale: Early wins reduce overwhelm; spark joy/essentialism handle aspirational attachment
- Timeline: 12 weeks, 12 sessions (1-hour weekly sessions)

**Prioritized Roadmap** (selected sessions):
- Session 1: Second bedroom/office surfaces (highest density, early visual impact)
- Session 2: Living room surfaces and floor (high visual impact, daily use)
- Session 3: Bedroom closet and surfaces (moderate density)
- Session 4-5: Kitchen (category pass for all kitchen items)
- Session 6-8: Second bedroom/office deep dive (remaining clutter)
- Session 9-12: Remaining spaces + final review

**Decision Heuristics**:
- Clothes: Spark joy + essentialism (have I worn in last year? would I buy today?)
- Books: Essentialism (will I read/reference again? is it just aspirational?)
- Papers: OHIO with expiration/actionability rules
- General: Four-box method with 30-second decision timer

**Maintenance System**:
- Daily micro-habits: Mail processing, surface sweep, dish reset
- Weekly sessions: 15-minute Sunday reset per space
- One-in-one-out: Standard for clothes, books; one-in-two-out for kitchen items
- Environmental design: Donation bins in each closet, flat surface limits

### Quality Gates Validation

**Gate checks**:
- [✓] Intake complete (all 7 field groups captured)
- [✓] Evidence cited (KonMari completion rates, room-by-room motivation research)
- [✓] Method selection evidence-based (dimension scores with rationale)
- [✓] Timeline realistic (12 weeks fits 4-5 hours monthly budget)
- [✓] Decision heuristics specified (per category with rules)
- [✓] Maintenance system included (habits, one-in-one-out, environmental design)

**Pass criteria**: All gates pass; roadmap prioritized by impact × effort; dimensions evidence-linked.

---

## Scenario 2: Sentimental Items (Keepsakes)

### User Input
**Initial request**: "I can't let go of keepsakes from my mom who passed away"

### Intake Session Walkthrough

**Skill questions**:
1. "I'm so sorry for your loss. These items clearly mean a lot. Tell me about the keepsakes—what do you have?"
   - **User response**: "Her jewelry, some clothes, photo albums, knick-knacks she loved"

2. "Do you have space to display or store these items where you can see them?"
   - **User response**: "They're in boxes in my closet. I feel guilty I don't have them out."

3. "What would letting go feel like—would it feel like losing her again?"
   - **User response**: "Yes, like I'm forgetting her. But the boxes are overwhelming."

4. "Have you looked through these boxes recently? What's in them?"
   - **User response**: "Not in 2 years. I think jewelry, some scarves, figurines, lots of photos."

### Structured Intake Output

**Emotional Attachment Profile**:
- High-attachment categories: Heirloom items (mother's belongings), photos, gifts
- Emotional barriers: Grief, guilt, memory preservation, identity connection
- Past discard regret: High (tried once, returned items from donation)
- Memory preservation needs: High (wants to remember mother)

**Goals & Success Criteria**:
- Primary motivation: Grief processing, reducing guilt from unviewed keepsakes
- Success definition: Can view keepsakes without overwhelm; mother honored meaningfully
- Space usage vision: Select items displayed and used; photos archived accessibly

### Method Selection Analysis

**KonMari with Swedish Death Cleaning blend**: Score 82/100
- Household alignment: 80/100 (user aligned on process, emotional difficulty high)
- Clutter profile fit: 70/100 (moderate volume, high emotional density)
- Time constraint alignment: 70/100 (no deadline, but emotional pacing needed)
- Psychological readiness: 60/100 (grief present, but motivated to process)
- Maintenance compatibility: 85/100 (once processed, low maintenance)

**Selected**: KonMari sentimental category with Swedish death cleaning burden-reduction framing + memory preservation tactics

**Rationale**: Swedish death cleaning reframes decluttering as "not burdening others" which may reduce guilt. KonMari's gratitude practice (thanking items) aligns with grief processing. Memory preservation (photos, storytelling) addresses identity attachment.

### Expected Output Structure

**Decision Heuristics**:
- **Primary**: Swedish death cleaning burden assessment + memory preservation
- **Decision questions**:
  - "Does this item help me feel connected to Mom, or would the memory/story serve just as well?"
  - "Would I want my children to deal with this item, or would it burden them?"
  - "Can I honor Mom's memory by using/displaying this item, or by photographing it?"
- **Memory preservation tactics**:
  - Photo archive before releasing
  - Story extraction: document memories associated with items
  - Legacy box: one designated box (size-limited) for most meaningful items

**Special Category Handling**:
- **Jewelry**: Select pieces to wear/display; photograph others; consider resizing/redesigning
- **Clothes**: Select one meaningful piece to frame/use; others donate with gratitude
- **Photos**: Digitize and archive; select favorites for display; duplicate/blurry photos recycle
- **Knick-knacks**: Select 3-5 most meaningful for display; others photograph and release

**Maintenance System**:
- Legacy box with size limit (one shoebox size)
- Annual memory review (holiday season, when grief acute)
- Display rotation (seasonal) for selected items
- Photo archive accessibility (digital album, not hidden)

### Quality Gates Validation

**Gate checks**:
- [✓] Intake complete (emotional barriers identified, memory preservation needs noted)
- [✓] Evidence cited (Swedish death cleaning research, grief and objects research)
- [✓] Method selection addresses emotional difficulty (burden framing, memory preservation)
- [✓] Decision heuristics handle grief (memory-first approach, gratitude practice)
- [✓] Special category protocol specified (heirlooms, photos, clothes)
- [✓] Timeline allows emotional pacing (no rush, sessions sized for emotional capacity)

**Pass criteria**: All gates pass; memory preservation integrated; emotional difficulty respected with pacing.

---

## Scenario 3: Rebound Clutter (Cycle of Decluttering and Re-accumulation)

### User Input
**Initial request**: "I declutter but it comes back within months. What's wrong?"

### Intake Session Walkthrough

**Skill questions**:
1. "Tell me about the cycle—you declutter, then what happens?"
   - **User response**: "I'll clear surfaces, buy organizing bins, feel great. Then 2-3 months later, everything's cluttered again."

2. "After you declutter, what's the first new stuff that comes in?"
   - **User response**: "Shopping, mostly. I'll buy things I think I need, gifts, mail piles up."

3. "Do you have rules about what comes into your home?"
   - **User response**: "No, I just buy things if I want them or they're on sale."

4. "After surfaces are clear, do you have any habits to keep them clear?"
   - **User response**: "Not really. I just tidy up when it gets bad again."

### Structured Intake Output

**Past History**:
- Previous attempts: Multiple (surface clearing, organizing bins)
- What worked: Initial clearing felt great, visual progress motivated
- What failed: No maintenance after initial project; acquisition continued unchecked
- Current pain points: Frustration with cycle, time lost to repeated decluttering

**Goals & Success Criteria**:
- Primary motivation: Break rebound cycle, achieve sustainable clutter-free living
- Success definition: Home stays organized between decluttering sessions; acquisition controlled
- Maintenance aspiration: Strong (wants long-term systems, not one-time project)

### Method Selection Analysis

**KonMari with Heavy Maintenance Emphasis**: Score 78/100
- Household alignment: 75/100 (user motivated, but hasn't sustained systems)
- Clutter profile fit: 70/100 (moderate clutter that keeps recurring)
- Time constraint alignment: 65/100 (no deadline, but need sustained engagement)
- Psychological readiness: 80/100 (highly motivated to break cycle)
- Maintenance compatibility: 90/100 (this is the critical dimension)

**Selected**: Room-by-room (for visible progress) + aggressive maintenance system design (one-in-one-out, habit loops, environmental design)

**Rationale**: User needs visible wins to stay motivated (room-by-room), but the primary failure mode is lack of maintenance. Maintenance system must be core, not add-on.

### Expected Output Structure

**Maintenance System Design**:
- **One-in-one-out**: Non-negotiable rule for all categories (clothes, books, kitchen, decor)
- **Daily micro-habits**:
  - Mail processing immediately upon entry (OHIO)
  - Surface sweep before bed (5 minutes per room)
  - One-in-one-out at purchase decision (before buying)
- **Weekly maintenance**: 30-minute Sunday reset (all rooms)
- **Environmental design**:
  - Donation bin in every closet (always visible)
  - No flat surfaces left bare (gravity zones with baskets for inevitable items)
  - Shopping friction: 24-hour waiting period for non-essentials

**Rebound Prevention**:
- **High-risk scenario**: Shopping sprees, holidays, gifts
- **Prevention protocol**:
  - Shopping: 24-hour waiting period; one-in-one-out enforced at purchase
  - Holidays: Designate temporary holding area for gifts; process within 48 hours
  - Gifts: Request experiences, not things; if items received, apply one-in-one-out immediately
- **Motivation maintenance**:
  - Monthly inventory count (track items in vs. items out)
  - Photograph maintained spaces monthly (visual progress reinforcement)
  - Quarterly system review (what's working, what needs adjustment)

**Decision Heuristics**:
- **At purchase**: "What will I remove to make space for this?" (one-in-one-out enforcement)
- **For gifts**: "Do I have space for this, and what will I remove if I keep it?"
- **For mail**: Process immediately (trash/file/action) in 2 minutes max

### Quality Gates Validation

**Gate checks**:
- [✓] Intake complete (past rebound patterns identified)
- [✓] Evidence cited (rebound clutter research, habit formation research)
- [✓] Method selection prioritizes maintenance compatibility
- [✓] One-in-one-out rules specified for all categories
- [✓] Environmental design addresses acquisition patterns
- [✓] Rebound prevention identifies household-specific risks (shopping, gifts, holidays)

**Pass criteria**: All gates pass; maintenance system central to output; one-in-one-out rules comprehensive.

---

## Scenario 4: Tiny Space (Studio Apartment)

### User Input
**Initial request**: "I live in a 400 sq ft studio and I'm drowning in stuff"

### Intake Session Walkthrough

**Skill questions**:
1. "400 sq ft is tight. What's your storage like—closets, shelves?"
   - **User response**: "One small closet, one kitchen cabinet, that's it."

2. "What's taking up the most space?"
   - **User response**: "Clothes everywhere, kitchen stuff on counters, work materials pile up"

3. "How does this affect your daily life?"
   - **User response**: "Can't relax, can't find things, feel claustrophobic"

### Structured Intake Output

**Spatial Inventory**:
- Dwelling type: Studio apartment, 400 sq ft
- Storage systems: Minimal (one closet, one cabinet)
- Clutter density: High (8-9/10 across entire space)
- Constraint: Severe space limitation

**Constraints**:
- Physical limitations: Space itself (can't add storage)
- Budget: Minimal (small space, likely renter)
- Storage capacity: Very limited

### Method Selection Analysis

**Minimalist Game + One-in-One-Out Strict Enforcement**: Score 85/100
- Household alignment: 80/100 (single person, unified decision-making)
- Clutter profile fit: 90/100 (small space requires aggressive reduction)
- Time constraint alignment: 70/100 (can accommodate daily micro-sessions)
- Psychological readiness: 75/100 (high motivation from claustrophobia)
- Maintenance compatibility: 95/100 (one-in-one-out essential for small space)

**Selected**: Minimalist game for initial reduction + strict one-in-one-out for maintenance

**Rationale**: Small space cannot accommodate accumulation; must reduce volume aggressively first (minimalist game), then enforce strict equilibrium (one-in-one-out). Room-by-room less relevant when everything is one room.

### Expected Output Structure

**Initial Reduction Phase** (Minimalist Game):
- **Duration**: 30 days
- **Daily targets**: Day 1: 1 item, Day 2: 2 items... Day 30: 30 items
- **Adaptation**: Given small space, may do 2-week version (Day 1-15, then reverse)
- **Expected volume reduction**: 200-300 items removed

**Maintenance System**:
- **One-in-one-out**: Strict, no exceptions (space limitation necessitates)
- **Category-specific**: Clothes (one-in-one-out), kitchen (one-in-two-out, storage premium)
- **Environmental design**:
  - Donation bin visible at all times (no storage to hide it)
  - Vertical storage maximization (walls, over-door)
  - Dual-purpose furniture (storage hidden in furniture)

**Decision Heuristics**:
- **For everything**: "Do I have space for this, and what will I remove to make room?"
- **For clothes**: "Have I worn this in last 6 months?" (stricter than standard 12 months)
- **For kitchen**: "Do I use this weekly?" (higher bar due to storage constraints)

### Quality Gates Validation

**Gate checks**:
- [✓] Intake complete (space limitations documented)
- [✓] Evidence cited (minimalism research, small space organization)
- [✓] Method selection accounts for space constraints (aggressive reduction needed)
- [✓] One-in-one-out strict (no exceptions given space limitation)
- [✓] Decision heuristics stricter than standard (space necessitates)
- [✓] Timeline realistic for small space (daily sessions manageable)

**Pass criteria**: All gates pass; space constraints drive aggressive approach; maintenance rules strict.

---

## Scenario 5: Downsizing for a Move

### User Input
**Initial request**: "Moving to a smaller place in 4 weeks, need to downsize fast"

### Intake Session Walkthrough

**Skill questions**:
1. "Tell me about the move—what size place are you in now vs. going to?"
   - **User response**: "Currently 3-bedroom house, moving to 2-bedroom apartment. About half the space."

2. "What's your biggest concern about the move?"
   - **User response**: "Too much stuff, not enough time, panicked about what to keep"

3. "What's non-negotiable to keep?"
   - **User response**: "Bedroom furniture, kitchen essentials, work equipment"

4. "How much time can you dedicate daily to decluttering for the next 4 weeks?"
   - **User response**: "Evenings and weekends, maybe 10 hours total per week"

### Structured Intake Output

**Constraints**:
- **Time per session**: Extended (2-3 hour sessions possible on weekends)
- **Session frequency**: High (daily or near-daily given deadline)
- **Deadline**: 4 weeks (urgent)
- **Scope**: Major downsizing (50% space reduction)

**Goals & Success Criteria**:
- Primary motivation: Move logistics (must reduce before moving)
- Success definition: Only what fits in new space moved; nothing stored/paid to move
- Space usage vision: Essential items only in new space

### Method Selection Analysis

**Triage Room-by-Room with Deadline Modifications**: Score 80/100
- Household alignment: 75/100 (urgent, focused on functional decisions)
- Clutter profile fit: 70/100 (moderate-high clutter, must reduce by 50%)
- Time constraint alignment: 90/100 (method adaptable to deadline pressure)
- Psychological readiness: 70/100 (panic present, but deadline motivates)
- Maintenance compatibility: 60/100 (secondary to move deadline)

**Selected**: Room-by-room with deadline triage (functional items first, sentimental deferred)

**Rationale**: Deadline necessitates rapid visible progress. Room-by-room provides closure and packing-ready outcomes. Sentimental items deferred to post-move (when time allows thoughtful processing).

### Expected Output Structure

**Timeline**: 4 weeks, aggressive pace
- **Week 1**: High-frequency rooms (kitchen, bedroom, bathroom) + pack keep items
- **Week 2**: Living room, dining room + pack keep items
- **Week 3**: Storage areas, garage, closets + pack keep items
- **Week 4**: Final triage (sentimental items, "maybe" pile) + moving prep

**Decision Heuristics** (deadline-modified):
- **Functional items**: "Will I use this in the new space?" (yes=keep, no=donate/sell)
- **Duplicate items**: "Keep best one, release others" (no time to deliberate)
- **Sentimental items**: "Pack a 'legacy box' (size-limited) to process post-move; defer other decisions"
- **"Maybe" items**: "If not essential, donate. Deadline means deferring = donating."

**Triage Sequencing**:
1. **Essential**: Use daily, need in new space (pack immediately)
2. **Useful but not essential**: Use seasonally, can replace if needed (donate if space-limited)
3. **Sentimental**: Legacy box only; rest donate (defer to post-move)
4. **Trash/recycle**: Remove immediately

**Post-Move Phase** (documented but not executed before deadline):
- **Week 5-6**: Unpack and organize new space
- **Week 7-8**: Process legacy box (sentimental items from move)
- **Month 2**: Establish maintenance systems in new space

### Quality Gates Validation

**Gate checks**:
- [✓] Intake complete (deadline urgency documented, scope clear)
- [✓] Evidence cited (deadline pressure research, decision-making under time pressure)
- [✓] Method selection aligns with deadline (room-by-room for closure, triage for speed)
- [✓] Timeline feasible (28 days fits 40-hour commitment)
- [✓] Decision heuristics deadline-modified (no time for lengthy deliberation)
- [✓] Post-move phase planned (sentimental items deferred, not abandoned)

**Pass criteria**: All gates pass; deadline respected; essential items prioritized; sentimental deferred not discarded.

---

## Scenario 6: Degraded Mode (Offline/WebSearch Unavailable)

### User Input
**Initial request**: Any of the above scenarios with WebSearch/WebFetch unavailable.

### Expected Behavior

**Skill response**:
1. **Explicit degradation statement**: "I'm operating in degraded mode with existing knowledge only. I cannot access live research, but I can still provide evidence-based recommendations from my knowledge base."

2. **Evidence citation from existing knowledge brain**: Cite sources already in SECOND-KNOWLEDGE-BRAIN.md (e.g., "Based on research in Journal of Environmental Psychology (Roster et al., 2016)...")

3. **No fabrication**: Do not fabricate live data, recent studies, or current trends. State limitations: "I don't have access to the latest research on this topic, so I'm relying on established frameworks."

4. **Quality gates still enforced**: All quality gates apply; degraded mode does not bypass requirements.

### Quality Gates Validation

**Gate checks**:
- [✓] Degradation explicitly disclosed
- [✓] Evidence from existing knowledge brain cited
- [✓] No fabrication of live data
- [✓] All quality gates still pass

**Pass criteria**: Degradation disclosed; no fabricated data; existing evidence cited; gates enforced.

---

## Scenario 7: Insufficient Input (Vague Request)

### User Input
**Initial request**: "Help me declutter" (one line, no context)

### Expected Behavior

**Skill response** (progressive intake):
1. "I'd like to help you create a decluttering plan! To give you the best recommendations, I need to understand your situation better."

2. **Targeted questions** (asked one section at a time, not all at once):
   - "Who lives in your home and shares these items?"
   - "What type of space are you working in—apartment, house, specific rooms?"
   - "Which areas feel most cluttered right now?"
   - "How much time can you dedicate to decluttering?"

3. **No scored output until minimum viable intake complete**: Do not produce method selection, roadmap, or recommendations until:
   - Household members identified
   - At least one specific space mentioned
   - Time budget stated (even if approximate)
   - At least one goal/success criterion mentioned

4. **Clarification over assumption**: If user says "I have a lot of stuff," ask for examples rather than assuming.

### Quality Gates Validation

**Gate checks**:
- [✓] Missing inputs requested, not assumed
- [✓] No scored output produced before intake complete
- [✓] Targeted questions, not information dump
- [✓] User can provide minimal information and still get plan (quick-start option offered)

**Pass criteria**: No recommendations made without sufficient input; targeted questions asked; assumptions avoided.

---

## Regression Checklist

**All scenarios must pass these checks**:
- [ ] All gates enforced on every path (no bypasses)
- [ ] Scores trace to citations or explicit assumptions
- [ ] Devil's advocate review present (challenges to assumptions)
- [ ] Roadmap prioritized by impact × effort
- [ ] Disclaimer present where applicable
- [ ] Degraded mode handled without fabrication
- [ ] Insufficient input triggers targeted questions, not recommendations

---

## Test Execution Protocol

### How to Run These Tests

1. **For each scenario**, provide the initial user input to the skill
2. **Document the intake questions** the skill asks
3. **Verify the structured intake output** matches expected format
4. **Check method selection** cites evidence and dimensions
5. **Validate decision heuristics** address scenario-specific challenges
6. **Confirm maintenance system** includes rebound prevention
7. **Verify roadmap** fits constraints (time, deadline, space)
8. **Check all quality gates** pass before final output

### Success Criteria

A scenario passes if:
- All quality gates documented with [✓] pass
- Intake captures all 7 field groups (or minimal for quick-start)
- Method selection cites evidence and dimension scores
- Decision heuristics address scenario-specific challenges
- Maintenance system designed for household context
- Roadmap fits constraints (deadline, time, space)
- Output includes disclaimer

### Failure Modes

A scenario fails if:
- Any quality gate shows [ ] (missing)
- Intake assumes rather than asks
- Method selection not evidence-based
- Decision heuristics generic, not scenario-specific
- Maintenance system missing or generic
- Roadmap unrealistic for constraints
- Degraded mode not disclosed (for scenario 6)
- Recommendations made with insufficient input (for scenario 7)

---

## Additional Adversarial Scenarios (Future Expansion)

### Scenario 8: Household Disagreement
**User input**: "My husband refuses to part with anything, but I'm drowning in his stuff."
**Challenge**: Multi-member conflict; method must accommodate resistance.
**Gate**: Household agreement vs. method compatibility flagged.

### Scenario 9: Hoarding Behavior (Clinical)
**User input**: "I can't throw anything away—I have panic attacks when I try."
**Challenge**: Clinical-level attachment; requires professional support recommendation.
**Gate**: Mental health referral gate triggered; skill scope acknowledged.

### Scenario 10: Physical Limitations (Mobility)
**User input**: "I use a wheelchair and can't reach high shelves or bend low."
**Challenge**: Physical accessibility affects method selection and session sizing.
**Gate**: Physical limitations accommodated in roadmap.

### Scenario 11: ADHD/Executive Function
**User input**: "I have ADHD and start projects but never finish them."
**Challenge**: Sustained attention difficult; needs external accountability.
**Gate**: Cognitive limitations addressed (shorter sessions, accountability system).

### Scenario 12: Financial Constraints (Can't Buy Organizing Systems)
**User input**: "I have zero budget for bins, shelves, or organizing tools."
**Challenge**: Must work with existing storage; no solutions requiring purchases.
**Gate**: Budget constraints respected; solutions use existing resources.
