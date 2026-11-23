# SATYA NADELLA — DUE-DILIGENCE SCRUTINY (THE PERSON) — standalone pass (2026-11-23)

**Charter:** `charter_nadella_person.md` (row 1025). Part-5 method: professed standard → captured record, both sides carried. Prior Microsoft/Nadella pass reused by basename. Two prior-pass wording defects repaired in this report per the charter's pre-registration.

**Self-audit (regenerated from filesystem + MANIFEST):** 1,025 manifest rows, sequential, 0 dupes, 0 gaps. This pass: 9 captures in `captures/nadella_person/` (rows 1016–1024) + the charter (row 1025); report row follows. All hash-verified. Blockages recorded: cisa.gov CSRB-report PDF 404 (direct + wayback, both), WSJ article 401 (paywall; wayback capture is a headline stub — kept), YouTube caption-track empty (timedtext API returned 0 B; video page kept), Benzinga 403 (wayback captured), sdw.space 522 (wayback captured). Reuse: `captures/microsoft_nadella/` 13 kept files, all prior rows.

**The operator's framing (on record):** "now do the same for satya nadella as a standalone pass."

---

## PART A — HIS PROFESSED STANDARD (his own words, VERIFIED)

1. **The security directive to all employees (2024-05-03; `captures/nadella_person/msft_blog_prioritizing_security_above_all_else.html`, VERIFIED — his own communication, made public as an official record):** "Today, I want to talk about something critical to our company's future: prioritizing security above all else. Microsoft runs on trust, and our success depends on earning and maintaining it." Plus the three SFI principles: "Secure by Design: Security comes first when designing any product or service. Secure by Default: Security protections are enabled and enforced by default, require no extra effort, and are not optional. Secure Operations..." Plus: "we will instill accountability by basing part of the compensation of the senior leadership team on our progress towards meeting our security plans and milestones." And the tradeoff clause: "If you're faced with the tradeoff between security and another priority, your answer is clear: Do security. In some cases, this will mean prioritizing security above other things we do, such as releasing new features or providing ongoing support for legacy systems."
2. **The recall-trust claim (2024-05-20, WSJ/Stern interview; transcript chain captured — `captures/nadella_person/benzinga_nadella_recall_quotes.html` via web.archive.org quoting the interview, VERIFIED; video page also captured):** "This is my computer, this is my Recall, and it’s all being done locally. So that’s the promise." + "That’s one of the reasons why Recall works as a magical thing, because I can trust it that it is on my computer." [CORRECTED from the prior pass: this quote's attribution is now anchored to a saved capture, not the prior report's uncaptureable "CNBC secondary" label.]
3. **The trust framing on AI agents (same WSJ interview; SECONDHAND — the video page is captured (\`wsj_nadella_interview_video_youtube.html\`) but its caption track returned empty this pass, so the wording is carried from the interview's widely-syndicated transcript text and is a named discovery target for the primary transcript):** "It's a personal, maybe even spiritual decision" (agent choice) + "The future I see is a computer that understands me versus a computer that I have to understand." [Quotes NOT yet VERIFIED against a saved transcript — tiered accordingly.]
4. **The OpenAI-crisis statements (Nov 2023; `captures/microsoft_nadella/msft_nadella_openai_statement_all3.html` + `_nov19`/`_nov21`, VERIFIED):** "We remain committed to our partnership with OpenAI and have confidence in our product roadmap..." (Nov 19) → "We are encouraged by the changes to the OpenAI board. We believe this is a first essential step on a path to more stable, well-informed, and effective governance." (Nov 21) → the interim offer: "Sam Altman and Greg Brockman, together with colleagues, will be joining Microsoft to lead a new advanced AI research team." (Nov 19.)
5. **The mission restatement (`captures/nadella_person/satya_nadella_wikipedia.html`, VERIFIED as the Wikipedia-with-citation record):** under Nadella, Microsoft revised its mission to "empower every person and every organization on the planet to achieve more". [Wikipedia citation note: the capture carries the period outside the quotation mark] with a cultural shift emphasizing "empathy, collaboration, and 'growth mindset'." His book `Hit Refresh: The Quest to Rediscover Microsoft's Soul...` (2017).
6. **The open-source pivot (captured):** "Microsoft ❤️ Linux" — proclaimed in contrast to previous Microsoft campaigns against Linux; Linux Foundation Platinum member 2016.

---

## PART B — THE RECORD LAID AGAINST THAT STANDARD

### B1. ADJUDICATED/SETTLED (EU antitrust — company carries the fines; carried at company tier)

- **€561M EC fine 2013 (`captures/microsoft_nadella/eu_browser_fine_2013_fulldoc.html` + EC API row, VERIFIED):** "The European Commission has imposed a €561 million fine on Microsoft for failing to comply with its commitments to offer users a browser choice screen..." — a fine for breaching the company's own settlement commitments. [Timeline check: Nadella became CEO in Feb 2014; the 2013 fine fell under Ballmer's tenure — carried at the company tier, NOT charged to Nadella personally.]
- **EC Teams complaint (2024, IP/24/2423) + 2025 Bing/Edge fine** — under Nadella's tenure; the complaint body was an inaccessible EC shell (quarantined); the 2025 reported fine is SECONDHAND. A competition complaint is an allegation, not a finding.
- **CSRB review (2024; `captures/nadella_person/satya_nadella_wikipedia.html` + Verge, VERIFIED as reported):** the DHS Cyber Safety Review Board's review of the Storm-0558 exchange intrusion; The Verge: the Board labeled Microsoft's security culture as "inadequate." **His response is the Part A standard item — the same-week "Do security" memo, with SLT compensation tied to security milestones.** The CSRB report PDF itself: 404 on cisa.gov and wayback this pass — named discovery target, blockage recorded.

### B2. The Recall episode — the direct test of the trust standard (company + personal, carried together)

- **His standard (captured, May 20, 2024):** "Recall works as a magical thing, because I can trust it that it is on my computer" + "it's all being done locally... that's the promise."
- **The record (researcher findings + company remediation, all captured):**
  - Kevin Beaumont (ex-Microsoft, quoted via `captures/nadella_person/sdw_space_recall_analysis.html`, VERIFIED): "Stealing everything you've ever typed or viewed on your own Windows PC is now possible with two lines of code — inside the Copilot+ Recall disaster." Q/A in the same capture: db files "just files in AppData, in the new CoreAIPlatform folder"; "Here's a few second video of two Microsoft engineers accessing the folder"; Microsoft's own Copilot AI could help write exfiltration scripts; Ars Technica verified cross-user access.
  - **The company's own remediation (`captures/microsoft_nadella/win_blog_recall_update_jun2024.html` + `cnbc_recall_optin.html`, VERIFIED):** opt-out → opt-in ("If you don't proactively choose to turn it on, it will be off by default" — Pavan Davuluri, June 7); Windows Hello ESS "just in time" decryption; then Recall pulled from the June 18 launch entirely (June 13), delayed to Insiders, then further delayed Oct. 31.
  - The juxtaposition is carried, not adjudicated: his "I can trust it" claim is quoted as a claim; the company's own withdrawal-from-launch for security reasons is the company's own record, 11 days later.
- **Both-sides note:** the decision chain the record shows runs through product leadership (Davuluri/Mehdi); Nadella is the launch's public face and the SFI's author. A second researcher's blunt assessment in the same capture: "Microsoft Recall is a dumpster fire. It should be a bigger story that it was somehow announced and shipped the way it was" — opinion, carried as such; the same capture also credits Microsoft's engineering ("there's a lot done to keep this truly local").
- **Elon Musk's counter-frame (captured, `benzinga_nadella_recall_quotes.html`):** Musk: "This is a Black Mirror episode... Definitely turning this 'feature' off" (PCMag-captured reporting) + "Maybe it is time to move consumer desktops to Linux." Carried as the other side of the record.

### B3. The OpenAI-governance duality (statements vs. the dossier's governance record)

- His Nov 2023 statements (captured): partnership commitment, welcome of the reconstituted board, the interim hiring offer — and "more stable, well-informed, and effective governance," welcomed while Microsoft became a non-voting observer. [CORRECTED 2026-11-23, carried from the prior pass: his personal board membership is UNCONFIRMED-negative; the observer reported for Microsoft was Dee Templeton (SECONDHAND); the observer seat belonged to Microsoft the company, per Altman's captured return post.]
- **His on-record denial to Musk's control claims (captured, VERIFIED):** Musk: "They own the code, the weights, everything! And GPT runs in a Microsoft data center." Nadella: "Look, while I have a lot of respect for Elon and all that he does, I'd just say that's factually not correct." Both sides in one paragraph.
- The dossier's OpenAI governance record (the Altman removal, "not consistently candid," the Murati memo) sits in other passes; his crisis statements were the counterweight — no personal-misconduct claim derives from that duality.

### B4. Labor record (company tier)

- **Jan 2024: 1,900 gaming/Activision roles cut** weeks after closing the $69B acquisition — press-primary captures failed (AP/CNBC 403/404, quarantined); SECONDHAND, discovery target. Business fact; nothing beyond optics inferred.
- GeekWire's related coverage headline in this pass's capture set: "Internal memo: Microsoft CEO addresses 'enigma' of layoffs amid record profits and AI investments" — carried as section provenance, not a capture of its own.

---

## PART C — WHAT THIS REPORT DOES NOT CLAIM

- The €561M fine predates his CEO term (Feb 2014) — carried at Microsoft-the-company tier, not charged to him.
- The Recall episode is a product-operations record researcher-verified plus company remediation; no adjudicated finding; his "trust" claim kept as a claim with its juxtaposition.
- The CSRB finding is a government review-board judgment ("inadequate" security culture) — not a court order; his response is the captured memo.
- The observer-seat arc: company-level; Nadella's personal board membership UNCONFIRMED-negative (bounded), the Templeton name SECONDHAND.
- Layoffs are business facts. No crime, no personal misconduct, no prediction anywhere. Every denial ("factually not correct") and every researcher opinion is carried beside what it answers.

## PART D — MANIFEST INTEGRITY

- 1,025 rows, sequential, 0 dupes, 0 gaps; this pass: rows 1016–1024 (captures), 1025 (charter), report row follows.
- All prior-pass reuse cited by basename. Blockages recorded: CSRB PDF (cisa.gov 404, wayback 404/504), WSJ direct 401 (stub kept, paywall noted), Benzinga 403 → wayback, sdw.space 522 → wayback, CISA report page 404.

## PART E — DISCOVERY TARGETS (named for a future pass)

- The CSRB report itself (both CISA URLs + wayback 404'd/504'd this pass — blockage recorded).
- The WSJ interview's full transcript (article paywalled 401 — wayback stub; the YouTube transcript API returned empty this pass).
- The EC Teams complaint IP/24/2423 full text (EC presscorner API path named in the closeout skill but not yet pulled).
- The 2025 EC Bing/Edge fine's primary order.
- The Microsoft Responsible AI Standard v2 PDF (quarantined 404s in the prior pass).
- The 2024 gaming-layoffs AP/CNBC primaries (both 403/404 this corpus).
- FTC cloud-computing staff report PDF (named in the prior pass; still UNCAPTURED).
- GeekWire's "Musk v. Altman: Nadella was worried about Microsoft being 'the next IBM'" piece (surfaced in this pass's capture set as related coverage).
