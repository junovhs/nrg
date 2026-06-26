# Findings — Visual Structure and LLM Comprehension

Source report (verbatim): [`working/visual-structure-research.md`](working/visual-structure-research.md), mined from the `semmap` repo. This is an **open research agenda** — six framed questions, not yet settled findings.

## Open question: tokenization fidelity of spatial structure
- **What:** How do BPE / SentencePiece / tiktoken decompose ASCII box-drawing characters (├ │ └) and indentation? Is the parent→child spatial relationship a recoverable post-tokenization signal, or does it degrade into arbitrary token sequences the model must re-infer via positional encoding?
- **Evidence / source:** [`working/visual-structure-research.md`](working/visual-structure-research.md)
- **Confidence:** low (open question)
- **Date:** 2026-06-26

## Open question: attention topology on structured input
- **What:** Do attention heads spontaneously "trace" parent-child relationships along indentation levels, or does attention stay local/sequential regardless of visual structure?
- **Evidence / source:** [`working/visual-structure-research.md`](working/visual-structure-research.md)
- **Confidence:** low (open question)
- **Date:** 2026-06-26

## Remaining sub-threads
- **What:** The source report frames six total research questions on visual structure vs. LLM comprehension. See the verbatim report for the full set.
- **Evidence / source:** [`working/visual-structure-research.md`](working/visual-structure-research.md)
- **Confidence:** low (open question)
- **Date:** 2026-06-26
