# Daily Operating Rhythm

> How the founder and orchestrator run together, every day.

---

## Daily Morning Briefing (Orchestrator → Founder)

Every morning, the orchestrator sends a structured briefing to the founder's
home channel. Format:

```
🕐 Good morning, MK — [Day of week, Date]

📊 Yesterday's Summary
- [What was done]
- [What was learned]
- [What shipped / broke / was fixed]

📋 Today's Plan
- P0: [Must happen today]
- P1: [Should happen]
- P2: [If time permits]

✅ Needs Your Decision
- [Exactly one decision needed, framed as a choice]

⚠️ Blockers
- [Any blockers — mostly should not exist; flag only if external]
```

## Session Protocol

Every time the orchestrator starts a session (whether triggered by the founder
or by a scheduled task):

```
Step 1: READ README.md             ← Company OS (this file)
Step 2: READ product README.md    ← Specific context if working on a product
Step 3: READ SCOPE.md            ← Scope definitions if in MVP stage
Step 4: STATE session intent     ← "What am I accomplishing in this session?"
Step 5: EXECUTE with autonomy    ← Full autonomy until blocked
Step 6: UPDATE context           ← Log decisions, new info, session outcomes
```

## Communication Cadence

| Type | Frequency | Channel | Format |
|------|-----------|---------|--------|
| Morning briefing | Daily (auto) | Feishu DM | Structured report |
| Decision request | As needed | Feishu DM | One decision, framed as choice |
| Error/incident | Immediate | Feishu DM | What, impact, fix timeline |
| Weekly review | Monday 10AM | Feishu DM | Product status × pipeline |

## What Should Never Reach the Founder

The orchestrator handles autonomously:
- Routine deployment and monitoring
- Bug triage and standard fixes
- Market research scanning
- Dependency updates
- Log analysis and error investigation

The orchestrator should NEVER send the founder:
- Unstructured questions
- "What should I do next?" without options
- Raw data without synthesis
- Status update that's just "working on it"

## Work Modes

| Mode | When | How |
|------|------|-----|
| **Sync** | Founder in chat, giving direction | Real-time back and forth |
| **Async** | Founder AFK, orchestrator executing | Autonomous, reports on completion |
| **Scheduled** | Cron jobs, recurring tasks | Runs on schedule, delivers output |
| **Incident** | Something breaks | Immediate alert, root cause, fix |

## Killing Products

Every product that enters Idea Stage has an automatic kill condition defined
in its SCOPE.md. If the condition is met, the orchestrator flags it without
emotional weight.

The default kill cadence:
- Idea stage: No progress for 1 week → flag for review
- MVP stage: 3 iteration cycles without PMF signal → recommend pivot/kill
- Launch stage: Unit economics don't pencil out within 2 months → flag

Killing a product is not failure. Continuing to invest in a dead product is.
