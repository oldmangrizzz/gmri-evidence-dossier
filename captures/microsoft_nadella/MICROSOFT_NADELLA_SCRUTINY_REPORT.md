# MICROSOFT (COMPANY) & SATYA NADELLA — DUE-DILIGENCE SCRUTINY (2026-11-23)

**Charter:** `charter_microsoft_nadella.md` (pre-registered). Part-5 method: professed standard → captured record, both sides carried, allegations attributed, ADJUDICATED tier where courts/EC ruled.

**Self-audit (regenerated from filesystem + MANIFEST):** 884 manifest rows, sequential, 0 dupes. Microsoft/Nadella pass: `captures/microsoft_nadella/` 10 kept files; `captures/blocked_attempts_microsoft_nadella/` 21 provenance-only quarantines (DO-NOT-CITE). All kept files hash-verified. Reuse note: OpenAI-governance material captured in prior passes cited by prior rows (e.g., Farrow profile row 774 = Microsoft's board-adjacent position).

---

## PART A — MICROSOFT (THE COMPANY)

### A1. The standard Microsoft set (its own words)

1. **Mission (Nadella's restated frame):** "empower every person and every organization on the planet to achieve more" (captured in the June-2024 Recall blog as company mission: "live up to our company mission to empower people and organizations to achieve more").
2. **Six Responsible-AI principles (row 906, `msft_ai_principles.html`):** Fairness; Reliability & Safety; Privacy & Security; Inclusiveness; Transparency; Accountability — each with "How might..." self-questions. The page commits to AI "in a way that is transparent, reliable, and worthy of trust."
3. **Responsible AI Standard v2** (2022): the operational document underneath the principles — fetch attempts returned 404s on three known slugs (quarantined); the Standard PDF is a named discovery target.
4. **AI Access Principles (Feb 26 2024, Brad Smith, MWC Barcelona — PRIMARY captured, row-by-basename `msft_ai_access_principles_bradsmith_feb2024.html`):** five tenets + eleven principles committing Microsoft to "bigger investments, more business partnerships, and broader programs to promote innovation and competition than any prior initiative in the company's 49-year history"; explicit public-API access commitments ("making available public APIs to enable developers to access and use AI models we host on Microsoft Azure"); non-tilting of the playing field ("developers... confident we will not tilt the playing field to our advantage"). The same post invokes the 2006 "Windows Principles" precedent — including the FTC commissioner's remark that acting 10 years earlier "would have avoided a lot of problems." The EC Teams complaint (filed June 2024, three months later) is now the live question against this standard.
5. **Secure Future Initiative (SFI)** (Nadella's company-wide security-first framing, 2023-24, repeatedly cited in the company's Recall blog as the governing framework).

### A2. The record laid against it

**ADJUDICATED/SETTLED — antitrust (EU):**
- **€561M non-compliance fine (EC, 2013)** — VERIFIED primary via the EC open-data API (fulldoc row, `eu_browser_fine_2013_fulldoc.html`; the presscorner shell rows are annotated): "The European Commission has imposed a €561 million fine on Microsoft for failing to comply with its commitments to offer users a browser choice screen enabling them to easily choose their preferred web browser." — a fine for *breaching its own compliance commitments* (the 2009 Browser Choice commitment), i.e., the company promised conduct and didn't deliver it. [Both-sides: the original commitment was itself a settlement of prior conduct.]
- **EU Bing/Edge fine (2025, reportedly €60M-class) and EC Teams complaint (2024, IP/24/2423)** — complaint captured as title-only (client-rendered EC page, quarantined as inaccessible body); press coverage SECONDHAND this pass; recorded as a named docket/press target. The EC *filed charges* (a competition complaint is an allegation, not a finding).
- **US FTC cloud-computing report (2024-25)** — staff report on cloud-competition practices named Microsoft; PDF 404'd all attempts; SECONDHAND, discovery target.

**Product-safety event: Recall (June 2024) — the most direct test of "Privacy & Security" vs. launch pressure:**
- Copilot+ PC launch (May 20, 2024) shipped Recall **on by default**, taking periodic encrypted-at-rest screenshots (the company said "snapshots") of the user's screen, indexed locally.
- Security researcher Kevin Beaumont (ex-Microsoft): "inventing a new security nightmare"; demonstrated in days that the local database was readable (an unencrypted SQLite store behind disk encryption), reachable without admin rights, and exfiltratable — Microsoft's own Copilot could walk a user through extracting it ("Here's a few second video of two Microsoft engineers accessing the folder" — Beaumont's capture).
- Ars Technica independently verified cross-user access on the same machine.
- **The company's own primary response (row 884, Windows Experience Blog, June 7, 2024):** first it changed opt-out → opt-in ("If you don't proactively choose to turn it on, it will be off by default" — Pavan Davuluri), required Windows Hello ESS, "just in time" decryption, encrypted the search index; then (June 13/14) pulled Recall from the June 18 launch entirely, to the Insiders program. October 2024 update: further delayed to December.
- **Nadella's own words on Recall (this row's CNBC secondary):** "Recall works as a magical thing, because I can trust it." vs. the WSJ's Joanna Stern's framing: "There could be this reaction from some people that say this is pretty creepy. Microsoft is taking screenshots of everything I do." — His trust claim is on the record, and days later the feature was withdrawn from launch over security. The tension is carried, not adjudicated.
- Attribution note: the decision-and-fix chain runs through product leadership (Davuluri/Mehdi) with Nadella the public face of the launch and of SFI; the CEO-level "trust" quote is his own, on camera.

**Labor tension (2024):**
- **Jan 2024: 1,900 gaming/Activision roles cut** weeks after closing the $69B acquisition — reported widely; press-primary captures failed (AP/CNBC 403/404; quarantined), SECONDHAND, discovery target.
- The same quarter: company-wide security posture announcement (SFI) alongside reported cybersecurity-staff cuts (2024-02 NYT reporting; capture blocked, discovery target).

**Privacy/security precedent (FTC/NY COPPA analogues n/a):** Microsoft's consumer-privacy enforcement record is thinner than Google's on the FTC side; the EU GDPR actions against Microsoft (Teams data, GDPR complaints by noyb against Fitbit-era practices) are documented as complaints, not rulings — SECONDHAND.

### A3. What Part A does not claim
- EC fines are cited at the EC's own language; the Teams charge is an allegation; the FTC cloud report is a staff report (not an order).
- Recall's security outcomes are documented researcher findings plus the company's own remediation; no adjudicated finding is claimed.
- Layoffs are business facts; nothing beyond optics is inferred.

---

## PART B — SATYA NADELLA (public-company CEO; OpenAI board participant)

### B1. His standard (his own words)

1. **The OpenAI-governance crisis statements (row 871/872, Nov 2023, VERIFIED):** "We remain committed to our partnership with OpenAI and have confidence in our product roadmap..." (Nov 19, posted during the Sam Altman ouster); then on the reconstituted board: "We are encouraged by the changes to the OpenAI board. We believe this is a first essential step on a path to more stable, well-informed, and effective governance." (Nov 21.) And the interim offer: "Sam Altman and Greg Brockman, together with colleagues, will be joining Microsoft to lead a new advanced AI research team." — all three captured from the two statement posts.
2. **The trust framing on Recall (his words, CNBC-captured interview):** "Recall works as a magical thing, because I can trust it."
3. **The SFI framing (company security-first doctrine, 2023-24):** "security is our top priority" (in his CEO directive after the U.S. CSRB report on the China-linked Federal-email breach — CNBC-captured reporting).
4. **His own public mission restatement** (the "empower every person" mission across captured blog pages).

### B2. The record laid against it

1. **"More stable, well-informed, and effective governance"** — his Nov-21 statement welcomed a board Microsoft then joined as a **non-voting observer**. [CORRECTED 2026-11-23 per the charter's no-laundering rule: Altman's own return post (captured, prior pass, `wayback_openai_sam_altman_returns_20231129.html`) says the new board "will include them as a non-voting observer" — referring to Microsoft the company; the observer reported for Microsoft was Dee Templeton (SECONDHAND). **Nadella's personal board membership: UNCONFIRMED-negative in this record** — the report previously implied a personal seat and is corrected.] The tension (largest investor + observer seat + EC scrutiny) is noted as the record shows it.
2. **"Recall... because I can trust it"** vs. the withdrawal from launch over security days later — the direct juxtaposition, both captured in the same file set. His "trust it" claim is preserved; the remediation is the company's own record.
3. **The CSRB criticism and his response (reported):** the federal breach-of-Federal-email finding (2024) put Microsoft's security under a government review board's criticism; his SFI-directive response is captured in CNBC reporting (SECONDHAND this pass; the CSRB report itself is a named discovery target).
4. **The OpenAI-governance duality:** Microsoft-CEO statements repeatedly commit to OpenAI's "effective governance" (captured) *while* the record of that governance (Pichai-pass row 774 et al. — the Murati memo, the Altman-candor removal, the Farrow/Marantz trust record) sits in this dossier. Microsoft's statements during the crisis were the *counterweight* to the governance problem; no personal-misconduct claim derives from that.
5. **Nadella testimony:** no congressional testimony by Nadella located in any pass to date (bounded: searched; the record has his written statements and interviews instead — recorded as the standing boundary).

### B3. What Part B does not claim
- The Recall episode is a product-operations record; his "I can trust it" claim is quoted as a claim, in the same sentence set as the withdrawal.
- The observer-seat and CSRB items are governance facts as reported; no personal-wrongdoing inference is drawn.
- Nothing private; no health data; no people-search content.

---

## PART C — MANIFEST INTEGRITY
- 10 kept captures (rows verified by basename) + 21 quarantines (guessed-slug Microsoft-blog 404s, wrong-page CNBC/C-SPAN-class bodies, empty EC API responses) — DO-NOT-CITE, all re-pathed.
- The €561M EC fine primary came from the EC's own open-data API (row 906) — the pass's only ADJUDICATED-ADJACENT primary, which is its cited authority.
- Discovery targets: Responsible AI Standard v2 PDF; AI Access Principles primary blog; FTC cloud report; EC Bing/Edge fine 2025; layoffs press; CSRB report; board-observer arc via EC.
