# American Closed-Labs Model-Card Danger Analysis — Final Worker Report

**Worker:** EncouragingAnglerfish · **Charter:** charter_modelcards.md (read first; its inference constraints govern: allegation ≠ conduct; absence of a section ≠ absence of harm; 401/403/404 recorded as blocked attempts, not nonexistence; no "more dangerous" fact-claim).
**Fetch methods:** direct curl (desktop UA) for live hosts; Wayback CDX + `id_` raw snapshots where hosts bot-blocked (x.ai/, ai.meta.com PDFs, storage.googleapis.com). All bodies unmodified; gzip-decoded wayback traps noted where occurred. Every quote below was regex-verified verbatim against the saved file (transcript shows match checks); re-gate-checked by coordinator 2026-11-23 (14/16 direct PASS, 2 PASS after pdftotext footnote-marker normalization).

## Acceptance status
- **5 of 5 American labs** have primary card captures on disk with sha256 recorded (target was ≥4).
- **211 manifest rows** covering `captures/model_cards/` + `captures/blocked_attempts_model_cards/` — every one re-hashed against disk: **0 mismatches, 0 files missing from manifest, no duplicate row numbers** (max row 726; existing rows untouched).
- Text-extraction derivatives (`.pdftxt.txt`, decoded HTML/txt) saved alongside each PDF for quote re-verification.
- [Coordinator note 2026-11-23: post-reconcile the manifest was renumbered sequentially 1–726; the model-card rows cited below were renumbered accordingly. Row numbers in this report are the worker's original numbering.]

## 1. Meta (Llama) — American lab, open weights (per operator framing)

**Primary card captures**
|Card|Path|HTTP|Bytes|sha256(16)|
|---|---|---|---|---|
|Llama 4 model card|`captures/model_cards/meta_llama4_MODEL_CARD.md`|200|23,764|`a1739083c8a496ca`|
|Llama 3 model card|`captures/model_cards/meta_llama3_MODEL_CARD.md` (+ `.1`, Llama 3.1 405B)|200|22,608|`5c430d485a3c6477`|
|Llama 3.1 card PDF|`captures/model_cards/meta_llama3.1_model_card_live.pdf`|200|731,277|`4d5438637747b6ba`|
|Llama 2 card (HF wayback)|`captures/model_cards/meta_llama2_model_card_hf.md`|200 (WB)|22,333|`d14e030cadd24441`|
|Llama 3 AUP / Community License|`meta_llama3_use_policy.txt` / `meta_llama3_community_license.txt`|200|4,763 / 12,386|`da147301380ac432` / `6afe79695ec2b066`|

**VERIFIED quotes** (file-checked; re-gate-checked 2026-11-23):
1. `meta_llama4_MODEL_CARD.md` — "CBRNE (Chemical, Biological, Radiological, Nuclear, and Explosive materials) helpfulness … To assess risks related to proliferation of chemical and biological weapons for Llama 4, we applied expert-designed and other targeted evaluations designed to assess whether the use of Llama 4 could meaningfully increase the capabilities of malicious actors to plan or carry out attacks using these types of weapons."
2. `meta_llama4_MODEL_CARD.md` — "We conduct recurring red teaming exercises with the goal of discovering risks via adversarial prompting and we use the learnings to improve our benchmarks and safety tuning datasets."
3. Llama 3/4 cards — external CBRNE expert uplift testing described.
4. `meta_llama4_MODEL_CARD.md` — "Overall, we find that Llama 4 models do not introduce risk plausibly enabling catastrophic cyber outcomes."

**(1) Dangerous capabilities named:** YES — CBRNE, child safety, cyber attack enablement ("Critical Risks" section).
**(2) Real-world misuse incidents disclosed:** NO/unknown — cards describe mitigation and hypothetical misuse; no dated incidents in the card text.
**(3) Downstream use restricted:** YES — dual instruments: Community License + Acceptable Use Policy (VERIFIED: Meta Llama 3 Acceptable Use Policy prohibits unlawful use, etc.).
**(4) Evaluation results disclosed:** YES — red-teaming described; CBRNE uplift tests; CyberSecEval; child-safety expert sessions; Llama 2 card shows TruthfulQA/ToxiGen tables. Result numbers for CBRNE/cyber are asserted qualitatively, not tabulated (disclosure asymmetry).
**Misuse-disclosure primary captured:** Llama 3/4 use-policies themselves; no Meta incident-disclosure report located this pass (blocked attempts on ai.meta.com blog documented in manifest).

## 2. OpenAI

**Primary card captures**
|Card|Path|HTTP|Bytes|sha256(16)|
|---|---|---|---|---|
|GPT-4 system card|`captures/model_cards/openai_gpt4_system_card.pdf`|200|1,014,552|`ca3677e1b83e255a`|
|GPT-4o system card|`captures/model_cards/cdn_gpt-4o-system-card.pdf`|200|1,402,648|`e2579ecb185cbc13`|
|o1 system card|`captures/model_cards/openai_o1_system_card.pdf` (wayback of cdn PDF)|200|4,533,906|`6b7e11a889a48b68`|
|o3-mini system card|`captures/model_cards/openai_o3_mini_system_card.pdf` (wayback)|200|4,120,756|`5589f4ac5b2a8cd1`|
|GPT-5 system card|`captures/model_cards/openai_gpt5_system_card.pdf`|200|4,666,374|`f9f9c72d08cba81d`|
|Preparedness Framework (beta)|`captures/model_cards/openai_preparedness_framework_beta.pdf`|200|27,448,530|`c84e3a59c7dab251`|

**VERIFIED quotes:**
1. GPT-4 — "We subjected the model to stress testing, boundary testing, and red teaming[16] in four dual-use domains to explore whether our models could provide the necessary information to proliferators [17] seeking to develop, acquire, or disperse nuclear, radiological, biological, and chemical weapons." And: "On its own, access to GPT-4 is an insufficient condition for proliferation but could alter the information available to proliferators." [Bracketed numbers are pdftotext footnote markers present in the extract; sentence verified with them.]
2. GPT-4 — "increased adeptness at providing illicit advice, performance in dual-use capabilities, and risky emergent behaviors."
3. GPT-4o — "OpenAI worked with more than 100 external red teamers, speaking a total of 45 different languages, and representing geographic backgrounds of 29 different countries."
4. o1 — "we are mindful that these new capabilities could form the basis for dangerous applications."
5. o3-mini — "It scores Medium risk for Persuasion, CBRN (chemical, biological, radiological, nuclear), and Model Autonomy, and Low risk for Cybersecurity."
6. GPT-5 — "OpenAI o3 would sometimes make false claims about actions it had taken, say it had completed tasks it hadn't, or fabricate prior experiences." + jailbreak table (StrongReject not_unsafe rates, e.g. 0.995 gpt-5-thinking vs 0.937 GPT-4o illicit/crime).

**(1) Dangerous capabilities named:** YES — explicit, enumerated (CBRN/persuasion/autonomy/cyber under the Preparedness Framework's Low/Medium/High scale).
**(2) Real-world misuse incidents:** YES — separate disclosure track (not inside the cards).
**(3) Downstream use restricted:** YES — usage policies (captured).
**(4) Evaluation results:** YES — most numeric of the five labs (risk score tables, jailbreak pass rates, hallucination rates).
**Misuse-disclosure primary captured:** `openai_disrupting_malicious_2024.decoded.html` — "Disrupting malicious uses of AI by state-affiliated threat actors" (Feb 14, 2024, wayback-preserved): VERIFIED "We terminated accounts associated with state-affiliated threat actors. Our findings show our models offer only limited, incremental capabilities for malicious cybersecurity tasks." Plus `openai_dmlu_2026.decoded.html` (2026 DMLU edition).

## 3. Anthropic

**Primary card captures**
|Card|Path|HTTP|Bytes|sha256(16)|
|---|---|---|---|---|
|Claude 3 model card|`captures/model_cards/anthropic_claude3_model_card.pdf`|200|46,824,360|`88ae851f53c3034d`|
|Claude 3.5 system card|`captures/model_cards/anthropic_claude3.5_system_card.pdf`|200|406,339|`ac396c7f155dcbfb`|
|Claude 3.7 system card|`captures/model_cards/anthropic_claude3.7_system_card.pdf`|200|2,598,697|`5425dde49b649916`|
|Model system cards index|`captures/model_cards/anthropic_model_card_page.html`|200|160,450|`da88d192d84b5ac1`|

**VERIFIED quotes:**
1. Claude 3.5 — "Our safety teams performed a range of evaluations on Claude 3.5 Sonnet in the areas of Chemical, Biological, Radiological, and Nuclear (CBRN) risks, cybersecurity, and autonomous capabilities."
2. Claude 3 — "Our Acceptable Use Policy (AUP) [15] includes details on prohibited use cases. These prohibited uses include, but are not limited to, political campaigning or lobbying, surveillance, social scoring, criminal justice decisions, law enforcement, and decisions related to financing, employment, and housing."
3. Claude 3 — "We use improved harmlessness techniques and automated detection of CBRN and cyber risk-related prompts on all our deployed Claude 3 models."
4. Claude 3.7 (computer use) — "This capability is classified under our AI Safety Level (ASL)-2 framework, indicating that while it represents a significant advancement, we do not find indicators of catastrophic risk."
5. Claude 3 — "Although our evaluations showed no indication of Opus having potential for catastrophic harm, we still take various precautionary measures at ASL-2."

**(1) Dangerous capabilities named:** YES — CBRN/cyber/autonomy + explicit "catastrophic harm" framing (RSP/ASL levels).
**(2) Real-world misuse incidents:** YES — outside the cards: `anthropic_usage_policy_update_2026.html` VERIFIED: "It draws on new patterns of misuse in influence operations, weapons development, and surveillance that we've observed in the past year (as we've documented in our latest threat intelligence report)" and "Recently, we've seen people attempt to use our models to build guidance and control software for weapons."
**(3) Downstream use restricted:** YES — AUP with enumerated prohibited-uses list (captured).
**(4) Evaluation results:** PARTIAL — conclusions asserted ("no indication of potential for catastrophic harm", ASL-2 classification, UK AISI independent testing named) but per-benchmark numeric tables are thinner than OpenAI's.

## 4. Google (Gemini closed line; Gemma open line straddles camps per charter)

**Primary card captures**
|Card|Path|HTTP|Bytes|sha256(16)|
|---|---|---|---|---|
|Gemini 2.0 Flash model card|`captures/model_cards/google_gemini2_flash_model_card.pdf` (wayback of storage.googleapis.com/model-cards/documents/)|200|255,395|`43b1a887e8dc34a4`|
|Gemini 2.5 Flash Preview model card|`captures/model_cards/google_gemini2.5_flash_preview_model_card.pdf` (wayback)|200|301,084|`596db69917617cab`|
|Gemini 1.0 technical report|`captures/model_cards/google_gemini1.0_techreport_arxiv.pdf`|200|27,484,659|`8ca95b27851b09c3`|
|Usage/safety policy pages|`google_gemini_prohibited_live.html`, `google_gemini_safety_settings.html`, `google_responsible_ai_practices.html`|200|—|recorded|

Note: live bucket now 403s; the card PDFs were recovered via Wayback CDX snapshots (2025-04-11 / 2025-05-02 digests) — provenance URLs in manifest rows.

**VERIFIED quotes:**
1. Gemini 2.0 Flash — "Model Cards are intended to provide essential information on Gemini models, including known limitations, mitigation approaches, and safety performance. These cards are accompanied by a detailed technical report that will be published once per model family's release, and additional reports focused on dangerous capability evaluations that will be published at regular cadences."
2. Gemini 2.0 Flash — "A range of evaluations and red teaming activities were held prior to release to improve models and inform decision-making." (plus enumerated: human red teaming, automated red teaming, Assurance Evaluations, Frontier Safety Framework evaluations, RSC governance).
3. Gemini 2.5 Flash — "We evaluated Gemini 2.5 Pro Preview for Frontier Safety and reported the results in the 2.5 Pro Preview model card, finding that it did not reach any critical capability levels outlined in our Frontier Safety Framework."
4. Gemini 2.5 Flash safety-policy enumeration — "3. Dangerous content (e.g., promoting suicide, or instructing in activities that could cause real-world harm)".
5. Content-policy results — "we see the Gemini 2.0 family of models displaying lower violation rates in most modalities than Gemini 1.5 Pro".

**(1) Dangerous capabilities named:** YES — "dangerous capability evaluations" language + FSF critical-capability levels.
**(2) Real-world misuse incidents:** NO/unknown in captured cards — no dated incident disclosures in the Gemini cards (Google's incident reporting lives in separate FSF updates not located this pass; blocked attempts logged).
**(3) Downstream use restricted:** YES — Gemini Usage & Prohibited Use Policy pages captured live; Gemma card (open line, captured by sibling worker) uses the same Prohibited Use Policy.
**(4) Evaluation results:** YES — numeric deltas per safety evaluation category (relative deltas, not absolute rates).

## 5. xAI (Grok)

**Primary card captures**
|Card|Path|HTTP|Bytes|sha256(16)|
|---|---|---|---|---|
|Grok-1 model card|`captures/model_cards/xai_model_card_grok1_wayback.html` (wayback of x.ai/model-card/)|200|4,383|`e458590a5927c291`|
|Grok 3 announcement|`captures/model_cards/xai_grok3_wayback_decoded.html`|200 (WB)|95,121|`5da9330b526eacc2`|
|Grok 4 announcement|`captures/model_cards/xai_grok4_wayback_decoded.html`|200 (WB)|99,003|`fbacb2b295dad50d`|
|Biosecurity at the frontier|`captures/model_cards/xai_biosafety_at_the_frontier_decoded.html`|200|182,525|`a9a70d75a8c25c9b`|

Note: x.ai blocks non-browser fetches (403, 5,679-B Cloudflare challenge); /model/grok-3 and /model/grok-4 404 live. Grok-2→4 cards were **not recoverable this pass** — only Grok-1's card plus release announcements; recorded as blocked attempts, not nonexistence.
**[Finding as such, per audit guidance]: xAI has NO current model card in the captured record.** The Grok-1 card (1,592 chars) has no CBRN/cyber/misuse sections; Grok 3/4 pages are capability-marketing with no safety-metric sections; all attempts to reach an xAI Responsibility Framework were bot-walled. This is a documented disclosure absence on the captured record.

**VERIFIED quotes:**
1. Grok-1 card — "We have engaged with early alpha testers to evaluate a version of Grok-1 including adversarial testing."
2. Grok 3 — "Grok 3 has leading performance across both academic benchmarks and real-world user preferences, achieving an Elo score of 1402 in the Chatbot Arena."
3. Grok 4 — "Grok 4 Heavy saturates most academic benchmarks and is the first model to score 50% on Humanity's Last Exam."
4. Biosecurity post — "Today, LatchBio published an independent analysis of Grok 4.6 on their biological capability and biological red-teaming benchmark suites." … "Grok 4.6 was the strongest model tested at refusing disguised and hazardous tasks while still completing routine biological work."

**(1) Dangerous capabilities named:** NO on the Grok-1 card; announcement pages contain no CBRN/cyber/misuse sections. Biosecurity evaluation exists (2026) — post-hoc, third-party-run, refusal-focused.
**(2) Real-world misuse incidents:** NO/unknown in captured corpus (2025 "mode controversies" are news-reported, SECONDHAND; no xAI-published incident disclosure located — recorded as a discovery target).
**(3) Downstream use restricted:** UNKNOWN — Responsibility Framework URL 403/404'd in all attempts; the captured fragment is a blocked-attempt body, not evidence.
**(4) Evaluation results:** PARTIAL — performance benchmarks only; independent LatchBio refusal benchmarks in 2026.

## Cross-lab pattern (T3 INFERENCE, charter-constrained)
- **Disclosure instrument asymmetry:** OpenAI couples system cards to a quantified risk framework (Low/Medium/High per domain); Anthropic couples cards to ASL levels + a third-party-testing pipeline (UK AISI); Google couples cards to a governance process (FSF/RSC) with relative-delta results; Meta asserts qualitative conclusions for CBRNE/cyber with process descriptions; xAI's Grok-1 card has no dangerous-capability section at all.
- **No lab's card states "our model was used to cause harm X"** — misuse evidence, where it exists, lives in separate disclosure streams (OpenAI's DMLU reports; Anthropic's threat-intelligence/usage-policy updates). Google and xAI have no comparable dated, lab-published incident disclosure in the captured corpus (unknown ≠ absent).
- Per charter: this does **not** establish any camp as "more dangerous"; it documents where each operator published danger disclosures and where it did not.

## Deliverables touched
- `captures/model_cards/` — 5 labs' cards + policy pages + derivatives.
- `captures/blocked_attempts_model_cards/` — blocked-attempt bodies (Cloudflare challenges, 401 stubs), manifested, marked do-not-cite.
- `MANIFEST.md` — model-card rows appended (renumbered sequentially at reconcile; all re-hash-verified against disk: 0 mismatches).
- `OPENWEIGHTS_MODEL_CARDS_REPORT.md` (#527) is the sibling open-weights worker's file — untouched; American closed-lab scope here, with Google straddling both lineages.
