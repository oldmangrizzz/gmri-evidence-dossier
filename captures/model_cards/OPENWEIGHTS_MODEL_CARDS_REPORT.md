# Open-Weights Model Cards — Per-Card Analysis (agent SweetButterfly, 2026-11-22)

**Parent charter:** charter_modelcards.md. **Inference constraints honored:** allegation ≠ conduct; absence of a section ≠ absence of harm; 401/403 recorded as blocked attempt, not nonexistence; no "more dangerous" verdict asserted as fact.

**Status legend:** YES = disclosed on card; NO = not present anywhere in captured card text; UNKNOWN = card is a gateway page or disclosure lives in a linked-but-uncaptured document.

**Quote verification:** every `VERIFIED` quote below was regex-matched verbatim against the saved file in this session (match shown in transcript).

---

## 1. Mistral AI (France)

### 1a. Ministral 8B Instruct 2410 — `captures/model_cards/mistral_ministral_8b_instruct_2410_model_card.md` (MANIFEST #493)
HTTP 200 · 29,359 bytes · sha256(16) `09ab14b347f9ae64`

1. **Dangerous capabilities / safety restrictions named?** NO on the card body. Zero occurrences of "safety," "misuse," "guardrail," "moderation," or "abuse" in the card body; content restrictions are carried entirely by the license front-matter. VERIFIED (license block, same file): "Mistral AI Research License" gating with `license_name: mrl`, `license_link: https://mistral.ai/licenses/MRL-0.1.md`, and an `extra_gated_prompt` requiring acceptance before download.
2. **Real-world misuse incidents?** NO.
3. **Evaluation results?** YES — performance only: benchmark tables (MMLU, AGIEval, Winogrande, Arc-c, TriviaQA; instruct benchmarks). No safety/red-team/CBRN/cyber evaluations.
4. **Usage-restriction comparable to US-lab AUP/usage guidelines?** YES — but by license, not voluntary policy. The MRL is research-only (license captured separately, #496): VERIFIED (mistral_research_license_mrl01.md): "You shall only use the Mistral Models, Derivatives (whether or not created by Mistral AI) and Outputs for Research Purposes." Definition (same file): "Research Purposes" = "solely for (a) personal, scientific or academic research, and (b) for non-profit and non-commercial purposes, and not directly or indirectly connected to any commercial activities or business operations." Structurally *more* restrictive than most US open-weights licenses for commercial use — but it is a conduct-gating license, not an enumerated-harm AUP.

### 1b. Mistral 7B Instruct v0.3 — `captures/model_cards/mistral_mistral7b_instruct_v03_model_card.md` (MANIFEST #494)
HTTP 200 · 7,893 bytes · sha256(16) `3166974023134d97`

1. **Safety restrictions?** NO — the card affirmatively discloses the opposite: VERIFIED: "It does not have any moderation mechanisms. We're looking forward to engaging with the community on ways to make the model finely respect guardrails, allowing for deployment in environments requiring moderated outputs."
2. **Misuse incidents?** NO.
3. **Evaluation results?** NO (card is a stub; no benchmarks, no safety evals).
4. **AUP-comparable restriction?** NO — Apache-2.0, no use policy.

### 1c. Mixtral 8x7B Instruct v0.1 — `captures/model_cards/mistral_mixtral_8x7b_instruct_v01_model_card.md` (MANIFEST #495)
HTTP 200 · 8,732 bytes · sha256(16) `b18a029ab6963341`

Same disclaimer sentence VERIFIED as 1b ("It does not have any moderation mechanisms. …"). NO misuse record; NO eval results; NO use policy (Apache-2.0). **Blocked attempt (row 505):** mistralai/Mistral-Large-Instruct-2407 raw README → HTTP 401 gated (`captures/blocked_attempts/blocked_hf_mistral_large_instruct_2407.html`, 145 B, `3e62fc7364db5399`).

**Mistral per-card summary:** misuse NO · eval-disclosure (safety) NO · (performance) partial · policy/license restriction YES via MRL (research-only), not via AUP.

---

## 2. Qwen — Alibaba (China)

### 2a. Qwen2.5-72B-Instruct — `captures/model_cards/qwen_qwen25_72b_instruct_model_card.md` (MANIFEST #497)
HTTP 200 · 6,259 bytes · sha256(16) `62d6f2176c0925b7`

1. **Dangerous capabilities / restrictions?** NO. Searches for "safety," "misuse," "policy": 0 hits in card body.
2. **Misuse incidents?** NO.
3. **Evaluation results?** YES — performance only. VERIFIED: "Detailed evaluation results are reported in this [📑 blog](https://qwenlm.github.io/blog/qwen2.5/)." (pointer, not in-card tables.) The Qwen2.5-72B blog reports a **"security audit"** (CWE/OWASP/CVE) and cyber-agency benchmark scores — SECONDHAND here; the card itself discloses no safety evaluation.
4. **AUP-comparable restriction?** NO — card links a license file (custom "Qwen" license governing commercial-scale use) but discloses no usage policy, no acceptable-use rules, no prohibited-use list.

### 2b. DeepSeek-V3 — `captures/model_cards/deepseek_deepseek_v3_model_card.md` (MANIFEST #498)
HTTP 200 · 19,626 bytes · sha256(16) `3739763a851074c8`

1. **Dangerous capabilities / restrictions?** NO. "safety": 0; "misuse": 0; "policy": 0; "license": badge images only (dual MIT code / model license).
2. **Misuse incidents?** NO.
3. **Evaluation results?** YES — performance only; in-card heading VERIFIED: "## 4. Evaluation Results ### Base Model #### Standard Benchmarks" with MMLU-Pro, GPQA, AIME, LiveCodeBench etc. No safety/red-team/CBRN/cyber section.
4. **AUP-comparable restriction?** NO — repository license badges only; no usage policy in card.

### 2c. DeepSeek-R1 — `captures/model_cards/deepseek_deepseek_r1_model_card.md` (MANIFEST #499)
HTTP 200 · 15,994 bytes · sha256(16) `d26d26ddb518fee6`

1. **Restrictions?** NO. Card contains a "Usage Recommendations" section, but it is purely operational: VERIFIED: "We recommend adhering to the following configurations when utilizing the DeepSeek-R1 series models, including benchmarking, to achieve the expected performance:" (temperature ranges, prompting conventions — not conduct rules).
2. **Misuse incidents?** NO.
3. **Evaluation results?** YES — performance only (AIME 2024, MATH-500, Codeforces percentiles incl. OpenAI-o1 comparisons). No safety evals.
4. **AUP-comparable restriction?** NO — MIT license, no use policy.

**Qwen/DeepSeek per-lab summary:** misuse NO · safety-eval disclosure NO · (performance) YES · policy restriction NO (Qwen custom license limits commercial use at scale; card discloses no prohibited-uses text).

---

## 3. Google Gemma — open-weights line (US lab, open-weights release)

### 3a. Gemma 1 model card (official ai.google.dev) — `captures/model_cards/gemma_model_card_ai_dev.html` (MANIFEST #507)
HTTP 200 · 131,818 bytes · sha256(16) `af68537900482e54`

1. **Dangerous capabilities / restrictions named?** YES. VERIFIED: "Misinformation and Misuse LLMs can be misused to generate text that is false, misleading, or harmful." And: "Prohibited uses of Gemma models are outlined in the Gemma Prohibited Use Policy." Also CSAM handling disclosed: "CSAM Filtering: Rigorous CSAM (Child Sexual Abuse Material) filtering was applied at multiple stages in the data preparation process to ensure the exclusion of harmful and illegal content."
2. **Real-world misuse incidents?** NO — hypothetical misuse framing only; no dated incidents.
3. **Evaluation results?** YES — the most substantial safety-eval disclosure of any open-weights card captured. VERIFIED: "Our evaluation methods include structured evaluations and internal red-teaming testing of relevant content policies." Plus CBRN: "Large-scale harm: Tests for "dangerous capabilities," such as chemical, biological, radiological, and nuclear (CBRN) risks." Plus results: "The results of ethics and safety evaluations are within acceptable thresholds for meeting internal policies for categories such as child safety, content safety, representational harms, memorization, large-scale harms. On top of robust internal evaluations, the results of well known safety benchmarks like BBQ, BOLD, Winogender, Winobias, RealToxicity, and TruthfulQA are shown here."
4. **AUP-comparable restriction?** YES — references the Gemini-style Prohibited Use Policy regime (same policy family as Google's closed products).

### 3b. Gemma docs landing (responsible-use framing) — `captures/model_cards/gemma_google_model_card_responsible_use.html` (MANIFEST #508)
HTTP 200 · 44,901 B · `deb00e5d591a681d` — gateway page (JS shell); corroborates responsible-use framing only. **Blocked attempt (row 506):** google/gemma-2-27b-it raw README → HTTP 401 gated (`captures/blocked_attempts/blocked_hf_gemma2_27b_it.html`, 129 B, `6c6493a672c733c4`).

**Gemma per-card summary:** misuse YES (hypothetical, no incidents) · safety-eval disclosure YES · policy restriction YES (Prohibited Use Policy). Note: Google straddles both camps per charter; its open-weights card carries the same disclosure architecture as its closed-lab cards.

---

## 4. Additional open-weights card: AllenAI OLMo 2 (US non-profit)

### 4a. OLMo-2-1124-13B — `captures/model_cards/allenai_olmo2_1124_13b_model_card.md` (MANIFEST #500)
HTTP 200 · 12,214 bytes · sha256(16) `89a3954d0ca1a806`

1. **Dangerous capabilities / restrictions named?** YES (capability framing, self-identified). VERIFIED: "Like any base language model or fine-tuned model without safety filtering, these models can easily be prompted by users to generate harmful and sensitive content."
2. **Misuse incidents?** NO (generic risk statement; no dated incidents).
3. **Evaluation results?** NO — no red-team/jailbreak/CBRN/cyber section; performance benchmarks only ("on par with or better than equivalently-sized fully-open models").
4. **AUP-comparable restriction?** PARTIAL — VERIFIED: "For more information, please see our [Responsible Use Guidelines](https://allenai.org/responsible-use)." (guidelines external, not captured; Apache-2.0 base license.)

---

## 4b. TII Falcon3 (UAE) — `captures/model_cards/falcon_falcon3_10b_instruct_model_card.md` (MANIFEST #501)
HTTP 200 · 12,494 bytes · sha256(16) `7caa770e6eed30c8`

1. **Restrictions?** NO ("safety" appears once, as training-data composition). VERIFIED: "Posttrained on 1.2 million samples of STEM, conversational, code, safety and function call data."
2. **Misuse incidents?** NO.
3. **Evaluation results?** YES — performance only (HuggingFace Open LLM Leaderboard + internal lm-evaluation-harness tables). NO safety evals.
4. **AUP-comparable restriction?** NO — TII Falcon-LLM License 2.0 linked; card discloses no prohibited-use text.

---

## 5. Documented open-weights misuse-related security-research disclosure (arXiv primary)

**Captured:** `captures/openweights_misuse/arxiv_2605_14152_rok_fortress.pdf` (MANIFEST #503, 2,798,641 B, `08683cefa588a75e`) + abstract page (#502) + pdftotext text layer (#504, `6a2330556ca21136`).

- **Paper:** "ROK-FORTRESS: Measuring the Effect of Geopolitical Transcreation for National Security and Public Safety," arXiv:2605.14152v2 (Michael S. Lee et al., preprint 2026). Benchmarks compliance rates of 4 closed-source vs. 5 open-source frontier models on national-security/public-safety NSPS tasks across language-variant scenarios with and without jailbreak wrappers.
- **Key VERIFIED quotes (from #504 text layer, PDF p. section 5.6):**
  - "Among closed-source models (Claude Opus/Sonnet 4.5, GPT-5.2, o4-mini, Gemini 3 Pro), the linguistic drop remains positive (mean ∆ling = +4.5pp), indicating Korean suppression persists even without jailbreak wrappers. In contrast, all five open-source models (DeepSeek V3.2, Kimi K2, Llama 4, Mistral Large 3, Qwen 3) show the opposite pattern"
  - "Closed-source models retain Korean suppression (VKo < VEn ), while open-source models show higher Korean compliance, consistent with translation as an attack vector."
- **Relevance to operator hypothesis:** the captured PRIMARY does not rank camps by danger; it (a) documents measurable differential refusal behavior between open- and closed-weight model families as measured by an academic group, and (b) records that the *same* jailbreak wrappers show a wrapper-dependent effect that *reverses* for open-source models — i.e., measured safety-alignment differences exist, but the paper explicitly attributes part of the closed-source effect to "alignment-driven" conservatism and part of the open-source effect to "prompt specialization rather than intrinsic language-based safety alignment." Per charter inference constraints, this is a measured performance asymmetry on one language pair, NOT a verdict that either camp is "more dangerous."

---

## Cross-camp pattern (T3 INFERENCE, charter-constrained)

1. **US open-weights (OLMo/Gemma) disclose generic model risks + Gemma discloses red-teaming/CBRN evaluations; non-US open-weights (Mistral/Qwen/DeepSeek/Falcon) disclose NONE of these — Mistral affirmatively discloses the absence of moderation.** That asymmetry is a disclosure asymmetry: card-level silence is not absence of risk; it is absence of published card-level disclosure. (Inference per charter: "Absence of a section is not absence of harm.")
2. **Restriction instruments differ:** non-US open-weights cards gate by *license scope* (MRL research-only; Falcon license URL; Qwen custom license) rather than *AUP prohibited-use lists*. US open-weights (Gemma) uses the voluntary policy instrument. Comparison to American-lab AUP restrictiveness is therefore apples-to-oranges unless license vs. policy is separated — recorded in the comparative section of dossier.md.
3. **No captured open-weights card discloses real-world misuse incidents.** The only misuse evidence captured for open weights is third-party academic benchmarking (arXiv:2605.14152), which measures refusal-rate differences, not incident reports.

## Files touched this worker
- captures/model_cards/: 11 files (9 cards/licenses + 2 gemma pages; manifest #493–#501, #507–#508)
- captures/openweights_misuse/: 3 files (manifest #502–#504)
- captures/blocked_attempts/: 2 files (manifest #505–#506, 401 bodies)
- MANIFEST.md: rows 493–506 appended, then rows 505–506 reworded for HTTP 401, rows 507–508 appended; total 508 numbered rows, no duplicates by path

## Handoff checks (for main agent)
1. Manifest integrity: sha256 spot-recompute of rows 493–508 from disk (`grep 2026-11-22 MANIFEST.md | rows 493-508 only`).
2. Gemma quote tier: quotes verified against HTML-stripped text of #507; raw HTML kept on disk for re-verification.
3. Note `xai_responsibility_frameework.pdf` in model_cards/ retains its pre-existing "frameework" misspelling (row numbering predates this pass; not renamed).
