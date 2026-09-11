---
name: customer-evidence-mapper
description: Analyze qualitative customer interview transcripts into defensible problem chains, evidence-backed product insights, validation gaps, and recommended follow-up interviews. Use for customer discovery synthesis and opportunity mapping; do not use for ordinary transcript summaries.
---

# Customer Evidence Mapper

Turn interviews into the smallest useful set of high-severity, well-evidenced customer problems. Do not summarize interviews chronologically or make conclusions more certain than the evidence permits.

Read [references/framework.md](references/framework.md) for detailed field definitions, evidence rules, and row-quality criteria.

## Core reasoning model

Build each insight as a defensible causal chain:

`Persona -> Type of Org -> Use Case -> Current Way -> Limitation -> Problem -> Severity -> New Way -> Feature -> Benefit -> Wow Factor -> Evidence`

Every field must follow logically from the prior field. If evidence cannot support part of the chain, qualify it, mark it as needing validation, or omit the row.

Maintain three levels of certainty:

- **Validated:** the interviewee directly described the workflow, problem, consequence, severity, or desired outcome.
- **Inferred:** the conclusion reasonably follows but was not explicitly stated. Signal this in the relevant cell with wording such as “Inferred from…”
- **Hypothesis:** the conclusion requires further evidence. Label it “Hypothesis,” “Potentially,” or “Needs validation.”

Do not add an evidence-classification column unless the user asks for it.

## Analyze the evidence

1. Read first for jobs, behavior, workarounds, friction, uncertainty, consequences, frequency, urgency, and priorities. Initially set aside proposed features.
2. Group related evidence into problem chains. Multiple quotes may support one row; do not create a row for every quote.
3. Assign each problem to the person who directly experiences it. Separate practitioner, manager, buyer, administrator, and end-customer problems when their workflows or consequences differ.
4. Distinguish firsthand accounts from claims about other people. Treat secondhand claims as weaker evidence and label that limitation when material.
5. Assess severity from `frequency x impact x urgency`, using only transcript evidence. Never infer severity from the appeal of a possible solution.
6. Describe the improved behavior as the **New Way** before naming a **Feature**. Map only the smallest plausible capability that could enable it.
7. Keep the **Benefit** to a credible first- or second-order outcome. Do not present downstream revenue, churn, retention, or profitability effects as established without direct evidence.
8. Express the **Wow Factor** in concise customer-facing language without strengthening the claim.

For multiple interviews, synthesize rather than concatenate. Consider recurrence, persona, organization context, workflow similarity, severity, workarounds, and contradictions. Label evidence from only one interview as an emerging signal, not a market-level conclusion. Report meaningful contradictions and examine whether role, size, maturity, industry, business model, stack, or complexity explains them.

## Produce the output

Start with a Markdown table using these exact columns and order:

| Persona | Type of Org | Use Case | Current Way | Limitation | Problem | Severity | New Way | Feature | Benefit | Wow Factor | Evidence / Quote |
|---|---|---|---|---|---|---|---|---|---|---|---|

Then include these sections:

### Strongest Validated Problems

Identify the 3–5 strongest chains as `Persona -> Problem -> Why it matters`. Rank evidence strength and severity above novelty.

### Hypotheses That Still Need Validation

For each strategically interesting but unproven conclusion, state:

- **Evidence says:** what the interviews established.
- **Hypothesis:** what may follow.
- **Needs validation:** what evidence would raise confidence.

### Evidence Gaps

Call out missing firsthand interviews, unclear frequency or severity, unknown current workarounds, unknown willingness to change or pay, untested features, and assumed downstream outcomes when applicable.

### Recommended Next Interviews

Recommend the next persona, the assumption to test, and the evidence that would change confidence. Include 3–5 behavioral questions focused on a specific past event, actual steps, participants, time, frequency, consequences, workarounds, and urgency. Avoid leading feature-preference questions unless the user specifically requests concept testing.

## Integrity constraints

- Preserve exact quotes and correct attribution. Never invent, polish, splice, or reframe a paraphrase as a quotation.
- Do not assume that the interviewee, buyer, or senior decision-maker is the affected persona.
- Keep **Current Way**, **Limitation**, and **Problem** distinct: behavior, structural weakness, and resulting consequence.
- Treat customer feature requests as possible solution evidence, not proof of a severe underlying problem.
- Use clear customer language rather than abstract business jargon.
- Do not manufacture quantitative claims or generic ROI language.
- Prefer fewer strong rows over a large table of weak or repetitive findings.

Before returning the analysis, audit every row against [references/framework.md](references/framework.md). Rewrite, downgrade, flag, or remove any row that fails.
