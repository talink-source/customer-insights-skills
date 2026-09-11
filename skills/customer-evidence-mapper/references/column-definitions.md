# Column Definitions

Produce a table using these exact columns:

| Persona | Type of Org | Use Case | Current Way | Limitation | Problem | Severity | New Way | Feature | Benefit | Wow Factor | Evidence / Quote |
|---|---|---|---|---|---|---|---|---|---|---|---|

## Persona

**Question:** Who directly experiences the problem?

Identify the specific role whose workflow, pain, or outcome is described: individual contributor, team lead, department head, owner, administrator, end user, or customer. Do not confuse the economic buyer, decision-maker, manager, interviewee, or presumed target market with the affected person.

If an employee performs the difficult workflow, the employee is the persona even if a manager buys the solution. A manager struggling to create team consistency is a separate problem. A negative consequence experienced by an end customer may warrant another row. Split rows only when personas experience meaningfully different problems.

## Type of Org

**Question:** What environment makes the problem especially relevant?

Include only characteristics that explain why the problem exists or how it manifests: industry, business model, company or team size, maturity, operational complexity, technology, customer model, centralized versus distributed operations, high-touch versus self-service, or new versus established organization. Prefer supported specificity over generic labels.

## Use Case

**Question:** What is the persona trying to accomplish?

State the job, goal, or workflow independently of any product. It should remain valid if the proposed solution did not exist.

Good examples:

- Understand a customer’s situation before deciding how to respond.
- Identify accounts that may require attention.
- Coordinate work across multiple team members.
- Introduce a process without disrupting existing operations.

Product interactions such as “use the dashboard,” “configure the integration,” “use AI insights,” or “receive notifications” are not use cases.

## Current Way

**Question:** How do they accomplish the use case today?

Describe the actual behavior, workflow, tools, or workaround: software, spreadsheets, email, messaging, meetings, manual processes, memory, judgment, SOPs, system switching, or asking others for context. Prefer “They check several systems, compare the information, and contact another team member when context is missing” over “They do it manually.”

## Limitation

**Question:** Why does the current way fall short?

Name the structural weakness, such as fragmented information, reliance on individual memory, manual detection, repetitive entry, late information, inconsistent team processes, or data without context. Do not repeat the problem.

## Problem

**Question:** What negative consequence does the limitation create?

Answer “So what?” Distinguish the chain:

- Current Way: Users check several systems before acting.
- Limitation: Relevant information is fragmented.
- Problem: Users spend significant time reconstructing context before deciding what to do.

Another valid chain is manual monitoring -> dependence on individual attention -> important situations go unnoticed until they are harder to address.

## Severity

**Question:** How much does the problem actually matter?

Assess `Frequency x Impact x Urgency`. Use `Low`, `Medium`, `Medium-high`, `High`, or `Very high`, followed by a brief evidence-based explanation.

- Very high: explicitly a top operational priority or severe recurring consequence.
- High: frequent workflow with meaningful time, cost, risk, or customer impact.
- Medium: acknowledged issue with a workable alternative or moderate consequence.
- Low: infrequent issue with little operational consequence.

Look for repeated mentions, strong emotion, measurable cost, time consumed, lost customers, missed opportunities, risk, revenue impact, turnover, workarounds, executive attention, explicit priority, urgency, and frequency. Never infer severity because a solution sounds valuable. If severity is not established, say so.

## New Way

**Question:** What should the persona be able to do instead?

Describe an improved behavior or workflow conceptually and mostly product-agnostically. For example: “The user sees relevant context together before deciding what action to take.” Avoid prematurely prescribing UI, implementation, architecture, technology, AI, or automation. Prefer “The user is proactively shown meaningful changes” over “An AI assistant sends an alert.”

## Feature

**Question:** What product capability could enable the New Way?

Possible capabilities include unified profiles, integrations, automated alerts, historical activity views, recommendations, workflow automation, permissions, reporting, collaboration, search, and synchronization. Features are often hypotheses. A validated problem does not validate a specific feature. Reason `Problem -> New Way -> Potential Feature`, never `Feature Idea -> Invented Problem`.

## Benefit

**Question:** What gets better immediately?

State the specific, believable first-order outcome: less time gathering information, earlier identification, less repetitive work, better decision context, less system switching, faster response, greater consistency, or fewer errors. Do not jump to revenue, churn elimination, profitability, competitiveness, or lifetime value without the additional causal evidence.

## Wow Factor

**Question:** What is the most compelling truthful expression of the immediate benefit?

Make it specific, clear, immediate, emotionally relevant, and grounded:

- Identify situations sooner -> “Know what needs your attention without hunting for the signal.”
- Reduce context gathering -> “Start with the full picture instead of piecing it together yourself.”
- Reduce administration -> “One less thing to manage—not one more.”

Amplify the benefit without exaggerating it. “Identify changes sooner” must not become “Never lose another customer.”

## Evidence / Quote

**Question:** What in the interview supports the conclusion?

Prefer exact quotes that validate the current way, limitation, problem, severity, or desired outcome. Strong quotes contain specificity, emotion, priority, frequency, measurable consequences, detailed examples, comparisons, or workarounds. Follow all quote-integrity rules in [evidence-integrity.md](evidence-integrity.md).
