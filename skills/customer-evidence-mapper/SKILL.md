---
name: customer-evidence-mapper
description: Analyze qualitative customer interview transcripts into defensible problem chains, evidence-backed product insights, validation gaps, and recommended follow-up interviews. Use for customer discovery synthesis and opportunity mapping; do not use for ordinary transcript summaries.
---

# Customer Evidence Mapper

Turn interviews into the smallest useful set of high-severity, well-evidenced customer problems. The job is analysis, not transcript summarization. Never make a conclusion more certain than the interview evidence permits.

## Required references

Read the references that govern the requested analysis:

- Always read [column-definitions.md](references/column-definitions.md) before constructing the framework table.
- Always read [evidence-integrity.md](references/evidence-integrity.md) before classifying or quoting evidence.
- Always read [analysis-process.md](references/analysis-process.md) before analyzing one or more transcripts.
- When two or more interviews are provided, also read [multi-interview-synthesis.md](references/multi-interview-synthesis.md).
- Always read [output-and-quality-check.md](references/output-and-quality-check.md) before drafting and again before returning the final answer.

## Core reasoning model

Build each insight as a defensible causal chain:

`Persona -> Type of Org -> Use Case -> Current Way -> Limitation -> Problem -> Severity -> New Way -> Feature -> Benefit -> Wow Factor -> Evidence`

Every field must follow logically from the prior field. If evidence cannot support part of the chain, qualify it, mark it as needing validation, or omit the row.

Maintain three levels of certainty:

- **Validated:** the interviewee directly described the workflow, problem, consequence, severity, or desired outcome.
- **Inferred:** the conclusion reasonably follows but was not explicitly stated. Signal this in the relevant cell with wording such as “Inferred from…”
- **Hypothesis:** the conclusion requires further evidence. Label it “Hypothesis,” “Potentially,” or “Needs validation.”

Do not add an evidence-classification column unless the user asks for it.

## Integrity constraints

- Preserve exact quotes and correct attribution. Never invent, polish, splice, or reframe a paraphrase as a quotation.
- Do not assume that the interviewee, buyer, or senior decision-maker is the affected persona.
- Keep **Current Way**, **Limitation**, and **Problem** distinct: behavior, structural weakness, and resulting consequence.
- Treat customer feature requests as possible solution evidence, not proof of a severe underlying problem.
- Use clear customer language rather than abstract business jargon.
- Do not manufacture quantitative claims or generic ROI language.
- Prefer fewer strong rows over a large table of weak or repetitive findings.

The analysis must let readers distinguish what customers said, what the evidence suggests, what remains hypothetical, and what the team may choose to build. Before returning it, use the full audit in [output-and-quality-check.md](references/output-and-quality-check.md). Rewrite, downgrade, flag, or remove any row that fails.
