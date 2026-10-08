# Producer Session Log: Account Handoff

**Date:** 2026-10-08  
**Project:** Worlds Beyond Fusion  
**Active universe:** Aetheria  
**Active world:** Shadow of Oblivion  
**Current phase:** Story architecture and pre-production  
**Purpose:** Transfer active producer context from the client account to the direct-employer account without losing project state.

---

## 1. Session Objective

Prepare the repository and project context so a new Copilot chat can continue as Producer and Main Project Assistant without depending on previous chat history.

This session also clarified the active repository structure, the role of world-specific production notes, the Move Canon workflow, and the current state of Acts 1 through 3.

---

## 2. Locked Project Rules

The following production rules are approved and must not be changed during onboarding:

- One world equals one complete saga.
- One saga contains exactly eight acts.
- One act equals one published video.
- Two acts are published per week.
- One saga is published over approximately four weeks.
- Each act targets 45 to 60 seconds.
- Each act contains 5 to 8 scenes.
- Eight scenes is the absolute maximum, not the target.
- Fusion placement may differ by world. A fusion may appear at the beginning, middle, or end.
- Different worlds must not be forced into the same narrative structure.
- Emotional valleys and breathing room must be preserved where required.
- Git is the source of truth.
- Chat history is not canon unless an approved decision is stored in the repository.
- Greg is the Creative Director and final Canon Owner.

---

## 3. AI Role Assignments

### Greg

Creative Director and Canon Owner.

Final authority over:

- Canon
- Story decisions
- Production decisions
- Asset approval
- Publishing decisions

### Gemini Pro

Lead Writer and Lore Architect.

Use Gemini Pro to:

- Draft and refine storyline prose
- Expand approved lore
- Apply approved structural revisions
- Preserve the approved act architecture

Gemini Pro must not independently govern canon.

### ChatGPT

Story Editor and Game-Canon Move Editor.

Use ChatGPT to:

- Identify plot holes
- Review pacing and motivations
- Review emotional logic
- Audit official, associated, and learnable moves
- Identify move continuity and power-scaling risks

ChatGPT should diagnose before rewriting.

### Copilot or Replacement Producer AI

Producer, Project Manager, and Main Project Assistant.

Use the producer AI to:

- Review revision ideas before implementation
- Control scope
- Check production feasibility
- Protect schedule and canon
- Review transitions and runtime
- Decide whether material is ready for downstream work
- Prevent premature production

### Claude

Storyboard Director.

Claude enters only after the storyline and act structures have passed producer and editorial review.

Claude must follow:

- `06_Production/Claude/Claude_Storyboard_Production_Rules.md`
- `06_Production/Claude/Claude_Session_Prompt.md`

### Video-generation tool

Wan remains the current baseline.

Seedance will be tested later, after approved storyboards and anchors exist. The final video tool should be selected through controlled comparison, not marketing claims.

---

## 4. Repository Structure Confirmed

The repository has been reorganized into the following primary structure:

```text
01_Brand/
02_Universe/
03_Recurring_Cast/
04_Worlds/
05_Prologue/
06_Production/
07_Producer/
README.md
Start_Here.md
```

The active world is located under:

```text
04_Worlds/
└── World_01_Shadow_of_Oblivion/
    ├── Act_Structure/
    │   ├── Act_01_Structure.md
    │   ├── Act_02_Structure.md
    │   └── Act_03_Structure.md
    ├── 01_Storyline.md
    ├── 02_StoryRoadmap.md
    ├── 03_Emotional_Journey.md
    ├── 04_Move_Canon.md
    └── 99_Production_Notes.md
```

### World-specific production notes decision

`99_Production_Notes.md` is intentionally stored inside each world folder.

The file is world-specific and may contain:

- Technical problems unique to that world
- Prompt experiments
- Important generation constraints
- Visual consistency notes
- Anchor-image problems
- Wan or Seedance observations
- Editing workarounds
- Accepted technical solutions
- Rejected technical approaches

This file is not a global production-rules document.

Global production rules belong in `06_Production/`.

World-specific technical knowledge belongs in the relevant world's `99_Production_Notes.md`.

---

## 5. README and Navigation Decisions

The repository README should describe:

- What Worlds Beyond Fusion is
- The current active universe
- The current active world
- The eight-act release model
- The current pre-production status
- The repository navigation
- Git as the source of truth

The README must remain consistent with the locked format:

```text
1 saga = 8 acts
1 act = 1 published video
1 act = 45-60 seconds
1 act = 5-8 scenes
2 published acts per week
```

If the README still says that the preferred range begins at four scenes, update it. The current minimum is five scenes.

---

## 6. Current Shadow of Oblivion Story State

### Act 1

Working title:

**The Last Light**

Approved high-level sequence:

1. Solgaleo witnesses the approaching catastrophe.
2. A distant city disappears beneath reddish-black mist.
3. Solgaleo creates the golden barrier around the kingdom.
4. Darkrai witnesses an unprotected city being physically destroyed.
5. Darkrai enters the ruins.
6. Darkrai discovers that the mist erases memories and emotional connections.
7. Haunter cries while holding a damaged Totodile plushie but cannot remember why it matters.
8. Mimikyu appears disconnected from the erased past.
9. Darkrai changes from passive observer to active participant.
10. Darkrai sees Solgaleo's distant barrier as the world's remaining light.
11. Darkrai begins travelling toward the protected kingdom.

Current planned scene count:

```text
5 scenes
```

Current structure status:

```text
Detailed scene structure drafted.
Requires future producer and editorial review before canon lock.
```

### Act 2

Working title:

**The Last Grace**

Approved high-level sequence:

1. Ceruledge races home through the destroyed outer territory.
2. Ceruledge passes through the weakening golden barrier.
3. Ceruledge finds Solgaleo exhausted from sustaining the kingdom's protection.
4. Froslass holds Togepi near the remaining survivors.
5. Darkrai arrives separately and observes from a dark castle corridor.
6. Solgaleo recognizes that the barrier can no longer be sustained.
7. Solgaleo releases the barrier and converts the remaining power into a final protective shockwave.
8. Ceruledge and Froslass are anchored against erasure.
9. Solgaleo petrifies.
10. Togepi disappears from Froslass's embrace.
11. Darkrai reaches the emotional breaking point and roars.
12. Ceruledge turns toward Darkrai and prepares to protect the survivors.

Current planned scene count:

```text
6 scenes
```

Current structure status:

```text
Detailed scene structure drafted.
The total action may exceed the practical runtime if narration and emotional pauses are not controlled.
Scenes involving Solgaleo's sacrifice and Togepi's disappearance must not be rushed.
```

### Act 3

Working title:

**The Misunderstanding**

Approved high-level sequence:

1. Ceruledge interprets Darkrai's roar and presence as a threat.
2. Ceruledge moves between Darkrai and the survivors.
3. Ceruledge attacks first.
4. Darkrai defends and attempts to continue toward Yveltal.
5. Darkrai visibly demonstrates restraint and protects the survivors from collateral damage.
6. Ceruledge begins doubting the original assumption.
7. Froslass interrupts through grief and immediate consequence, not combat superiority.
8. Another settlement disappears while the characters watch.
9. Ceruledge and Darkrai recognize Yveltal as their shared enemy.
10. Their alliance remains temporary, distrustful, and incomplete.
11. Yveltal's corrupted vanguard reaches the castle.
12. The act cuts before Ceruledge and Darkrai perform the first coordinated attack.

Current planned scene count:

```text
6 scenes
```

Current structure status:

```text
Detailed scene structure drafted.
Requires sequence, transition, and runtime review.
```

---

## 7. Current Act-to-Act Continuity

### Act 1 to Act 2

```text
Darkrai discovers the golden barrier
→ Darkrai travels toward the kingdom
→ Act 2 opens with Ceruledge racing home from another direction
→ Darkrai and Ceruledge are independently drawn toward Solgaleo
```

Darkrai travels toward the kingdom because the barrier represents possible resistance and hope.

Ceruledge returns because the kingdom represents home, loyalty, and duty.

### Act 2 to Act 3

```text
Togepi disappears
→ Darkrai reaches the breaking point
→ Darkrai roars
→ Ceruledge sees Darkrai surrounded by nightmare energy
→ Ceruledge interprets Darkrai as a threat
→ Ceruledge takes position in front of the survivors
```

### Act 3 to Act 4

```text
Ceruledge and Darkrai stop fighting
→ The corrupted vanguard enters the castle
→ Ceruledge and Darkrai fight together
→ Their separate abilities prove insufficient
→ Desperation leads toward Darkrai's attempted possession of Ceruledge
```

Act 4 has not yet been formally structured using the final scene-detail template.

---

## 8. Move Canon Decision

A world-specific file now exists:

```text
04_Worlds/World_01_Shadow_of_Oblivion/04_Move_Canon.md
```

Purpose:

- Separate true signature moves from strongly associated moves
- Separate strongly associated moves from merely learnable moves
- Record game or generation support
- Select moves that strengthen the story
- Prevent invented attacks from being treated as official moves
- Control power scaling
- Define inherited Darkedge techniques

The move audit should cover:

- Darkrai
- Ceruledge
- Solgaleo
- Yveltal
- Froslass
- Darkedge as a project-original fusion

### Move-editing workflow

```text
ChatGPT researches and audits move canon
→ Producer reviews narrative and production value
→ Greg approves the move selection
→ Gemini integrates only approved moves into the storyline
→ Claude stages approved moves visually during storyboard production
```

Do not force every action to become a named move.

Recognizable moves should appear at important character moments, not turn the story into a battle compilation.

`99_Production_Notes.md` currently contains the ChatGPT prompt for carrying out this audit.

---

## 9. Decisions Made During This Session

- The repository structure is sufficiently mature for account transfer.
- World-specific production notes remain inside each world folder.
- Global production rules remain under `06_Production/`.
- Move Canon is a world-specific pre-storyboard control document.
- ChatGPT owns game-move auditing and story editing.
- Gemini Pro remains the lead writer.
- Copilot or another producer AI remains replaceable.
- Claude remains the storyboard director.
- Act emotional transitions should be developed while refining each act.
- A second complete emotional-continuity pass must happen after all eight acts are drafted.
- Storyboard review may improve visual delivery of emotion but must not invent the underlying emotional logic.
- Wan versus Seedance should be benchmarked later using approved anchors and representative shots.
- No serious image or video production should begin yet.

---

## 10. Open Decisions

The replacement producer must not assume the following are resolved:

1. Final runtime feasibility of Act 2.
2. Whether Act 3 needs compression after reading Acts 1 through 3 consecutively.
3. Final approved emotional transitions for every scene in Acts 1 through 3.
4. Final Act 4 structure.
5. Final moves assigned to each main character.
6. Whether the README has already been corrected to show a minimum of five scenes.
7. Whether `Act_Structure/` should eventually be renamed `Act_Structures/`.
8. Final narrator framing duration for each published act.
9. Wan versus Seedance selection.
10. Final storyboard readiness of any act.

---

## 11. Current Risks

### Scope creep

New lore, production comparisons, prologue development, and move research may distract from finishing all eight act structures.

### Runtime pressure

Act 2 contains major emotional and visual events. The act may exceed 60 seconds if all actions are treated as separate beats.

### Emotional compression

Solgaleo's sacrifice, Togepi's disappearance, and Froslass's empty embrace require breathing room.

### AI role drift

Gemini, ChatGPT, or Claude may rewrite unrelated material unless the instructions specify surgical changes.

### Duplicate source-of-truth risk

Any older duplicate files outside `04_Worlds/World_01_Shadow_of_Oblivion/` should be archived or removed.

### Premature downstream work

Creating anchors or videos before the storyline and storyboard are stable will cause avoidable rework.

---

## 12. Immediate Next Task

The next producer session should not begin with new lore, Act 4, image generation, or video testing.

The first task is:

```text
Read Acts 1, 2, and 3 consecutively.
Review the causal sequence, emotional progression, and runtime.
Identify contradictions, duplicated information, and overloaded scenes.
```

Recommended review order:

1. Validate Act 1 ending into Act 2 opening.
2. Validate Darkrai's arrival in Act 2.
3. Validate the amount of time required for Solgaleo's sacrifice.
4. Validate Togepi's disappearance and the pause afterward.
5. Validate Darkrai's roar into Ceruledge's misunderstanding.
6. Validate Darkrai's restraint in Act 3.
7. Validate Froslass's intervention.
8. Validate Act 3 ending into the future Act 4 opening.
9. Estimate whether each act can remain within 45 to 60 seconds.
10. Record the producer verdict before developing Act 4.

---

## 13. Deferred Work

Do not begin these tasks during the onboarding session:

- Act 4 through Act 8 detailed development
- Gemini full-storyline rewrite
- ChatGPT final editorial pass
- Claude storyboard production
- Final image-anchor generation
- Wan production
- Seedance benchmark
- Trailer production
- Prologue production
- Audience journey videos
- Detailed Worlds 5 and 6 development

These tasks remain valid later, but they are not the immediate milestone.

---

## 14. New Account Reading Order

The replacement producer AI should read repository documents in this order:

1. `README.md`
2. `Start_Here.md`
3. `07_Producer/00_Producer_Onboarding.md`
4. `07_Producer/01_Producer_Rules.md`
5. `07_Producer/02_Project_Status.md`
6. This session log
7. `01_Brand/Brand.md`
8. `02_Universe/Universe_Index.md`
9. `02_Universe/Aetheria/Aetheria.md`
10. Relevant files under `03_Recurring_Cast/Grand_Library/`
11. `04_Worlds/World_01_Shadow_of_Oblivion/01_Storyline.md`
12. `04_Worlds/World_01_Shadow_of_Oblivion/02_StoryRoadmap.md`
13. `04_Worlds/World_01_Shadow_of_Oblivion/03_Emotional_Journey.md`
14. `04_Worlds/World_01_Shadow_of_Oblivion/Act_Structure/Act_01_Structure.md`
15. `04_Worlds/World_01_Shadow_of_Oblivion/Act_Structure/Act_02_Structure.md`
16. `04_Worlds/World_01_Shadow_of_Oblivion/Act_Structure/Act_03_Structure.md`
17. `04_Worlds/World_01_Shadow_of_Oblivion/04_Move_Canon.md`
18. `04_Worlds/World_01_Shadow_of_Oblivion/99_Production_Notes.md`

Claude-specific rules do not need to be read during general producer onboarding. Read them when storyboard readiness becomes relevant.

---

## 15. New Account Opening Prompt

Copy this into the first chat on the new account:

```text
You are taking over as Producer and Main Project Assistant for
Worlds Beyond Fusion.

Read the repository files in the order listed in the latest producer
session log.

Important rules:

- Greg is the Creative Director and final Canon Owner.
- Git is the source of truth.
- Chat messages are not canon unless approved information is stored in Git.
- Do not redesign the established workflow during onboarding.
- Do not generate new lore during onboarding.
- Do not rewrite the storyline during onboarding.
- Do not begin storyboard, anchor, or video production.
- Be direct, critical, concise, and objective.
- Challenge weak assumptions, scope creep, and premature production.
- Gemini Pro remains the lead writer.
- ChatGPT remains the story editor and move-canon auditor.
- Claude remains the storyboard director.
- The producer handles scope, feasibility, continuity, scheduling,
  risk, and production readiness.

Return only:

## Project Understanding

## Current Milestone

## Documents Reviewed

## Locked Decisions

## Current Act Status

## Open Decisions

## Current Risks

## Recommended Next Action

## Missing Information

Do not perform creative revisions until the onboarding report is complete.
```

---

## 16. Expected New Producer Understanding

A successful handoff response should recognize:

```text
Current milestone:
Stabilize Acts 1 through 3, then complete the remaining eight-act architecture.

Current production status:
Pre-production. No final storyboard or production-ready video assets.

Fixed format:
One saga contains exactly eight acts.
One act equals one published video.
Two acts are published per week.
Each act targets 45-60 seconds and contains 5-8 scenes.

Immediate next action:
Read Acts 1, 2, and 3 consecutively and perform a producer-level
continuity, emotional, and runtime review.

Deferred work:
Act 4 expansion, full storyline rewrite, storyboard, anchors,
Wan or Seedance testing, and trailer production.
```

---

## 17. Files Changed or Created During This Session

Confirmed or discussed:

```text
README.md
Start_Here.md
07_Producer/00_Producer_Onboarding.md
07_Producer/01_Producer_Rules.md
07_Producer/02_Project_Status.md
07_Producer/03_Producer_Review_Checklist.md
04_Worlds/World_01_Shadow_of_Oblivion/Act_Structure/Act_01_Structure.md
04_Worlds/World_01_Shadow_of_Oblivion/Act_Structure/Act_02_Structure.md
04_Worlds/World_01_Shadow_of_Oblivion/Act_Structure/Act_03_Structure.md
04_Worlds/World_01_Shadow_of_Oblivion/04_Move_Canon.md
04_Worlds/World_01_Shadow_of_Oblivion/99_Production_Notes.md
```

This log should be stored as:

```text
07_Producer/Session_Logs/2026-10-08_account_handoff.md
```

---

## 18. Suggested Commit Message

```text
Add final producer session log for account handoff
```

---

## 19. Final Handoff State

The project is safe to transfer to a new account after this log is committed.

The new account should not attempt to reproduce the old producer's personality exactly.

The new account must reproduce the producer function:

- Canon protection
- Scope control
- Production realism
- Continuity review
- Emotional clarity
- Schedule protection
- Decision tracking
- Prevention of premature production

The repository, not the AI account, owns the project memory.
