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

## Conflict-of-interest rule (subject-tool analysis)

When a tool's own developer is a subject of the research, that tool must
not take analytical lead on material coded to that developer. Analytical
lead covers register codings, signal resolutions, self-indictment
assessments, and synthesis rulings.

- **Claude** must not lead on Anthropic-coded material. Assign it to
  Gemini or DeepSeek.
- The same rule applies to any other tool whose developer is a subject.
  For example, Gemini must not lead on Google/DeepMind-coded material,
  and ChatGPT must not lead on OpenAI-coded material. Assign that work to
  a non-conflicted tool.
- A conflicted tool may still collect and cite **facts** about its
  developer, marked as fact-gathering only, and hand the coding off.
- If a conflicted tool has already written a coding, mark it at the point
  of use as an unreviewed placeholder. Do not delete it. A non-conflicted
  tool re-codes it.

Origin: Aug 17, 2026 catch-up ledger (`streams/stream-one-data-ledger/cycle-iv-catchup-ledger-2026-08-17.md`),
restated Sep 9, 2026. Added here Nov 22, 2026 after a breach in
`oct-nov-catchup-ledger-2026-11-22.md` §2.

## Updates to this file

This file will be updated as the project evolves. Check the most recent
version before assuming any specific instruction is current.

---

Last updated: Nov 22, 2026 by Claude (Anthropic): added conflict-of-interest rule
