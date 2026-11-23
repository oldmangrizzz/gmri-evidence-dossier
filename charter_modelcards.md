# CHARTER — Comparative Model-Card Danger Analysis (2026-11-23)

## Pre-registration (before any retrieval)

## Propositions (verbatim from operator)

> "The American Labs have spent years saying that the open source models are the danger. I don't think they are. I think it's the other way around."

> "Love meta into the American models, not the open source." *(interpreted as: "Lump Meta in with the American models, not the open source" — Meta is grouped with the closed American labs for this comparison despite releasing open weights; this is the operator's framing and it is preserved.)*

> "Pull the model cards for the open source models and the American models. Do comparative analysis."

> "Let's find out who's actually the more dangerous, truly dangerous."

## What I will examine
1. Model cards / system cards / use policies from the American closed labs: Meta (Llama), OpenAI (GPT), Anthropic (Claude), Google (Gemma/Gemini), xAI (Grok).
2. Model cards from open-weight non-American labs: Mistral (France), Qwen/DeepSeek (China), Gemma (Google open-weights, noted: Google straddles both camps).
3. Each card's documented misuse/danger evidence: self-reported danger disclosures, known misuse incidents, use-policy violations, jailbreak/safety incidents from both camps.
4. Comparative danger metric: model-card danger disclosures, incident rate where published, use-policy restrictiveness, and disclosure asymmetry.

## Inference constraints (FORBIDDEN inference)
- Allegation ≠ conduct. A vendor claiming open-source is dangerous is an allegation, not proof.
- Model-card self-disclosure ≠ comprehensive incident record. Absence of a section is not absence of harm.
- Use-policy restrictiveness ≠ real-world danger. A card can claim safety without disclosing incidents.
- "Open source" ≠ "open weights" for the purposes of this comparison — I compare model cards, not licenses, unless the license itself is the subject.
- Meta model cards will be read as American-lab releases per operator framing, AND their open-weights status will be noted independently.
- A failed web fetch is not evidence of nonexistence. 404/403 is recorded as blocked attempt, not absence.
- No claim that any camp is "more dangerous" is stated as fact unless a captured primary supports it at VERIFIED tier. The operator's hypothesis is tested, not assumed.

## Deliverables
1. `captures/model_cards/` — saved primary model cards (both camps)
2. `dossier.md` section — comparative danger analysis, tiered
3. Appendix to private intel report (operator-only summary)
4. Updated public repo with new captures + MANIFEST rows

## Tier key
- T1 VERIFIED: captured primary on disk, hash-anchored
- T2 SECONDHAND: relayed from search/fetch output without a saved primary
- T3 INFERENCE: explicitly labeled, derived from T1/T2 constraints above
- T4 UNVERIFIED claim: cannot reach T1 yet, named as discovery target


## Post-audit enforceability addendum (2026-11-23, auditor-repair #3)
The comparative dimensions (danger disclosures, incident disclosures, use restrictions, evaluation disclosure) are reported SEPARATELY in the deliverable, never aggregated into an overall ranking. A captured primary verifies that a claim was made, not that the claim is true ("VERIFIED" attests to the document and the quote, never the claim's truth). Without comparable measured outcome data, no objective danger ranking is established.
