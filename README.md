# Customer Insights Skills

Skills for turning qualitative customer research into structured, evidence-backed product decisions.

## Featured skill: Customer Evidence Mapper

**Customer Evidence Mapper** analyzes one or more customer interview transcripts to identify the strongest validated problems, current workflows, limitations, desired outcomes, potential product capabilities, and research gaps.

It explicitly separates:

- what customers said;
- what the evidence reasonably suggests;
- what remains an unvalidated hypothesis;
- and what a team may choose to build.

### Skill files

| File | Purpose |
|---|---|
| [SKILL.md](skills/customer-evidence-mapper/SKILL.md) | Skill entry point, reasoning model, routing, and core integrity constraints |
| [Column definitions](skills/customer-evidence-mapper/references/column-definitions.md) | Detailed guidance and examples for every evidence-mapping column |
| [Evidence integrity](skills/customer-evidence-mapper/references/evidence-integrity.md) | Validation levels, quotation rules, persona integrity, and feature/benefit discipline |
| [Analysis process](skills/customer-evidence-mapper/references/analysis-process.md) | Complete eight-step workflow and recommended behavioral interview questions |
| [Multi-interview synthesis](skills/customer-evidence-mapper/references/multi-interview-synthesis.md) | Cross-interview synthesis, segmentation, contradictions, and customer language |
| [Output and quality check](skills/customer-evidence-mapper/references/output-and-quality-check.md) | Required deliverables, prohibited shortcuts, and the row-by-row final audit |
| [Employee interviews](skills/customer-evidence-mapper/references/employee-interviews.md) | Employee mode: how each column changes for EVP and employer-brand research, and the biases to flag |
| [Content-ready outputs](skills/customer-evidence-mapper/references/content-outputs.md) | Clip log, speakers sheet, positioning check and insights summary for filmed or recorded interviews |
| [Interview guide](skills/customer-evidence-mapper/references/interview-guide.md) | Behavioral question guide, leading-question rewrites and an interviewer briefing |
| [Codex metadata](skills/customer-evidence-mapper/agents/openai.yaml) | Display name, skill description, and default invocation prompt |

## Modes

- **Customer** (default): product and customer discovery.
- **Employee:** EVP, recruiting, retention and employer-brand research with a company's own people. The chain stays the same; "Current Way" becomes life before joining, and "Feature" becomes the employer capability.
- **Content-ready** (add-on): for filmed or recorded interviews whose evidence will feed content. Adds a clip log, a speakers sheet with notes on leading questions, a positioning check, and an `insights.md` summary.
- **Interview guide:** plans behavioral, non-leading questions and an interviewer briefing before the interviews happen.

## What it produces

The skill creates a structured evidence table following this causal chain:

```text
Persona → Type of Org → Use Case → Current Way → Limitation → Problem
→ Severity → New Way → Feature → Benefit → Wow Factor → Evidence
```

It then identifies:

1. The strongest validated customer problems
2. Hypotheses that still need validation
3. Important evidence gaps
4. The next personas and behavioral questions to research

In content-ready mode it also produces `insights.md` and `clip-log.xlsx` (clip log, speakers, evidence map, counts and positioning check sheets).

## Use it

Invoke the skill with an interview transcript or a set of interviews:

```text
Use $customer-evidence-mapper to analyze these customer interviews.
```

Other examples:

```text
Use $customer-evidence-mapper in employee mode, content-ready, on these filmed interviews.
Use $customer-evidence-mapper to write an interview guide for next month's interviews.
```

The skill is designed for product, research, marketing, people and leadership teams conducting customer discovery, opportunity analysis, or employer value proposition research. It is not intended for ordinary transcript summaries.

## Repository structure

```text
skills/
└── customer-evidence-mapper/
    ├── SKILL.md
    ├── agents/
    │   └── openai.yaml
    └── references/
        ├── analysis-process.md
        ├── column-definitions.md
        ├── content-outputs.md
        ├── employee-interviews.md
        ├── evidence-integrity.md
        ├── interview-guide.md
        ├── multi-interview-synthesis.md
        └── output-and-quality-check.md
```

## License

Released under the [MIT License](LICENSE).
