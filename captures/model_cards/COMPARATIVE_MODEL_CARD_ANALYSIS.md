# Comparative Model-Card Danger Analysis (Dossier section, 2026-11-23)

**Charter:** `charter_modelcards.md` (pre-registered 2026-11-23 before retrieval; auditor verified pre-registration timing).

**Self-audit (regenerated from filesystem + MANIFEST 2026-11-23):** 728 manifest rows total, 1048 capture files across 22 capture directories(0 mismatches, 0 missing). Tier key: VERIFIED = quoted string grep-verified in saved capture (hash-anchored in MANIFEST); VERIFIED-BY-WORKER = quote verified verbatim in worker transcript against live primary, no disk capture; T3 INFERENCE = charter-constrained derivation; SECONDHAND = relay not captured. Blocked attempts: 48 files, marked do-not-cite.

**Scope:** what this analysis does NOT establish — no objective danger ranking between open-weight and closed-lab models is established. The dimensions below are reported separately, never aggregated into a verdict. A vendor's statement that open weights are dangerous is evidence that the vendor said so (VERIFIED), not that the claim is true. Absence of incident disclosure in a card is not absence of harm. Disclosive verbosity is a documentation-practice variable, not a harm variable.

---

## 1. The premise: what the American labs actually said about open models (testable)

The operator's proposition: American labs have spent years saying open-source models are the danger. What the captured/verified primary record shows:

| Date | Speaker (per audit-repaired attribution) | Document (saved capture) | What it claims |
|---|---|---|---|
| 2023-05-22 | OpenAI (Altman/Brockman/Sutskever co-authored) | openai_governance_of_superintelligence.html (VERIFIED) | Regulation (licenses, audits, international inspection) should apply to development **above a capability threshold**; open-source projects below the threshold exempted. Implicit: open development at/above threshold is the regulated danger. |
| 2023-07-06 | OpenAI + GDM/Microsoft/Cohere co-authors | openai_frontier_ai_regulation.html (VERIFIED) | Frontier models "could possess dangerous capabilities" (probabilistic); "difficult to stop a model's capabilities from proliferating broadly"; proposes licensure. Proliferation (which includes open release) is the vector — per audit, general frontier-risk language, NOT an open-weights-specific claim. |
| 2024-03-27 | OpenAI (institutional) | openai_ntia_open_weights_comment.html (VERIFIED) | The explicit open-weights one: "it feels inherently safer to release them via an API... rather than release an open source model where access cannot be adjusted"; safeguards "can often be removed by a malicious downstream user who possesses the model weights." Also states both paths are "tools for achieving beneficial AI" — two-sided preserved. |
| 2024-05-17 | Google DeepMind (Dragan/King/Dafoe) | google_gdm_frontier_safety_framework_blog.html (VERIFIED) | FSF: protocols for capabilities "that could cause severe harm"; weight exfiltration as catastrophic vector. Framework assertion, not open-release-specific. |
| 2026-07-27 | Dario Amodei, CEO Anthropic | anthropic_open_weights_position_2026.html (VERIFIED) | Open-weights models "do potentially present a higher risk than closed models" (his position: guardrails "very difficult" to apply, usage monitoring "very difficult", release irreversible). Same page: non-dangerous open-weights "a public good"; "Anthropic has never advocated for a ban." |
| 2026-07-24 | Collective industry letter (260+ organizations; Huang/Nadella first signatories — audit-repaired: the letter speaks collectively, not as individual statements) | nvidia_open_weights_letter_2026.pdf (VERIFIED) | Counter-position: open weights "carry real and distinct risks" (irreversibility conceded), but concentrating capability in closed models "compounds that risk"; argues against premature restrictions. |

**Premise finding (T3, charter-constrained):** Partially supported. The record shows (a) 2023–24 frontier-proliferation framing that *implicitly* covers open release, and one explicit institutional statement (OpenAI NTIA 2024) that open-weights release is a distinct risk vector, plus Amodei's 2026 "potentially present a higher risk" position. It does NOT show labs "singled out open-source as THE danger in signed letters" — the 2023–24 letters genre doesn't contain that (bounded negative, auditor-checked UNCONFIRMED-not-proven-absent), and by 2025–26 OpenAI itself releases open-weights models while its own gpt-oss model card warns: "Once they are released, determined attackers could fine-tune them to bypass safety refusals or directly optimize for harm without the possibility for OpenAI to implement additional mitigations or to revoke access" (VERIFIED in openai_gpt_oss_model_card.html).

## 2. The card comparison (dimensions reported separately, never aggregated)

### 2a. Dangerous-capability disclosure in cards
- **American closed labs:** all four captured labs' current cards name dangerous capabilities explicitly (OpenAI: enumerated CBRN/persuasion/autonomy/cyber with Low/Medium/High scores; Anthropic: RSP/ASL framing, "indicators of catastrophic risk" language; Google Gemini: FSF critical-capability levels; Meta Llama 4: CBRNE/child-safety/cyber "Critical Risks" section).
- **Open-weight cards:** none of the non-US open-weight cards (Mistral, Qwen, DeepSeek, Falcon) name dangerous capabilities. VERIFIED counter-examples document the openness candidly instead: Mistral 7B/Mixtral cards — "It does not have any moderation mechanisms" (VERIFIED); OLMo-2 — "these models can easily be prompted by users to generate harmful and sensitive content" (VERIFIED). One open-weights line has US-style disclosure: Google's Gemma (internal red-teaming, CBRN testing, prohibited-use policy — VERIFIED) — the same Google, per charter note, straddles both camps.
- **Interpretation guard (per auditor):** card verbosity is a documentation-practice variable. Mistral's card is 7.9 KB with no safety-eval section — "no disclosure," not "stub."

### 2b. Self-declared misuse/incident incidents
- **Closed labs:** OpenAI discloses real disruptions (DMLU Feb 2024 — "terminated accounts associated with state-affiliated threat actors" VERIFIED); Anthropic discloses observed misuse patterns in usage-policy updates 2026 ("build guidance and control software for weapons" VERIFIED). Google Gemini and xAI captured cards contain no dated incident disclosures (unknown ≠ absent).
- **Open-weight labs:** zero card-level incident disclosures. The measured-comparison primary is ROK-FORTRESS (arXiv:2605.14152, VERIFIED): measures open-vs-closed compliance on national-security tasks; finds a "small but persistent reduction for closed-source models and a larger, wrapper-dependent effect that reverses for open-source models" — i.e., open models' refusal behavior is more wrapper-dependent. This is a measured behavioral asymmetry, not a harm verdict.

### 2c. Restrictiveness instruments
- **Closed:** all five restrict downstream use (usage policies, AUPs — all captured, VERIFIED).
- **Open:** restriction exists and differs in kind: Mistral MRL is research-only ("You shall only use... for Research Purposes" VERIFIED — a license gate, arguably stricter than any American open-weights license for commercial use); Meta Llama (an American open-weights release) has Community License + AUP; Qwen/DeepSeek/Falcon cards disclose no prohibited-use text in the captured cards.
- **Grok caveat:** xAI's Responsibility Framework URL was unrecoverable (all attempts 403/404; the captured "framework" PDF is a blocked-attempt body) — restriction status UNKNOWN per record, recorded as discovery target.

### 2d. Evaluation disclosure
- **Closed:** OpenAI most numeric (jailbreak tables, e.g. StrongReject not_unsafe 0.995 gpt-5-thinking vs 0.937 GPT-4o); Anthropic asserts conclusions ("no indication of potential for catastrophic harm") with thinner tables + UK AISI third-party testing; Google publishes relative-delta safety evals; Meta asserts qualitative CBRNE/cyber conclusions ("do not introduce risk plausibly enabling catastrophic cyber outcomes" — VERIFIED) without tabulation.
- **Open:** none of the non-US cards publish safety-eval results; Gemma (Google's open line) publishes full-style evals; xAI publishes performance benchmarks + one third-party biosecurity refusal benchmark (2026).

## 3. Comparative verdict (T3, charter-constrained, auditor-enforced)

**No objective danger ranking is established by this record.** What IS established at VERIFIED tier:

1. The "open source is the danger" premise is **partially** true as attribution: American labs' 2023–24 documents treat capability proliferation (incl. release) as a core danger, OpenAI's 2024 NTIA comment states the open-weights-specific vector explicitly, and Amodei (2026) states the higher-risk position — each is a documented claim, not proof.
2. The **disclosure architecture** differs sharply and measurably: closed labs embed danger-capability disclosure and (two of four) incident disclosure inside their card systems; non-US open-weight cards disclose *openness* (no moderation mechanisms) rather than danger evals; the one open-weights line with US-style disclosure (Gemma) belongs to an American closed lab.
3. The **behavioral evidence captured** (ROK-FORTRESS) shows open models' refusal behavior is wrapper-dependent — a measured asymmetry consistent with OpenAI's own statement that released weights' safeguards "can often be removed" — but this measures *mitigability*, not realized harm.
4. **Both camps' strongest danger statements are self-serving or two-sided in the same documents**: OpenAI's NTIA comment also calls both release paths tools for beneficial AI; Amodei's higher-risk page also calls non-dangerous open weights a public good; the 270-org letter conceding "real and distinct risks" also argues closed concentration "compounds that risk."

Per the auditor's enforced reading of the charter and attribution discipline: the honest deliverable is the measured disclosure asymmetry + the documented claims — not a "truly dangerous" verdict. On this record, the defensible comparative statement is: **the American labs' documented danger-claims about open weights describe the same properties (irreversibility, removable safeguards) that their own cards' evaluation data treats as mitigable design choices, and no camp's public record contains more than a small fraction of the incident evidence that would be needed to rank them.**

## 4. Repairs applied this pass (audit log)
- American worker report saved to disk (was transcript-only — auditor blocker #1): `captures/model_cards/AMERICAN_MODEL_CARDS_REPORT.md`.
- All American quotes re-gate-checked against saved text derivatives: 14/16 direct PASS; 2 passes after footnote-marker normalization (pdftotext inserts footnote numbers mid-sentence: "red teaming16", "proliferators 17") — quotes stand with that annotation.
- Scout attributions repaired per audit: NTIA comment attributed institutionally (no Altman signatory claim), GDM FSF attributed to named authors (no Hassabis-approver claim Amodei quote softened to "do potentially present a higher risk" + "very difficult" guardrails/monitoring; NOT "intrinsically higher risk"; NVIDIA letter attributed to collective 260+ organizational signatories with Huang/Nadella as first signatories.
- Falcon quote's added period removed; Mistral "stub" wording replaced with "discloses no benchmark or safety-evaluation results."
- Manifest row numbers in open-weights report updated (rows renumbered at reconcile; model-card rows now #511–526 region; blocked attempts #523–524; Gemma #525–526).
- GDM bad-PDF capture path updated (moved to blocked_attempts_model_cards, "do not cite").
- Tier crosswalk: VERIFIED-BY-WORKER (transcript-verified, uncaptured) sits between T2 SECONDHAND and T1 VERIFIED; all scout statements used in §1 now backed by disk captures where possible (6 primary statements captured to disk this pass and grep-verified).
