# Product Scope Document

> Every product must complete this document before any code is written.
> This is the decision record — what we chose, what we rejected, and why.

---

## 1. The Problem

**One sentence:**
> A specific person has a specific problem, and here's why existing solutions don't solve it.

**Detail:**
- Who experiences this problem? (job title, demographic, behavior)
- How often do they experience it?
- How severely does it affect them?
- What do they currently do about it?
- Why aren't existing solutions good enough?

## 2. The Solution

**One sentence:**
> We build X, which lets Y do Z that they couldn't do before / do much better.

**The core interaction (the ONE thing that must work):**
```
User arrives → [does what?] → gets what outcome?
```
If this interaction fails, the product fails. Everything else is secondary.

## 3. Scope Boundaries

| What we DO build | What we do NOT build (yet) |
|------------------|---------------------------|
| ...              | ...                       |
| ...              | ...                       |

**Feature amendment criteria:**
> What specific evidence from real users would justify adding something new?
> (Not "founder thinks it's cool" — real, observed user behavior.)

## 4. Why We're Building This

- **Market signal:** What data tells us this is worth doing?
- **Why now:** What makes this time different from six months ago?
- **Our advantage:** Why us and not someone else?
- **If we don't build this:** What is the cost of inaction?

## 5. Customer Discovery Protocol

> Talk to real humans before writing code. This section is your interview plan.

### 5a. Who to Talk To

**Target profile:** (specific job titles, company types, behaviors)
- Who experiences this problem most acutely?
- Where can we find them? (communities, LinkedIn groups, Slack workspaces)

**Prioritization:** Rank prospects by how close they are to the problem.

| Priority | Persona | Where to find them | Outreach channel |
|----------|---------|-------------------|-----------------|
| P0 | | | |
| P1 | | | |
| P2 | | | |

**Target: 10-15 interviews before making a build decision.**

### 5b. What to Ask

**Core questions** (past behavior, not future hypotheticals):
1. "Tell me about the last time you dealt with [problem]."
2. "What did you do to solve it?"
3. "What did that cost you? (time, money, frustration)"
4. "What have you tried that didn't work?"
5. "What would an ideal solution look like to you?"

**Question audit** — Before using, check each question for:
- [ ] Is it leading the respondent? ("Don't you think...?")
- [ ] Is it about the future? ("Would you use...?") → Rewrite about the past
- [ ] Is it too broad? ("Tell me about your workflow")
- [ ] Will it produce a socially desirable answer?

### 5c. Post-Interview Analysis

After every 5 interviews, synthesize:

```
Evidence that SUPPORTS our hypothesis:
1. _________________________________
2. _________________________________

Evidence that CHALLENGES our hypothesis:
1. _________________________________
2. _________________________________
```

**Then ask:** Is the asymmetry in these lists real, or is it what we wanted to find?

### 5d. Outreach & Scheduling

- [ ] Prospect list compiled
- [ ] Outreach sequence drafted
- [ ] Scheduling process defined
- [ ] Tracking sheet set up (status, follow-up cadence, completion)

---

## 6. Counterarguments (MANDATORY)

Write the strongest case AGAINST this product:

1. _________________________________________________
2. _________________________________________________
3. _________________________________________________

For each counterargument, note what would have to be true for it to be wrong.

## 7. Unit Economics

| Item | Cost |
|------|------|
| API cost per user action | $ |
| Infrastructure per user/month | $ |
| Payment processing | $ |
| **Total cost per paying user/month** | **$** |

| Pricing tier | Price | Users to break-even |
|-------------|-------|-------------------|
| Basic | $/mo | N = |
| Pro | $/mo | N = |

## 8. What Success Looks Like

**Week 1:** _________________________________________________
**Month 1:** ________________________________________________
**Month 3:** ________________________________________________

**The metric that tells us we're wrong:**
> If X doesn't happen by Y date, we kill this product.

## 9. Architectural Principles

- Tech stack decisions and why:
- What we explicitly avoid and why:
- Deployment target:

## 10. Security & Compliance

Before any user touches this product:
- [ ] Auth/session review (or explicitly not needed — state why)
- [ ] Secrets management (no hardcoded keys)
- [ ] Input validation / injection risks
- [ ] Data exposure in API responses
- [ ] Dependency vulnerability scan
- [ ] Cost verification (infra + API actually matches projections)

---

*Completed by: ______ | Date: ______*
*Founder reviewed on: ______*
