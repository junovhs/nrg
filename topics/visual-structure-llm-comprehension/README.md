# Visual Structure and LLM Comprehension

- **Slug:** `visual-structure-llm-comprehension`
- **Status:** active
- **Owner(s):** Spencer
- **Started:** 2026-06-26
- **Last updated:** 2026-06-26

## Question
Does the visual/spatial structure of input (indentation, box-drawing characters,
hierarchy) actually help an LLM comprehend content, and through what mechanism?

## Why it matters
Underpins `semmap`'s bet that visually structured output improves model
comprehension over flat prose. If the signal degrades at tokenization or isn't used
by attention, the format choice needs rethinking.

## Key questions / sub-threads
- [ ] Tokenization fidelity of box-drawing chars and indentation (BPE/SentencePiece/tiktoken)
- [ ] Attention topology on hierarchically-indented vs. flat input
- [ ] (further sub-questions in the source report)

## Current state
A set of six open research questions mined from the `semmap` repo (archived). This
is a question framing / research agenda rather than settled findings — sub-threads
remain open.

## Links
- Findings: [`findings.md`](findings.md)
- Working material: [`working/`](working/) — verbatim source report
- Source repo: `../semmap/docs/archived/visual-structure-research.md`
