[Trial audit log — 2026-11-22] Stage 5 discipline: apply every fix in place and log repairs transparently.

Applied (source: adversarial audit by separate reviewer agent, 13 findings):
1. ledger.md FOMC concentration row: attribution restored to "A few participants" (was merged under "Most participants").
2. ledger.md Fink CNBC row: circular-financing questions decoupled from Fink (report framing/investors), Burry kept separate speaker.
3. ledger.md Fink CNBC + diginomica rows: retiered VERIFIED → SECONDHAND (interview accounts; raw footage not captured).
4. ledger.md Aligned DC row + summary: ownership attributed to AIP+MGX+GIP consortium; "not a BlackRock corporate asset" note added (charter forbidden-inference fix).
5. ledger.md Azure row: PIR count corrected 2 → 3 Azure OpenAI incidents (8GCS-858, LYXT-C1Z, 7QL5-Z50).
6. ledger.md Cox row: $880k (captured order, CMG) split from $25k MindSift/1010 + $930k total (uncaptured FTC announcement; SECONDHAND).
7. ledger.md HN Algolia row: corrected nbHits=0-for-both to "1 human-story hit for 'I desire to remain'; 0 for 'I desired to maintain'".
8. p5 report: dated appended correction reconciling attempt counts (endpoint inventory governs).
9. dockets report: dated appended note — no dated Sam Altman response located for the 7 coordinated suits / FL civil suit; Raine denial is OpenAI's, not Altman's.
10. dockets report: dated appended correction — Florida matter is a criminal INVESTIGATION + separate civil suit; "referral" heading corrected.
11. prior_artifacts.md: Fed capture paths fixed to actual on-disk filenames.
12. ledger.md: first-X-post date conflict (Nov 14 UTC capture vs Nov 13 per Doc 18 ¶16) explicitly preserved.
13. ledger.md status line updated (BlackRock leg complete; not stale).

Post-fix gate rerun: all Stage-5 gates pass (charter verbatim quotes present, P1–P5 rows present, no tier-less capture rows, all capture refs on disk, Fed phrase in capture, denial present beside allegations, manifest > 150 rows).

Self-audit line for dossier: every DIRECT VERIFIED citation maps to a file on disk under captures/ (188 manifest rows, 182 capture files + 4 worker reports). Interview-sourced statements about living persons (Fink) are SECONDHAND. All allegations about living persons appear with dated denials or explicit no-response notes. The operator's P5 quote is his firsthand account; public corroboration not found; coverage documented; nonexistence not asserted. The "prison time" conclusion is outside this ledger's testable scope, per charter P6.


## 2026-11-23 — Model-card comparative analysis (charter_modelcards.md)
- Auditor: ObviousEel (reviewer agent, artifacts-only). Charter pre-registration verified via mtimes (charter 01:27:26Z before first capture 01:28:47Z).
- Blocker repaired: American-lab report was transcript-only → saved to captures/model_cards/AMERICAN_MODEL_CARDS_REPORT.md, quotes re-gate-checked against saved pdftotext derivatives (14/16 direct PASS; 2 PASS after pdftotext footnote-marker normalization, annotated in report).
- Scout attributions repaired: NTIA comment attributed institutionally; GDM FSF attributed to named authors; Amodei quote softened to "do potentially present a higher risk" + "very difficult" guardrails/monitoring; NVIDIA letter attributed to collective 260+ organizational signatories (Huang/Nadella = first signatories only).
- Falcon quote punctuation repaired; Mistral "stub" wording replaced with "discloses no benchmark or safety-evaluation results."
- GDM bad-PDF capture (133 B) moved to captures/blocked_attempts_model_cards/ and marked do-not-cite; GDM FSF re-fetched as blog HTML (143,811 B) and scout quotes re-gated: PASS.
- Open-weights report manifest references updated after sequential renumber (rows 493–509 → 511–526 region + reports).
- All 6 scout position statements captured to disk this pass (governance, frontier-ai-regulation, NTIA comment, GDM FSF blog, Anthropic position, NVIDIA letter; NVIDIA PDF quote "real and distinct risks" grep-verified in PDF text).
- Stage-5 gates at close: captures/model_cards 163 files + blocked_attempts_model_cards 48 + openweights_misuse 3 — all hash-verified vs MANIFEST (0 mismatch, 0 missing); 726 rows, sequential, 0 dupes.
