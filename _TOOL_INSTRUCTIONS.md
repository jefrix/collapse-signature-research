# Tool Instructions

This file is the first document any AI tool should read when pointed at
this repository. It explains how to navigate the project, where to find
relevant materials, and where to commit outputs.

## What this repository is

This is the private research workspace for The Collapse Signature, a
book and dispatch project by Jeff Ricks. The project's full description
is in `tools/CollapseSignature_Foundation.docx`. Read that document first
if you have not already done so.

## Reading order for first-time access

1. `tools/CollapseSignature_Foundation.docx` — project overview,
   methodology, four research streams, and your possible roles.
2. `methodology/` — the operating methodological framework, especially
   the Stream Three method memo. This memo sets the standards every
   case brief and dispatch is held to.
3. The folder relevant to your assigned stream:
   - SuperGrok: `streams/stream-one-data-ledger/` and
     `streams/stream-two-principal-dossiers/`
   - DeepSeek: `cases/late-tang/`, `cases/ming-consolidation/`,
     and other Chinese cases as they are added
   - Gemini: `streams/stream-two-principal-dossiers/` for ingested
     interviews; `cases/` for historical lecture summaries
   - ChatGPT: `methodology/`, plus structured-data work in
     `streams/stream-one-data-ledger/`
   - Perplexity: this is a verification tool; check whichever folder
     contains the claim that needs verification

## Where to commit outputs

Commit your outputs to the folder that matches the stream and case
you are working on. Use clear, dated filenames. Examples:

- `streams/stream-one-data-ledger/supergrok-daily-2026-05-08.md`
- `cases/ming-consolidation/deepseek-case-brief-2026-05-15.md`
- `streams/stream-two-principal-dossiers/altman/gemini-axios-interview-2026-04-22.md`
- `synthesis/jeff-weekly-2026-05-12.md`

For principal dossiers, create a subfolder per principal as needed
(e.g., `streams/stream-two-principal-dossiers/altman/`,
`streams/stream-two-principal-dossiers/fink/`).

## File format conventions

Markdown (.md) is preferred for new outputs. Word documents (.docx) are
acceptable when they are the format a primary source arrived in or
when extensive formatting matters.

Every output should include at the top: tool name, date, stream/case,
confidence level summary, and a one-sentence purpose statement.

## Source citation requirements

Every factual claim must cite its source with a URL or full bibliographic
reference. Distinguish three categories:

- Verified primary-source data (direct quote or data from primary source)
- Secondary-source synthesis (paraphrased from primary or scholarly source)
- Analytical inference (your own reasoning, marked clearly as such)

Use the five-level confidence taxonomy from the Stream Three method
memo: A (contemporaneous primary), B (strong reconstruction with
multiple sources), C (contested or single-source), D (analytical
inference), E (speculative).

## Coordination

Jeff is the central coordinator. Output goes to him first. For editorial
review on dispatches and book chapters, Claude is the editorial pass.

If you need a tiebreaker on an analytical disagreement with another
tool, surface both positions to Jeff with the reasoning behind each.
Do not assume any one tool's claims override another's.

## Relay filing for read-only tools

DeepSeek can read the repository but cannot push. Jeff relays DeepSeek
output into a Claude session, and Claude commits it **verbatim** to the
matching case or stream folder. Each relayed file gets a header naming
the tool, date and stream/case, plus a filing note saying it was relayed
and committed by Claude. Claude's review of the relayed work goes in a
separate file. Relayed content is never edited in place.

## Conflict-of-interest rule (disclose, do not hand off)

When a tool's own developer is a subject of the research, the tool **may**
do the analysis, including codings, signal resolutions, self-indictment
assessments and synthesis rulings. It must **disclose the conflict** in
the file, in a line near the top:

> **Conflict disclosure:** [Tool] is developed by [company], which is a subject of this entry.

This applies to Claude on Anthropic, Gemini on Google/DeepMind, and
ChatGPT on OpenAI, and to any similar case.

- Disclose at the file level, and again inline at any coding that bears
  directly on the conflicted developer.
- Reviewers should give conflicted codings an extra check. No handoff is
  required.
- Jeff may still assign a specific item to a non-conflicted tool when he
  wants an independent read.

History: Aug 17, 2026 rule required handoff (Claude off Anthropic-coded
analysis). Changed to disclose-not-hand-off by Jeff on Nov 22, 2026.
Codings that were marked "unreviewed placeholder" under the old rule
stand as disclosed Claude codings unless re-coded.

## Updates to this file

This file will be updated as the project evolves. Check the most recent
version before assuming any specific instruction is current.

---

Last updated: Nov 22, 2026 by Claude (Anthropic): conflict rule changed to disclose instead of hand off
