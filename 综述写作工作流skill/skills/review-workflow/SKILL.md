---
name: review-workflow
description: Use this skill whenever the user wants to choose a review topic, build a literature search plan, screen papers, construct an evidence extraction workflow, draft or revise a review article, simulate peer review, normalize citations, or finalize a review into Word-ready form. Also use it when the user asks to turn an existing review-writing process into reusable templates, checkpoints, or project structure.
version: 1.0.0
---

# Review Workflow

A reusable skill for turning a review-writing task into a structured, traceable workflow from topic selection through final manuscript packaging.

## What this skill is for

Use this skill to help the user build or run a literature review workflow with explicit intermediate artifacts instead of ad hoc chat output.

This skill is especially useful when the user needs any of the following:

- a review topic narrowed into a workable scope
- a searchable literature plan
- screening criteria and tagging rules
- an evidence extraction table and reading-note workflow
- an outline that reflects evidence strength rather than only topic coverage
- draft writing with visible citation anchors
- revision based on reviewer-style criticism
- final citation normalization and Word-ready export rules

## Core rule

Always preserve **traceability**. Do not treat the review as a single writing task. Break it into staged artifacts with explicit outputs saved to files.

## Default workflow

Follow this sequence unless the user asks to enter at a later stage:

1. Topic framing
2. Search strategy and candidate-pool setup
3. Screening and tagging
4. Evidence extraction and fact checking
5. Outline and figure/table planning
6. Draft writing
7. Revision and critique strengthening
8. Peer-review simulation and response drafting
9. Citation normalization and Word finalization

## Required working style

- Keep research claims conservative when only title/abstract metadata is available.
- Never invent authors, titles, venues, years, DOI, PMID, results, or performance numbers.
- Distinguish formal publications from preprints.
- Keep “background evidence”, “core evidence”, and “high-risk/to-be-checked evidence” separate.
- Prefer templates and tables over loose prose when defining process.
- Make evidence visible in the prose; avoid vague phrases like “some studies show” unless citation anchors are explicit.

## Output expectations by stage

### 1. Topic framing
Produce:
- topic statement
- scope boundaries
- target years
- language/publication constraints
- expected evidence volume
- non-negotiable research integrity rules

Read [references/topic-selection-template.md](references/topic-selection-template.md) before writing this stage.

### 2. Search strategy
Produce:
- databases to use
- search terms / query logic
- inclusion of synonyms and task variants
- candidate-pool target size
- file destinations for logs and candidate tables

Read [references/search-strategy-template.md](references/search-strategy-template.md).

### 3. Screening and tagging
Produce:
- inclusion criteria
- exclusion criteria
- priority tiers
- tagging system for task / method / data / evidence type

Read:
- [references/screening-rules-template.md](references/screening-rules-template.md)
- [references/tagging-schema-template.md](references/tagging-schema-template.md)

### 4. Evidence extraction
Produce:
- structured evidence table schema
- fact-check log schema
- reading-note schema
- evidence-to-section mapping guidance

Read [references/evidence-extraction-template.md](references/evidence-extraction-template.md).

### 5. Outline and figure planning
Produce:
- section-level outline
- evidence-strength notes per section
- figure/table candidates
- chapter-to-evidence mapping

Read:
- [references/outline-template.md](references/outline-template.md)
- [references/figure-table-planning-template.md](references/figure-table-planning-template.md)

### 6. Draft writing
Produce:
- section drafts grounded in evidence
- visible citation anchors
- explicit distinction between mature evidence and exploratory claims

Read [references/drafting-and-revision-checklist.md](references/drafting-and-revision-checklist.md).

### 7. Revision
When revising, prioritize:
- making evidence visible
- reducing repetition
- sharpening comparisons
- converting abstract judgments into concrete examples
- tightening claims where evidence is thin
- making future directions operational rather than wish-list-like

### 8. Peer-review simulation
Produce:
- simulated reviewer comments
- response table
- pre-submission checklist

Read [references/peer-review-reply-template.md](references/peer-review-reply-template.md).

### 9. Finalization
Produce:
- cleaned final markdown
- numbered citation style
- ordered reference list
- Word finalization instructions

Read [references/word-finalization-template.md](references/word-finalization-template.md).

## How to adapt this skill

If the user already has a project in progress:
- identify the current stage
- avoid restarting completed phases
- only add missing artifacts
- preserve the user’s existing naming and folder conventions when possible

If the user wants a reusable project structure:
- provide a clean stage-based repository layout
- separate generic templates from project-specific examples
- avoid mixing case-study outputs into the reusable core

## Suggested repository shape

```text
review-project/
├─ 00_topic/
├─ 01_search/
├─ 02_screening/
├─ 03_fulltext/
├─ 04_evidence/
├─ 05_outline/
├─ 06_drafts/
├─ 07_peer_review/
├─ 08_report/
└─ tools/
```

## Examples and references

For a concrete case-study abstraction, see:
- [examples/biomedical-review-case.md](examples/biomedical-review-case.md)

For templates and checklists, use the `references/` directory as needed rather than overloading this main skill file.
