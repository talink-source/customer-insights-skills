# Content-Ready Outputs

Use this mode when the interviews were filmed or recorded and the evidence will also be used to make content (short videos, quote posts, website copy, recruiter or sales messaging). It adds a moment-level clip log, a speakers sheet and a positioning check to the core analysis, and packages the conclusions as an insights summary.

Produce two files beside the transcripts:

- `insights.md`: the conclusions. It is what readers (and later sessions) read first.
- `clip-log.xlsx`: the moment-level evidence and the team's review columns. When the two disagree on a clip-level detail, the spreadsheet wins.

## Clip log (sheet "Clip log")

One row per usable moment, not per quote. A moment is a passage that could stand in a video or post, or that supports a theme.

| Column | Values and guidance |
|---|---|
| ID | `<interview-slug>-<nn>`, stable once assigned. Add new rows at the end; never renumber. |
| Interview | Interview number and name |
| Transcript file | File name of the source transcript |
| Speaker | Who says it. Mark "unclear" when the transcript can't tell. |
| Speaker role | Their role, so readers can tell frontline from leadership |
| Segment | Part of the interview, when it was recorded in segments |
| Start, End | Timecodes of the transcript block(s) |
| Est. length (sec) | Approximate spoken length |
| Quote (verbatim) | Exact transcript text, errors included. Never polish. |
| Summary | One sentence in plain words |
| Themes | Theme IDs from the evidence map, separated by semicolons (`T1;T5`), plus `ORIGIN` or `CASE` where relevant |
| Content bucket | The content type it best serves (for example, origin story, why-us, case story, social quote) |
| Format | story, quote, list, explanation |
| Value prop | Which value proposition it supports, or `none` |
| Alternative left | The alternative the person left behind (for example, stay at current employer, go independent), or `none` |
| Certainty | validated, inferred, hypothesis |
| Prompted | `answer_to_open_question`, `answer_to_leading_question`, or `unprompted` |
| Stands alone | `yes`, `needs_setup`, `no` |
| Strength (1-5) | How strong the moment is as evidence and as content |
| Compliance flags | `none`, or a list: names a hospital/employer/client, patient or client identifiable, criticizes a named party, medical or legal claim needs review, policy claim needs HR, consent needed, mental-health line |
| Workstreams | Which uses it serves |
| Notes | Setup needed, edits, cautions |
| Tier | Formula: A if strength ≥ 5, stands alone = yes and no compliance flags; B if strength ≥ 4 and stands alone ≠ no; otherwise C |
| Review columns | Speaker confirmed (Y/N), On-camera quality (1-5), Team pick (Yes/Maybe/No), Reviewer, Reviewer notes. Leave blank for the team. |
| Used in | The output that uses it (for example, a video ID). Keep it current when picks change. |

## Speakers (sheet "Speakers")

One row per person: interview, speaker, role, whether they speak firsthand or secondhand, their situation before (with timecodes), relevant life context, and **interviewer notes**. Interviewer notes record leading or presupposing questions with timecodes, words the interviewer introduced that the speaker then repeated, scripted prompts, and gaps or off-mic stretches. This sheet is what lets a later step explain why a planned piece can't be supported and slate an alternative.

## Evidence map and counts

Copy the evidence table into a sheet "Evidence map". Add a "Counts" sheet with usable moments by theme and tier (formulas over the clip log, with ranges that cover every row).

## Positioning check

When the company has a positioning document, canvas or EVP, add a table (in `insights.md` and as a sheet):

| Element | Verdict | What the interviews show | Evidence (speaker, timecode) | Recommendation |
|---|---|---|---|---|

Verdicts: Strongly supported, Supported, Mixed or tension, Not addressed, No evidence. Recommendations are proposals; never change the positioning document from this step.

## Insights summary (`insights.md`)

Use these sections, in this order:

1. Status line (date, author, approval state) and a short source and method note
2. **Bottom line:** the ranked strongest problems, in plain words
3. **Sample caveats:** who is firsthand vs. secondhand, interview conditions (who interviewed, leading questions), survivorship, transcript quality, and who is not covered
4. **Evidence map:** one subsection per theme with the full chain, severity, quotes and who supports it
5. **Positioning check** (when applicable)
6. **Hypotheses still to validate**
7. **Usable inventory:** counts by tier and rough ranges by content type
8. **Before public use:** the checks that must clear before external use
9. **Recommended next interviews:** next personas, assumptions to test, and 3 to 5 behavioral questions (see [interview-guide.md](interview-guide.md))

## Content-mode checks

Before returning, confirm:

- Every quote in the clip log matches its transcript exactly (check programmatically when you can).
- Every clip has a speaker; uncertain ones are marked "unclear" and listed for confirmation.
- Every leading or scripted prompt is recorded in the speakers sheet, and the matching clips are marked `answer_to_leading_question`.
- Compliance flags are set before tiers are trusted.
- The Counts formulas cover the full clip log range.
