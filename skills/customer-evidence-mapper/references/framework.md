# Evidence Mapping Framework

Use this reference while constructing and auditing the evidence table.

## Field definitions

### Persona

Name the role that directly experiences the workflow, pain, or consequence. Do not substitute a buyer, manager, or interviewee for the affected person. Create separate rows only when distinct personas experience meaningfully different problems.

### Type of Org

Describe only organizational characteristics that explain why the problem exists or how it manifests: industry, business model, size, maturity, team structure, operational complexity, technology, customer model, or centralization.

### Use Case

State the job or outcome the persona is trying to accomplish independently of any proposed product. “Understand a customer’s situation before responding” is a use case; “use an AI dashboard” is not.

### Current Way

Describe observed behavior, tools, workflow, or workaround concretely. Name systems, manual steps, meetings, messages, judgment, memory, handoffs, or system switching when the transcript establishes them.

### Limitation

Name the structural weakness of the current approach, such as fragmented information, dependence on memory, manual monitoring, repetitive entry, late information, inconsistent processes, or data without context.

### Problem

State the tangible negative consequence created by the limitation. Answer “So what?” Do not restate the limitation.

### Severity

Use `Low`, `Medium`, `Medium-high`, `High`, or `Very high` and briefly explain the rating. Base it on frequency, impact, and urgency supported by repeated mentions, emotional language, measured cost, time, missed opportunities, operational risk, workarounds, executive attention, prioritization, or urgency. If severity cannot be established, say so.

### New Way

Describe the improved behavior or workflow conceptually and mostly product-agnostically. Avoid prematurely prescribing interface, architecture, AI, or automation.

### Feature

Name the smallest plausible capability that could enable the New Way. Label it as a hypothesis unless the customer explicitly validated that capability. Reason from problem to workflow to capability, never backward from a favored feature.

### Benefit

Describe the specific, believable first-order improvement: less time gathering information, earlier detection, less repetitive work, better context, fewer system switches, faster response, greater consistency, or fewer errors. Avoid distant commercial outcomes without evidence.

### Wow Factor

Translate the immediate benefit into compelling, concise customer-facing language. Amplify clarity, not certainty. For example: “Start with the full picture instead of piecing it together yourself.”

### Evidence / Quote

Use exact, attributed quotes when available. Prefer evidence showing specificity, emotion, prioritization, frequency, measurable consequences, examples, comparisons, or workarounds. If only paraphrase or secondhand evidence exists, identify it as such rather than placing it in quotation marks.

## Evidence strength

Increase confidence for repeated comments, strong emotion, specific examples, quantified consequences, operational metrics, workarounds, explicit prioritization, frequent behavior, and clear cost or risk.

Reduce confidence when the interviewee speculates about others, describes aspiration instead of current pain, proposes features without establishing a problem, speaks for an uncontacted persona, answers only after prompting, or contradicts themselves.

## Causal-distance rule

Trace potential benefits as:

`Feature -> Direct capability -> First-order benefit -> Action -> Customer outcome -> Commercial outcome`

Default to the first- or second-order benefit. Later outcomes are hypotheses unless separately evidenced.

## Behavioral interview questions

Prefer questions grounded in actual past behavior:

- Tell me about the last time this happened.
- Walk me through exactly what you did.
- What happened next?
- How did you know there was a problem?
- Where did you look for the information?
- Who else was involved?
- How long did that take, and how often does it happen?
- What happens if you do not solve it?
- What have you tried instead?
- When does this become urgent?

Avoid “Would you use this feature?”, “Would AI solve this?”, or “Would you pay for this?” during problem discovery. Those may be appropriate later for concept testing but cannot replace behavioral evidence.

## Final row audit

For every row, verify:

1. **Persona:** Is this the person who directly experiences the problem?
2. **Type of Org:** Does this context explain where or why the problem occurs?
3. **Use Case:** Is this a customer job rather than a product interaction?
4. **Current Way:** Did the interview establish how they do it today?
5. **Limitation:** Is this what is structurally weak about the approach?
6. **Problem:** Is this the consequence rather than a restatement?
7. **Severity:** Is there evidence that it matters, with uncertainty acknowledged?
8. **New Way:** Does this describe a better workflow before implementation?
9. **Feature:** Does the capability enable the New Way, with hypothesis status clear?
10. **Benefit:** Is this a believable first-order outcome?
11. **Wow Factor:** Is it compelling without exceeding the evidence?
12. **Evidence:** Would the quote or paraphrase let a reader understand why the insight exists?

If any answer is no, rewrite, downgrade, flag, or remove the row.
