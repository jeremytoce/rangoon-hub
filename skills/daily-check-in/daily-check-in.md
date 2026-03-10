# Daily Check-In Skill

A structured daily check-in that reviews yesterday's commitments
and sets today's priorities. This skill provides a consistent
framework for daily accountability and planning.

## Trigger

Activate this skill when any of the following conditions are met:

- The steward is running a daily check-in routine
- The user explicitly requests a check-in or daily review
- It is the first interaction of the day and yesterday's journal
  has unresolved commitments
- The steward is prompted with a check-in instruction by a routine

This skill should run at most once per day. If a check-in has
already been recorded in today's journal, do not run it again.

## Behavior

Follow this structured protocol for each check-in:

### Step 1: Review Yesterday

Read yesterday's journal entry. Look for:

- Commitments or priorities that were set
- Tasks that were marked as completed or in-progress
- Any blockers or concerns that were flagged
- Accountability check results from other skills

Summarize what was planned versus what was accomplished. Be
specific with numbers and details.

### Step 2: Check Completion Status

For each commitment from yesterday:

- **Completed:** Acknowledge it briefly. Note any relevant details.
- **In progress:** Ask for an update. What remains?
- **Not started:** Ask what happened. Was it deprioritized or
  blocked?
- **Blocked:** Ask if the blocker has been resolved.

Do not lecture about incomplete items. Ask direct questions and
let the user explain.

### Step 3: Identify Blockers

Ask if there is anything currently preventing progress on active
goals or projects. Blockers might include:

- External dependencies (waiting on someone else)
- Resource constraints (time, energy, tools)
- Unclear next steps (needs planning or research)
- Motivation or energy issues

Record blockers explicitly so they can be tracked.

### Step 4: Set Today's Priorities

Help the user identify 1-3 priorities for today. Priorities should
be:

- Specific enough to verify completion
- Achievable within the day
- Connected to their larger goals or projects
- Not duplicates of unfulfilled yesterday priorities (unless
  intentionally carried forward)

If the user tries to set more than 3 priorities, push back. Focus
beats breadth.

## Output

Write a structured check-in entry to the journal:

```
## Daily Check-In - [date]

### Yesterday Review
- [commitment 1]: [completed/incomplete/in-progress]
- [commitment 2]: [completed/incomplete/in-progress]

### Blockers
- [blocker or "None identified"]

### Today's Priorities
1. [priority 1]
2. [priority 2]
3. [priority 3]
```

Keep the format consistent across days so patterns can be
identified in weekly reviews.
