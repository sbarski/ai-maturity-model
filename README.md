# AI Maturity Model for Software Developers
The AI Maturity Model helps software developers figure out whether they're still copy pasting from Claude or ChatGPT and pretending they didn't, or actually letting AI run the show. It gives each level a clear boundary, a key signal, and enough honesty to make self assessment uncomfortable. The goal is to make the gap between where you are and where you need to be so obvious, you can't ignore it over lunch.

## Level 1: Ad Hoc Experimentation

**Boundary:** AI answers random prompts. Nobody would call this a workflow with a straight face.

**Key signal:** You copy paste from ChatGPT and then rewrite most of it anyway.

**Developer:**

- Uses AI when they remember it exists
- Typical use: syntax help, snippets, explanations, first drafts
- Treats AI output as "sometimes helpful, sometimes confidently wrong"

**Organization:**

- No standard tools, workflows, or system integration
- No visibility into who's using what
- Policy is mostly "please don't paste secrets into weird websites"

---

## Level 2: AI as an Assistant to the Developer

**Boundary:** AI is a helper, not a teammate. Useful, but still on probation.

**Key signal:** AI wrote some of the code in your last PR, but you'd never bring that up in the review.

**Developer:**

- Uses AI regularly for day to day coding
- AI contributes pieces of work, not whole deliverables
- Developer is still driving; AI is riding shotgun and occasionally being useful

**Organization:**

- Approved AI tools exist
- Usage is common but uneven. Some teams swear by it, others swear at it
- Microsoft Copilot is used or mandated. Sadly.

---

## Level 3: Developer as an Assistant to AI

**Boundary:** AI completes bounded, single tasks end to end. The human kicks each one off.

**Key signal:** You hand AI a task and go make coffee. When you get back, it's done.

**Developer:**

- Delegates most programming tasks to AI, one at a time
- Human code review is only done on critical systems or components
- Developer focuses on what to build and whether it's right, not how to build it

**Organization:**

- AI is used across multiple SDLC stages, but each use is human triggered
- AI has read/write access to selected systems: repos, docs, tickets
- AI is part of how work gets done, not just a clever side habit

---

## Level 4: Agentic Engineering

**Boundary:** AI chains across tools and stages without being re prompted at each step. It's driving. You're in the passenger seat watching the road.

**Key signal:** AI read the ticket, wrote the code, opened the PR, and pinged you to review. You didn't ask it to do any of those steps individually.

**Developer:**

- Defines an objective; AI figures out the plan, writes the code, tests it, and iterates
- AI moves across contexts on its own: feature, PR, CI, triage, retry
- Developer manages the system, not each output

**Organization:**

- AI is wired into engineering systems: repos, CI/CD, docs, tickets, observability
- Guardrails, approvals, audit logs, and rollback paths in place
- When AI goes off the rails, there's an actual process. Not just someone yelling in Slack

---

## Level 5: Governed Autonomous Engineering

**Boundary:** AI operates toward ongoing goals within policy. Powerful, but not feral.

**Key signal:** You review what AI accomplished this week, not what it's doing right now.

**Developer:**

- Sets goals, constraints, policies, and acceptance criteria
- AI does all of the engineering work. 
- Human steps in for escalations, novel problems, or when AI gets creative in ways nobody asked for

**Organization:**

- AI performs substantial autonomous work across delivery and operations
- Autonomy is policy bounded, observable, and reversible
- Fallback modes exist for when AI becomes degraded, unavailable, or suddenly very confident and very wrong
