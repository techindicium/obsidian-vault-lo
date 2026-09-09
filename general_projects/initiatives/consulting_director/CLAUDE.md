# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## What this repository is

This is **not a software codebase** — it's Lorena Santos's working repository for the **Consulting Director (CD)** global initiative at Indicium: product discovery, PRDs, and meeting records for problems raised by CD stakeholders (chiefly Pedro Portela — "PP"). There is no build, lint, or test suite for the repository as a whole. The one exception is `discovery/discovery_app/`, a standalone HTML app — see its own section below.

Treat this repo as a knowledge base to read, extend, and keep internally consistent, not as code to compile.

## Directory structure

- `initial_context/` — source material mined *before* any discovery starts. `core_problems.md` is the canonical list of raised problems (issues), each with impact, known root cause, and correct process where already documented. Read this first for any new initiative — it defines what's already known vs. what discovery still needs to answer.
- `discovery/` — active discovery work, one initiative at a time (currently: EX Account Health, CRM/Commissions). See "Discovery convention" below for the file pattern used here.
- `discovery/PRD/` — both the working scratchpads (`PRD-*-scratchpad.md`) and the final PRD documents (`PRD-*.md`, following the 4D framework: Discovery → Design → Development → Delivery) for each initiative.
- `discovery/discovery-roteiro-metodologia.md` — the house methodology for running discovery: numbered steps (Passo 0–14), each with what to capture and support questions. This is a **complement** to the `prd-workflow` skill's Discovery phase (Steps 2–7), not a replacement — it's the preparation layer that runs before/during, so that by the time the skill's Discovery steps are filled in, the answers are already validated rather than first-pass guesses. The doc ends with a mapping table from its own steps to the skill's steps.
- `discovery/discovery_app/` — a standalone, dependency-free HTML interview app (question-by-question, voice input, autosave to a local JSON file) for running structured discovery interviews asynchronously. No build step. Test manually per `discovery/discovery_app/tests.md` — open `discovery_app.html` directly in a browser via `file://`.
- `meetings/` — one file per meeting, in the fixed format described below.

## Discovery convention

Each initiative under discovery uses **two files, in two languages, by design**:

- `PRD/PRD-[initiative]-scratchpad.md` — English, working notes. This is where analysis actually evolves: a Pre-Discovery Synthesis section, dated "Discovery Answers" entries (as real answers come in from stakeholders, via Slack or live meetings), a "Possible Products" section for solution ideas (explicitly non-committal until validated), a consolidated numbered "Open Questions" list (each with a *why it matters* line), a Risk & Dependency table (`R1`, `R2`, ... with mitigation plans left blank until the stakeholder provides them), and a dated, chronological **Judgment Calls Log** at the end — every correction, reversal, or decision gets its own dated entry so reasoning is never silently overwritten.
- `discovery_[initiative].md` — Portuguese, the actual question script taken into stakeholder conversations. Versioned in place (`_v2`, `_other_cds`, etc.) when the *shape* of the conversation changes materially — the old version is kept, not edited over, so prior discovery scripts remain a record of what was actually asked.

**Standing rules, load-bearing for how this repo is written:**

- **Never record real client names, real employee names, or real revenue figures** — not even when the source material (a screenshot, a spreadsheet, a prototype) contains them. Only structure (field names, layout, logic) gets copied into scratchpads or PRDs. Internal Indicium employee names used for stakeholder identification (PP, Beatriz, Igor Benincá, etc.) are fine.
- **Discovery and solutioning are separate phases — don't blur them.** A synthesized "requirement" is our interpretation until the stakeholder confirms it in their own words, even if it traces back to something they said before. Content lists, indicators, UI/format choices are hypotheses to validate, not a spec already committed to, until a stakeholder says otherwise.
- **Surface ambiguity as questions; don't resolve it unilaterally.** When a discovery script or scratchpad has gaps or seems stale against newer findings, that gets raised back as explicit questions, not silently patched.
- Large scratchpads (currently `PRD-crm-deals-commissions-scratchpad.md`) are intercepted by a context-guard hook once they cross ~10k tokens — full `Read`/`tail` gets blocked. Use targeted access instead: `Read` with `offset`/`limit`, `grep -n` or `sed -n 'X,Yp'` via Bash, or the hook's own `search_knowledge.py` for keyword search. For edits, prefer appending/inserting via a small Python script over trying to read-then-Edit the whole file.

## Meeting records (`meetings/`)

Filename pattern: `[Participant1]  [Participant2] - [topic] - YYYY_MM_DD - Resumo e Próximos Passos.md` (note the double space between the two participant names). Each file follows this fixed structure:

1. Header: **Data**, **Participantes**, **Transcrição completa** (a Google Docs link).
2. **Resumo do teor** — narrative summary of what the meeting covered and its overall shape.
3. **Pontos levantados** — bullet list of findings/decisions, one per point, bolding the key claim.
4. **Próximos passos de ação** — numbered, action-oriented, with owner where known.
5. A closing pointer (italicized) back to the relevant scratchpad section(s) in `discovery/PRD/`, since the scratchpad — not this file — holds the full quoted evidence.

When a meeting resolves an open question that lives in a scratchpad (e.g., an `Open Questions` list item, an `R#` risk row), update the scratchpad itself (with a dated Judgment Calls Log entry) in addition to writing the meeting record — the meeting file is the narrative account, the scratchpad is the source of truth other work refers back to.
