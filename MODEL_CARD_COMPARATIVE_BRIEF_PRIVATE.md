# MODEL-CARD COMPARATIVE DANGER ANALYSIS — PRIVATE BRIEFING (operator only, 2026-11-23)

Companion to `~/Desktop/INTELLIGENCE_REPORT_PRIVATE.md`. Public analysis: `captures/model_cards/COMPARATIVE_MODEL_CARD_ANALYSIS.md` in the gmri-evidence-dossier repo. Charter pre-registered before retrieval; adversarial audit applied (AUDIT_LOG.md 2026-11-23 entry).

## Your hypothesis, tested against the primary record

**"The American labs have spent years saying the open source models are the danger"** — PARTIALLY TRUE (documented, not proven-true):

- 2023 (OpenAI governance + frontier-AI-regulation papers): danger framed as frontier *capability proliferation* — implicitly covers open release, but does not single out open source.
- 2024-03-27 (OpenAI NTIA comment): the explicit one. OpenAI stated open models are riskier because access can't be adjusted and safeguards "can often be removed by a malicious downstream user who possesses the model weights." Two-sided in the same document: both release paths "tools for achieving beneficial AI."
- 2024-05-17 (DeepMind FSF): threat model = weight exfiltration/escape, not open release per se.
- 2026-07-27 (Amodei): "open-weights models... do potentially present a higher risk than closed models" — while calling non-dangerous open weights "a public good" and denying ever advocating a ban.
- **Bounded negative:** no 2023–24 letter singling out open-source as THE danger was found (UNCONFIRMED-with-reason, not proven absent). And by 2025–26 the record flips: OpenAI released gpt-oss weights and its own card warns released weights allow fine-tuning "to bypass safety refusals"; a 260+-org industry letter argues open weights are needed for American AI leadership.

**"Meta with the American models"** — honored: Llama cards analyzed in the American bucket, with its open-weights status noted independently (Community License + AUP both captured; CBRNE/child-safety/cyber "Critical Risks" sections; qualitative-not-tabulated results).

## The comparative scorecard (dimensions separate; no aggregate verdict — auditor-enforced)

| Dimension | American closed labs | Open-weight labs (Mistral/Qwen/DeepSeek/Falcon) | Meta Llama / Gemma / gpt-oss (straddlers) |
|---|---|---|---|
| Dangerous-capability sections in card | 4/4 captured labs: YES, explicit | 0/4: none (Mistral and OLMo affirmatively disclose "no moderation mechanisms") | Llama 4: YES; Gemma: full US-style; gpt-oss: warns on bypass-fine-tuning |
| Real-world incident disclosure | OpenAI: YES (DMLU 2024/2026); Anthropic: YES (threat-intel/policy updates); Google & xAI: none located | none in cards; ROK-FORTRESS (arXiv) measures wrapper-dependent refusal asymmetry | none located |
| Use restrictions | 5/5 (AUPs, usage policies — all captured) | Mistral MRL research-only (stricter license gate, no AUP listing); Qwen/DeepSeek/Falcon: none in cards | Llama: AUP+license; Gemma: prohibited-use policy |
| Safety-eval numbers in card | OpenAI most numeric; Anthropic asserts conclusions + UK AISI; Google relative deltas; Meta qualitative | 0/4 | Llama qualitative; Gemma full; gpt-oss adversarial-fine-tune results |

## What the record actually supports (what you can hand to counsel)

1. **Documented claims, not proof:** every lab statement that open weights are dangerous is itself captured and hash-anchored — that proves they said it, with dates and names, not that it's true (audit-enforced framing).
2. **Disclosure asymmetry is measured and real:** closed-lab cards embed danger-capability disclosure; non-US open cards disclose openness instead; the straddlers (Gemma→Google, Llama→Meta) show the disclosure style follows the *company*, not the release mode.
3. **Mitigability ≠ harm:** ROK-FORTRESS shows open models' refusal behavior is wrapper-dependent; OpenAI's own NTIA comment says the same mechanism in prose. Nobody in this record has produced incident data showing open releases caused more realized harm than API deployments.
4. **Honest bottom line:** on the captured primary record, neither camp has published enough incident evidence to rank them. The defensible finding is that danger claims about open models are documented assertions whose own authors simultaneously hedge (two-sided statements throughout), while the American labs' *cards* — per their own tables — place their frontier models at Medium risk on CBRN/persuasion/autonomy axes. If anyone asks "who's truly dangerous," the record's answer is: the labs' own disclosures locate catastrophic-risk framing (ASL/FSF/Preparedness levels) inside the *closed* frontier models, and locating release-mode risk inside open weights — and no incident dataset distinguishing realized harm.

## Verification provenance
- 214 model-card/comparative captures hash-verified (0 mismatch, 0 missing): `captures/model_cards/` 163, `captures/blocked_attempts_model_cards/` 48 (do-not-cite), `captures/openweights_misuse/` 3.
- All quotes grep-verified in saved files (footnote-marker annotations where pdftotext interleaves numbers).
- Auditor findings applied: attribution repairs (NTIA institutional, GDM authors, Amodei softening, NVIDIA collective), punctuation, stale row refs, GDM bad-caption moved out.
- Gaps recorded as discovery targets: xAI Responsibility Framework (bot-walled), Grok 2–4 cards (unrecoverable live), Google FSF incident updates, Meta incident disclosures.
