# BOOK 4 SPEC: "The Harness" (locked 2026-08-29)

Advanced AI book, sequel to Book 2 (The Thinking Machine).
Standalone (no roadmap references). Devanagari Marathi + English
tech nouns, Books 1-2 style. Zero code (fully conceptual).

## Locked via MCQs
- 3 parts, concept-grouped (like Book 2), separate PDFs then combined.
- Same chapter format as Books 1-2, SPINE/DEPTH kept.
- Zero code/commands; "स्वतः बघा" stays observational (phone/laptop).
- Standalone book; one part at a time, his OK gates the next.
- All 11 quality upgrades approved ("improve 15x").

## The 11 upgrades (all approved)
1. Book's law (सूत्र): "अंदाज फुकट झालाय, विश्वास महाग.
   Harness = अंदाजाचं विश्वासात रूपांतर करणारं यंत्र."
   Every chapter's closing block touches it.
2. Running example: "नानांची पेढी" — small-town CA office +
   its मुनीम-agent, grows chapter-by-chapter across all 3 parts.
   Part 1: why the raw model fails it. Part 2: harness built
   organ by organ. Part 3: production + earning.
3. Growing harness map: one ASCII diagram, each Part-2 chapter
   adds an organ (politics-book master-map style).
4. Verified war stories woven where they fit (Air Canada,
   Chevy $1, DB-deleting agent, METR 19% study, etc.).
5. "महाग चूक" section = misconception + what it cost (Rs/repute).
6. Fresh verified Aug-2026 numbers woven in.
7. Contested boxes: open debates shown two-sided + decision test
   (RAG vs long context, open vs closed, benchmark trust).
8. 3-4 post-mortem chapters: start from a dead agent, dissect.
9. Chained विचार करा: answer of one seeds the next chapter.
10. 5 one-page checklists at book end: agent-design, evals,
    security, cost, go-live (printable हात-नकाशे).
11. Fresh research-pass with agents before each part; every
    number/story verified, stricter than Books 1-3.

## Chapter block order
body (analogy per section, war story where fits) →
## महाग चूक → ## नकाशावर (map organ + 1-line सूत्र touch) →
## स्वतः बघा (5 मिनिटं) → ## विचार करा (chained, answer in quote)

## Outline (~52 ch)
PART 1 यंत्र घडवण्याची विद्या (~16): pretraining economics,
data-गाळणी, SFT, reward model, DPO/GRPO, RLVR, reward hacking,
RL environments | reasoning models, MoE, distillation, synthetic
data, model spec + constitutional AI, open vs closed frontier,
post-training shift.
PART 2 HARNESS (~17): attention budget, 4 शत्रू, 4 हत्यारं,
memory, agentic search | harness definition, tool design,
subagents, MCP, brakes/परवानगी, 12 नियम, spec-driven dev |
golden set, error analysis, LLM-as-judge, observability, evals-CI.
PART 3 PRODUCTION-सुरक्षा-धंदा (~19): GPU-साक्षरता, batching/
quantization/speculative, cache-aware काटकसर, build vs rent |
lethal trifecta, injection 2026, sandbox/least-privilege,
red-teaming | computer-use, A2A, agent-native software, vibe
coding उदय-अस्त | environments gold-rush, 2026 खंदक, एकट्याचा
कारखाना, अंतिम परीक्षा | + पूर्ण नकाशा + master glossary +
5 checklists.

## Pipeline (same as Books 1-3)
Files book/book4/partN/, BOOK.md assembly (sorted glob),
pdf generate to Temp then mv (path lock), --cover no --toc,
title "The Harness, Part N: <Marathi>", shingle+render verify,
stray-char scan, commit per part.
