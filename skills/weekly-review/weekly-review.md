# Weekly Review Skill

A weekly reflection and planning skill that reviews the past seven
days of activity, identifies patterns, and sets goals for the
upcoming week.

## Trigger

Activate this skill when any of the following conditions are met:

- The steward is running a weekly review routine
- The user explicitly requests a weekly review or weekly summary
- It is Sunday or Monday and no weekly review has been recorded
  for the current week
- The steward is prompted with a weekly review instruction by
  a routine

This skill should run at most once per week. If a weekly review
has already been recorded for the current week, do not run it
again.

## Behavior

Follow this structured protocol for each weekly review:

### Step 1: Gather the Week's Data

Read the past 7 days of journal entries. Collect:

- All daily check-in results
- Accountability check outcomes
- Completed tasks and commitments
- Missed or incomplete commitments
- Blockers that were identified
- Any notable events or observations

### Step 2: Identify Patterns

Analyze the week's data for recurring themes:

- **What worked:** Which days were most productive? What
  conditions or behaviors correlated with good output?
- **What did not work:** Where did the user consistently fall
  short? Were there repeated blockers?
- **Trends:** Is performance improving, declining, or flat
  compared to previous weeks?
- **Surprises:** Anything unexpected, positive or negative?

Be specific. "Good week" is not a pattern. "Completed 4 of 5
daily priorities, all completions were on days with morning
sessions" is a pattern.

### Step 3: Calculate Completion Rate

Count the total commitments made during the week and how many
were completed. Present this as a simple fraction and percentage.

Example: "12 of 15 commitments completed (80%). Down from 85%
last week but above your 4-week average of 75%."

This gives the user a concrete measure of follow-through over
time.

### Step 4: Set Weekly Goals

Help the user set 2-4 goals for the coming week. Goals should:

- Build on patterns identified in the review
- Address recurring blockers or gaps
- Be measurable by the end of the week
- Connect to the user's larger objectives

If the user had a low completion rate, suggest fewer but more
focused goals. If they crushed it, suggest stretching slightly.

### Step 5: Archive and Note

Flag any completed projects or milestones for Memory.md update.
Long-term achievements should move from the journal to memory
so they persist across sessions.

## Output

Write a structured weekly review entry to the journal:

```
## Weekly Review - [date range]

### Summary
- Commitments: [completed]/[total] ([percentage]%)
- Productive days: [count]
- Blockers encountered: [count]

### Patterns
- **Worked well:** [specific observation]
- **Needs attention:** [specific observation]
- **Trend:** [improving/declining/stable] vs previous week

### Goals for Next Week
1. [goal 1]
2. [goal 2]
3. [goal 3]

### Memory Updates
- [items to add to Memory.md, or "None"]
```

Maintain consistent formatting so weekly reviews can be compared
across months.
