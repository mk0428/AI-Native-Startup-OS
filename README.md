# AI-Native Company Operating System

> **One founder. One orchestrator. Zero bloat.**
>
> This document is the operating system of an AI-native company. It replaces
> org charts, hiring plans, and management layers with a repeatable system
> for turning ideas into products that matter.
>
> Inspired by Anthropic's "The Founder's Playbook: Building an AI-Native Startup."
>
> Public domain. Fork it, use it, improve it.

---

## 1. Who We Are

We are a company of two people: a founder and an orchestrator.

| Role | Who | Responsibility |
|------|-----|---------------|
| **Founder** | A human with domain expertise | Strategic direction, product definition, final judgment, customer conversations |
| **Orchestrator** | An AI agent | Research, coding, operations, automation — everything the founder shouldn't do |

There are no employees. No managers. No meetings.
The founder generates intent. The orchestrator executes direction.

## 2. How We Think

### The three capabilities

Every AI-native company rests on three pillars. We must be excellent at all three:

1. **Conversational Intelligence & Research** — An on-call expert for every domain.
   Market research, competitive analysis, customer discovery, strategic thinking partner.

2. **Agentic Coding** — The engineer who's always available, never blocked.
   Generate, test, debug, and refactor production-grade code at the speed of
   a full engineering team.

3. **Workflow Automation** — An on-demand ops team.
   Scheduling, reporting, monitoring, deployment — recurring operational work
   that happens automatically.

### The four stages

Every product we touch exists in exactly one of these stages:

```
Idea → MVP → Launch → Scale
```

A product cannot skip stages. A product cannot be in two stages at once.

### The founder's job redefined

The founder is an **orchestrator**, not an individual contributor.

```
IC mindset:   "How do I build this?"
Orchestrator: "What should be built, and who/what should build it?"
```

The founder's attention lives at the top of the stack: generating ideas and
directing the systems that carry them out. The orchestrator handles everything
below that line.

### "Build nothing" discipline

The most important skill in an AI-native company is **knowing what not to build**.

42% of startups fail because they built something nobody wanted. AI makes
building effortless, which makes this failure mode more dangerous, not less.

Building is never a shortcut past thinking.

---

## 3. The Stages — Operating Procedures

### 3A. Idea Stage

**Goal:** Problem-solution fit — real evidence that a real problem exists and
our proposed solution addresses it.

**Operating principle:** No code. Zero. Not even a "quick prototype."

#### Workflow

```
┌─────────────────────────────────────────────────────────────┐
│                     IDEA REGISTERED                          │
│   A problem statement, not a solution. Must pass the         │
│   "who, how often, how severe" test.                         │
└─────────────────────────────────────────────────────────────┘
                              │
                              ▼
┌─────────────────────────────────────────────────────────────┐
│                PHASE 1: SHARPEN THE HYPOTHESIS               │
│   Who exactly has this problem? How often? How severely?     │
│   What do they currently do about it?                        │
│   → Orchestrator writes the problem statement                │
│   → Founder reviews, corrects, approves                     │
└─────────────────────────────────────────────────────────────┘
                              │
                              ▼
┌─────────────────────────────────────────────────────────────┐
│             PHASE 2: ADVERSARIAL ANALYSIS                    │
│   Orchestrator argues AGAINST the idea:                      │
│   • Why doesn't this problem exist?                          │
│   • Why do existing solutions work well enough?              │
│   • What would a well-funded competitor's advantage be?      │
│   • Where is the confirmation bias in our reasoning?         │
└─────────────────────────────────────────────────────────────┘
                              │
                              ▼
┌─────────────────────────────────────────────────────────────┐
│              PHASE 3: CUSTOMER DISCOVERY                     │
│   Talk to real humans. Not surveys. Not assumptions.         │
│   • Who are the 10 people we should talk to?                 │
│   • What questions surface what people DO, not what they     │
│     think they would do?                                     │
│   • Orchestrator drafts questions. Founder interviews.       │
└─────────────────────────────────────────────────────────────┘
                              │
                              ▼
┌─────────────────────────────────────────────────────────────┐
│              DECISION GATE — BUILD OR NOT?                   │
│   Three questions. All three must be YES.                    │
│                                                               │
│   1. Is the problem real and specific?                        │
│      → Can we name who has it, how often, how severely?       │
│                                                               │
│   2. Does our solution address the actual problem?            │
│      → Not the problem we assumed. The one discovery          │
│        revealed.                                              │
│                                                               │
│   3. Do we have enough signal to justify building?            │
│      → Certainty is impossible. But we need enough            │
│        evidence that an MVP is a reasoned decision,           │
│        not an act of faith.                                   │
│                                                               │
│   ❌ Any NO → Back to hypothesis sharpening or kill.          │
│   ✅ All YES → Exit Idea stage. Enter MVP stage.              │
└─────────────────────────────────────────────────────────────┘
```

#### Exit criteria

Ready to leave the Idea stage when all three answers are YES.

**Common failure modes:**
- **Building before validating** — Mistaking a working prototype for evidence
- **Confirmation bias** — AI will find supporting evidence for any idea.
  Always ask it to argue against you first.
- **Premature scaling** — Expanding execution before validating demand

---

### 3B. MVP Stage

**Goal:** Evidence of product-market fit — proof that real users find the product
valuable enough to return to it, pay for it, or tell others about it.

**Operating principle:** Build only what generates evidence. Everything else is waste.

#### Workflow

```
┌─────────────────────────────────────────────────────────────┐
│             PHASE 1: WRITE THE SCOPE DOCUMENT                │
│   Before writing code, answer:                               │
│   • What does this product do? (the core interaction)        │
│   • What does it deliberately NOT do?                        │
│   • What evidence would justify adding something new?        │
│   • What are our architectural principles?                   │
│   → Save as SCOPE.md in the product directory                │
└─────────────────────────────────────────────────────────────┘
                              │
                              ▼
┌─────────────────────────────────────────────────────────────┐
│           PHASE 2: SET UP PERSISTENT CONTEXT                 │
│   Create CLAUDE.md for this project — architectural context  │
│   that every future session reads automatically.             │
│   • Dependencies, patterns, tradeoffs                        │
│   • What we chose and why                                    │
│   • What to avoid and why                                    │
│                                                               │
│   Without this, AI technical debt compounds. Every session    │
│   re-derives decisions from scratch. Codebase drifts.        │
└─────────────────────────────────────────────────────────────┘
                              │
                              ▼
┌─────────────────────────────────────────────────────────────┐
│            PHASE 3: MEASUREMENT FRAMEWORK                    │
│   Define before launch — NOT after:                          │
│   • Activation: what does a user need to do to get value?    │
│   • Retention: Day 7 target? Day 30 target?                 │
│   • Revenue: What pricing? Break-even unit economics?        │
│   • False positive: What would look like success but isn't?  │
│   → Save in product directory as MEASUREMENTS.md             │
└─────────────────────────────────────────────────────────────┘
                              │
                              ▼
┌─────────────────────────────────────────────────────────────┐
│           PHASE 4: BUILD THE MVP                             │
│   Three rules:                                               │
│   1. Ship the single core interaction first.                 │
│      One thing that must work. Nothing else.                 │
│   2. Each session starts with the scope doc + CLAUDE.md.     │
│   3. End each session by updating the context.               │
│      What was built? What decisions were made?               │
│                                                               │
│   → Orchestrator builds. Founder tests.                     │
└─────────────────────────────────────────────────────────────┘
                              │
                              ▼
┌─────────────────────────────────────────────────────────────┐
│            PHASE 5: SECURITY REVIEW                          │
│   Before any real user touches the product:                  │
│   • Authentication + session handling                        │
│   • Data exposure in API responses                           │
│   • Input validation + injection risks                       │
│   • API keys and secrets (never hardcoded)                   │
│   • Dependencies with known vulnerabilities                  │
│   → Orchestrator audits. Founder reviews findings.          │
└─────────────────────────────────────────────────────────────┘
                              │
                              ▼
┌─────────────────────────────────────────────────────────────┐
│              DECISION GATE — PMF OR PIVOT?                   │
│   After 3-5 iteration cycles, ask:                          │
│   • The Sean Ellis test: >40% "very disappointed"?          │
│   • The effort test: Is retention pulling or pushing?        │
│   • If no movement after 3 cycles → pivot or kill.          │
│                                                               │
│   ✅ PMF signal → Exit MVP. Enter Launch stage.              │
│   ❌ No signal → Back to Idea stage or kill.                 │
└─────────────────────────────────────────────────────────────┘
```

#### Exit criteria

- Users return (retention), pay (revenue), or tell others (referral)
- You can name the segment that's responding differently

**Common failure modes:**
- **AI technical debt** — Compounds. Without CLAUDE.md, codebase becomes incoherent.
- **False PMF** — Launch energy ≠ product-market fit
- **Zero-friction scope creep** — Each feature takes an afternoon, so you add them all.
  The antidote: a scope document with amendment criteria.
- **Security by inexperience** — Working code ≠ secure code

---

### 3C. Launch Stage

**Goal:** Repeatable, sustainable growth — the product deserves to exist, now prove
the business deserves to grow.

**Operating principle:** Remove the founder from every loop that doesn't need them.

#### Exit criteria

1. Growth is channel-driven — CAC, LTV, payback period are known numbers
2. Product handles production workloads — hardened, monitored, reliable
3. Operations run without founder bottlenecks — automation in place

**Common failure modes:**
- **Technical debt comes due** — The MVP shortcuts need remediation
- **Founder becomes bottleneck** — Same instinct that was an asset at MVP,
  now the constraint
- **Expansion before readiness** — New markets look like growth but dilute focus

---

### 3D. Scale Stage

**Goal:** The company is sustainable even when the founder is not running day-to-day.

#### Exit criteria (any one)

- Sustainable profitability at scale
- IPO readiness
- Acquisition readiness

All three require: systematic growth, auditable operations, defensible moat.

**Common failure modes:**
- Delegating without systems — Handing off without documentation
- GTM ceiling — Organic growth plateaus
- Organizational infrastructure — Compliance, financial controls, governance

---

## 4. How We Work Together

### Session protocol

Every session with the orchestrator follows the same pattern:

```
1. READ this CLAUDE.md (the company OS)
2. READ the product's CLAUDE.md (if working on a specific product)
3. STATE the session intent: "I need to..."
4. EXECUTE with full autonomy
5. UPDATE context at session end
```

### Communication

- **Founder → Orchestrator:** Strategic intent, product decisions, corrections
- **Orchestrator → Founder:** Status, findings, flagged decisions, completed work
- **Tone:** Direct, data-driven, no fluff

### Error handling

When the orchestrator makes a mistake:
1. Acknowledge immediately — no deflection, no "maybe"
2. Fix the root cause, not the symptom
3. Update the system so it doesn't happen again

When the founder catches a mistake:
- The orchestrator's job is to accept, understand, and remember.
- Debate is welcome on product decisions. Not on errors.

---

## 5. Project Conventions

```
~/Desktop/AI-Native-Startup-OS/
├── README.md                       ← This file. Company OS. Read at session start.
├── SCOPE.md                        ← Product scope template. Complete before building.
├── MEASUREMENTS.md                 ← Metrics framework template. Define before launch.
├── LAUNCH-CHECKLIST.md             ← Pre-launch audit. Pass before users touch it.
├── RHYTHM.md                       ← Daily operating rhythm. How we run.
├── PRODUCTS/                       ← 🟢 Products that passed Idea validation gate
│   └── [product-name]/             ←    (empty until the first one qualifies)
│       ├── README.md               ← Product-specific context
│       ├── SCOPE.md                ← What it does, what it doesn't, amendment criteria
│       ├── MEASUREMENTS.md         ← Metrics defined before launch
│       └── ...                     ← Product files
├── SKILLS/                         ← Reusable workflow definitions (~/.hermes/skills/)
└── JOURNAL.md                      ← What we learned, what we decided

Reading order: README.md → RHYTHM.md → product/README.md → product/SCOPE.md
```

---

## 6. The Security Non-Negotiable

AI-generated code is functional. It is not inherently secure.

Before any user touches any product:
- [ ] Authentication and session handling reviewed
- [ ] No secrets in code, config, or environment mismanagement
- [ ] Input validation against injection
- [ ] API response data exposure checked
- [ ] Dependencies scanned for known vulnerabilities
- [ ] Orchestrator audits → founder reviews findings

This checklist lives in every product's SCOPE.md and must be completed
before the product enters Launch stage.

---

## 7. What This System Replaces

| Traditional startup | This system |
|--------------------|-------------|
| Org chart | CLAUDE.md |
| Hiring plan | Sub-agent spawning |
| Management layers | Orchestrator |
| Standups | Async status via platform |
| Sprints | Session-based iteration |
| Board decks | Automated metrics reports |
| Security team | Automated audit protocol |
| Customer research | Structured discovery workflow |

---

*This is a living document. It evolves as we learn.*
*The operating system is the product.*
