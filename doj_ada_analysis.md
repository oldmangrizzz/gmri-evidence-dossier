# DOJ/ADA Pathway Analysis — Legal-Framework Addendum (worker: AdoDojAnalysis, 2026-11-22)

**Recipients:** coordinating agent (integrates into dossier.md/ledger.md); downstream counsel.
**Scope:** ADA Title III (Meta/OpenAI), §504 Rehabilitation Act, DOJ CRT complaint pathway, the operator's "active interference" theory, and the FCC CVAA contrast. Applied strictly to documented facts in the operator's corpus.
**Evidence tiers:** VERIFIED = operator's capture on disk (hash-recorded) or statute/case primary captured this pass under `captures/statutes_fcc_dtpa_ada/doj_ada/` (rows below in MANIFEST); SECONDHAND = case law/media as reported; UNCONFIRMED = stated with reason.

**Corrective note (supersedes the November brief's framing):** the cert denial in *Magee* is **October 2, 2017**, Supreme Court Docket No. **16-668**, 583 U.S. — *not* October 2022. The Fifth Circuit opinion below is ***Magee v. Coca-Cola Refreshments USA, Inc.*, 833 F.3d 530 (5th Cir. Aug. 15, 2016)** (CA5 No. 15-31018, published). No 2022 Supreme Court proceeding in *Magee* was located (SCOTUS Oct. 3, 2022 order list 100322zor_c18e captured and contains no *Magee* entry). The operator's November 2026 brief and any prior dossier text citing "Magee … denial of cert … 2022" must be corrected before filing anything.

---

## 0. The operator's captured fact base (what the theories must fit)

From the operator's on-disk record (all VERIFIED unless noted):

1. **Meta lockout + AI-support denial (2026-11-11 support chat):** complete lockout of Facebook/Instagram/Quest; false "suspicious activity" basis; 2FA re-enabled without consent; recovery gated to (a) codes on a laptop destroyed years earlier, (b) a phone number Meta allegedly never updated, (c) ID-upload that repeatedly failed/crashed; **14+ explicit denials of any human agent or phone contact** ("there isn't a human agent for you to chat with… I do not have the ability to provide a phone number") including after the operator's explicit **Title III reasonable-accommodation request for a telephone line**; unprompted 988/mental-health insertion despite his contrary statements; session closed by Meta's assistant. Primary: `~/Desktop/training/grizz-files-2026-11-12/meta-recovery/evidence/2026-11-11_meta_ai_support_chat.md` (corpus; mirrored in dossier §5a).
2. **OpenAI flagging/termination conduct (2025):** June 2025 conversation record of threatened law-enforcement contact, "Flag Types & Triggers" self-description, "Behavioral Pattern Tracking" language; operator's account of flagging triggered by uploading the Apollo evaluation-awareness paper (as recited in the capture — the flagging event itself is his account); account deactivations/unusual-activity cycles as described in his record. Captures under `captures/icloud_ai_logs/` (chat_p200, wys_p200, more_threats.txt, ledger rows 190-371). **Model-authored statements are VERIFIED as captured text only, not as proof of internal architecture** (standing dossier rule).
3. **Siri/Apple evidence:** 8-file pack (`siri_zip/siri_evidence/`) — Siri "software tool" denials, "Uh oh, something's wrong" errors on long context, and the **content-flagging admission** (OCR-extracted 2026-11-22 from screenshot PDFs; flagging admitted while its logic is not disclosed). The pack is VERIFIED on disk; OCR derivations are persisted at `captures/statutes_fcc_dtpa_ada/doj_ada/derived_ocr_siri/t0-3_*.txt` (DERIVED tier, hashes in MANIFEST row 483).
4. **SSA status:** the corpus recites a **fully favorable SSA disability determination** as asserted in `FROM PREDICTABLE ERROR TO DELIBERATE HARM.pdf` §4 ("The investigator holds a fully favorable Social Security Administration disability determination") and in meta-recovery material. **The SSA award letter itself is not among the captures I located this pass** — it must be pulled (s.sa.gov / my SSA / FOIA to SSA) before any filing cites tier-1 evidence. Until captured: SSA status = SECONDHAND-TO-CORPUS (operator's own brief), UNCONFIRMED as a document.
5. **TBI origin (corpus):** line-of-duty assault with lead pipe while rendering patient care (Fort Worth), per the Meta chat and his biographical record; "medically retired paramedic," federally recognized disabled veteran per assignment background. The DD-214/VA rating doc is likewise not in my located captures — same capture-before-citing rule applies.

---

## 1. ADA Title III against Meta/OpenAI — the 5th-Circuit nexus problem

### Current law, cited correctly

- **Elements of a Title III claim (§12182(a), captured):** (i) discrimination "on the basis of disability," (ii) in "the full and equal enjoyment of the goods, services, facilities, privileges, advantages, or accommodations," (iii) "of any place of public accommodation," (iv) by a person who "owns, leases (or leases to), or operates" that place. **Everything turns on "place of public accommodation"** — the twelve categories in §12181(7) (captured, incl. (E) sales/rental, (F) service establishments), all read by the 5th Circuit as **physical**.
- **Fifth Circuit rule:** *Magee v. Coca-Cola Refreshments USA, Inc.*, 833 F.3d 530 (5th Cir. 2016): vending machines (and by extension standalone digital interfaces) are not themselves "places of public accommodation"; §12181(7) terms are "a physical place open to public access"; panel expressly followed the Third/Sixth/Ninth and departed from the First/Second/Seventh. Cert. denied Oct. 2, 2017, No. 16-668, 583 U.S. ___ (order list captured). Two important limits stated *in* the opinion: (a) it left open suit against the *host* public accommodation (hospital/bus station — i.e., where the inaccessible thing is embedded); (b) DOJ's cert-stage amicus (captured: `doj_crt_magee_amicus_brief_2017.pdf`) said the Court "did not adopt a 'physical entry rule'" and that "questions concerning Title III's application to nonphysical establishments — including websites or digital services — may someday warrant this Court's attention," expressly flagging the unresolved nexus question (¶ and n.5-6 of the brief).
- **2026 status check:** no en banc, no intervening 5th Circuit en-paneled authority overruling *Magee*'s physical-place rule was located this pass (CourtListener case-law search of the 5th Cir. return for *Magee* shows the 2016 panel, the 2017 cert history, and citing district courts — no superseding 5th Cir. holding). **Negative finding recorded, not asserted as exhaustive** ( CourtListener full-text; negative ≠ nonexistence). Practical reading: **a standalone web/app account system in the 5th Circuit faces a controlling adverse precedent**; the open question DOJ flagged (nexus between the *service* and a physical place) remains unadopted in the 5th Circuit.
- **What survives:** a plaintiff can plead Title III against an entity whose *physical* public accommodation embeds the discriminatory interface. Meta owns and operates physical places (office/campus spaces generally open to visitors; Meta Store, Burlingame; Quest retail channels), but **the account/recovery system is not embedded in a Meta-owned store the operator visited** — that's the gap a court would seize on. OpenAI is worse: no consumer-facing public accommodation at all. Apple retail stores exist (physical), but the Siri service is not embedded in the store's goods/service in the way an in-store kiosk would be.

### Elements-vs-evidence table (Title III — Meta, the strongest target)

| Element | Law | HIS evidence | Verdict / gap |
|---|---|---|---|
| Covered individual | 42 U.S.C. §12102; ADAAA broad construction | SSA fully-favorable determination recited in corpus; TBI documented; requests made in the capture | Element supported **once SSA letter is captured**; else SECONDHAND-to-corpus |
| Discrimination on basis of disability | Denial/accommodation refusal linked to disability | The capture shows the accommodation request (human/phone) made *because of* the neurocognitive limitation and refused as a category — Meta's assistant: "not an option," no meaningful interactive process (28 C.F.R. §36.302 obligations, captured) | **Met on the capture's face** for the interactive-process/accommodation denial |
| Public accommodation | §12181(7) physical categories; *Magee* 5th Cir. | None: lockout occurred through web/app; no nexus pleaded to a Meta physical place | **NOT met in the 5th Circuit as the record stands** — the claim-blocking element |
| Owner/operator of the place | §12182(a) | Meta owns/operates places, but not proven that the denied service is a privilege of one of them | Gap; would need location-specific facts (e.g., Meta Store visit) or a nexus theory |
| Reasonable modification feasible / fundamental alteration | §36.302(c), captured | A phone line plainly exists (Meta advertises support for other products); refusal given without undue-burden showing of record | Strong on feasibility **if** he gets past threshold |
| Remedies | §12188(a): injunctive relief only; damages only via DOJ civil action | NA for private suit money damages | Shapes relief expectations |

**Bottom line:** In the Fifth Circuit, his standalone-web-interface Title III theory is **doctrinally blocked by the circuit's physical-place rule** unless (a) a physical nexus theory gets adopted post-*Magee* (not current law there), or (b) facts tie a Meta physical place to the denied privilege. **The practical value of asserting Title III is (i) as the predicate for the DOJ complaint (which is not jurisdictionally barred) and (ii) as the record-creating accommodation demand** (the 2026-11-11 chat is a demand + refusal record).

**OpenAI:** all of the above and worse — no plausible physical-accommodation hook at all. Title III vs OpenAI is **UNCONFIRMED-viable at best; treat as non-route** in the 5th Cir.

### Where the nexus argument still has life (counsel note, SECONDHAND synthesis on VERIFIED sources)

DOJ's own amicus in *Magee* conceded the "websites/digital services" question is open and that the Fifth Circuit merely held "not every physical object is a public accommodation." A plaintiff could plead: Meta *sells* the Quest device and services through physical stores/channels (Category E/F analogue), the **support/recovery service is a privilege of that sales relationship**, and denial of telephone support for it is discrimination in the "privileges … of" the sales establishment. That is the *nexus* theory DOJ distinguished but did not foreclose (brief pp. 13-14: "Petitioner is not without redress … the hospital and the bus station … are indisputably places of public accommodation"). Counsel should weigh pleading it against *Magee*'s strict reading. Tier: legal-strategy SECONDHAND built on captured primaries.

---

## 2. Section 504 angle — is there a federal-funding hook for HIS claim?

**Law (29 U.S.C. §794, captured:** "No otherwise qualified individual with a disability … shall, solely by reason of her or his disability, be excluded from the participation in, be denied the benefits of, or be subjected to discrimination under any program or activity receiving Federal financial assistance…" — the "program or activity" limitation (since 1988) means §504 does **not** cover an entire corporate group merely because part of it takes federal money; it covers the specific program/activity receiving the assistance.

**Fact check against primaries:**

| Entity | Federal hook found | Verdict for HIS claim |
|---|---|---|
| OpenAI | DoD CDAO **$200M prototype OTA to OpenAI Public Sector LLC**, announced June 16, 2025 (DoD daily contract announcements; verified Reuters/CNBC/DefenseScoop; CDAO press release July 14, 2025 grouping OpenAI/Anthropic/Google/xAI at $200M each — captured `aimil_cdao…html` and `defensescoop…html`) | A §504 claim would have to allege discrimination **in a "program or activity receiving Federal financial assistance"** — i.e., the CDAO project. **The consumer ChatGPT product is a different program.** Under §504's program-activity language and the aid-conditionality cases, the consumer product is *not* covered; a consumer-side §504 claim against OpenAI is **weak to dead**. The funding fact is still useful for influence/oversight arguments and for asking federal enforcers to condition funds. |
| Meta | No federal financial assistance to the *social network* program located. (DoD-Meta Anduril AR headset work exists — corporate adjacency, not FFA to the account program.) | **No §504 hook.** |
| Apple | USAspending queries for Siri-related FFA not conclusive this pass; government device procurement is a purchase, not typically "federal financial assistance" under §504's meaning (assistance = grants, loans, use of federal property/contracts below threshold). | **No viable hook.** |

Also structural: §504's private right runs against **recipients of federal financial assistance**; the operator is not a beneficiary of the federally assisted program (the DoD), so his standing to sue on the defense contract is doubtful *Cummings*-line standing questions aside. **Conclusion (verify result, not assumption): the §504 theory in the brief is essentially a regulatory-pressure argument, not a litigation pathway for HIS consumer claims.** Downgrade it accordingly in the addendum.

---

## 3. DOJ CRT complaint pathway — what filing actually does

Captured primaries: `civilrights.justice.gov_portal.html`, `adagov_file_a_complaint.html`, `adagov_mediation_overview.html`, and the **CCD Rights Task Force letter (2024-03-28, captured PDF)** that contains the key data:

- **Volume:** From **January 2018 to June 2023 DOJ received over 95,000 Title III complaints** (per CCD letter describing DOJ's FOIA response). 
- **What DOJ concedes it does NOT do:** does not publicly report complaint data, does not tabulate complaints by issue, does not track or report dispositions (CCD letter; that is *why* they were writing).
- **Known processing behaviors:** complaints are screened by the Disability Rights Section; many are referred to the ADA Mediation Program (Key Bridge Foundation). Mediation is voluntary, free, "scheduled promptly" relative to investigation; program self-reports **more than 5,000 complaints mediated, >75% successful resolution** (ada.gov mediation overview, captured, last updated 2026-01-26; KBF page reports 7,000+ referrals, 79% agreement implementation). Investigation of individual complaints is rare; DOJ enforces mostly through pattern-or-practice and its own docket.
- **Timing data:** **no official complaint-processing time statistics exist** (that is the point of the CCD letter). UNCONFIRMED-with-reason: any specific median processing time — DOJ does not publish it; mediation referrals reportedly move faster than investigations but no numbers are on the record.
- **Practical expectation for HIS filing:** intake ack → possible referral to §308 mediation or to Meta's own dispute channel → likely no DOJ investigation; complainant retains full private-rights window (60 SLA not a bar to private suit). Filing is cheap, creates the agency record, preserves the "exhausted federal administrative channels" narrative the operator wants, and the **Nov 2026 DOJ CRT reorganization/AG priorities are SECONDHAND unknowns** — file, don't wait.
- **Strategic use of the Meta chat:** the captured accommodation demand + refusal is exactly the type of document DOJ's DRS screens for; it is short, dated, unambiguous. Attach it to every filing.

---

## 4. The "active interference with federally recognized rights" theory — does *Magee* break it?

The brief's §4 pivots off Title III to (i) "active interference," (ii) disparate impact on neurocognitive users, (iii) §504. Evaluating each against current 5th-Circuit law:

**(a) As a standalone tort/statutory cause of action:** there is **no federal cause of action** called "active interference with federally recognized disability rights." Title III needs a public accommodation (blocked above); Title II/§504 need program/funding hooks (absent); §1983 is inapplicable to private parties. **The theory does not survive as a pleading vehicle** in any court, 5th Circuit or otherwise. A generic civil-rights theory against private AI companies has no home unless a state analog exists.

**(b) As a *theory of the case* inside other claims:** it has real force but must be re-anchored:
 - **TX DTPA/TDPSA** (coordinator's other tracks): the "interference" narrative describes *conduct* — deceptive misrepresentations ("suspicious activity" recited as false in his capture; "safety" flags later admitted to be content-filtering in the Siri capture), unconscionable account-seizure with no human recourse. That is where the *money damages* remedy actually exists for him. The disability status functions as context/aggravation, not as a standalone claim.
 - **FCC CVAA (§255/§716)** — see §5: the *accessibility* interference theory fits here natively (functional-enjoyment denial of an advanced communication service), with FCC enforcement + RDA.
 - **Model-conduct evidence:** the captured accommodation refusal (Meta) is direct interference evidence *factually*; it's the evidentiary core, not the causes of action.

**(c) Does *Magee* break it?** *Magee* blocks the **venue** (Title III private suit) but not the **narrative**. The theory as drafted ("architectural substitution shifting the burden of proof back onto the disabled user") is a *characterization* of the captured conduct — the apology-reproduce cycle, the flagging of lawful research, the refusal of the accommodation channel. For the addendum: keep the theory; **strip it of implied §1983/Title III standing; run it through DTPA + FCC RDA + DOJ complaints + public-record pressure.** Tier: legal analysis (SECONDHAND synthesis on captured primaries).

---

## 5. FCC CVAA angle — 47 U.S.C. §255/§716 and why it is the practical route

*(Detailed enforcement mechanics are in the parallel FccEnforcement leg; here is the comparative-jurisdiction judgment.)*

- **Fit to HIS facts:** Meta's account system supports **advanced communication services (ACS)** — Messenger video/voice, WhatsApp, Quest social/voice — all "interconnected VoIP"/ACS under §716 and 47 C.F.R. Part 14. **Disabling access** to the services = denying "access to and use of" the service "by individuals with disabilities" if the inaccessible recovery path is the cause. The Part 14 definition (captured) includes performance, functional control, documentation, and **customer support, technical support and repair** — the exact thing denied (human support channel denied). Accessibility obligations are function-based, **not physical-place-based** — none of the *Magee* nexus problem applies. This is the only federal statute where his lockout story is a *textbook* violation without jurisdictional gymnastics.
- **Who is covered:** "Manufacturers" and "providers" of ACS/software. Meta as provider of Messenger/WhatsApp/Quest ACS is squarely covered. ChatGPT is not an ACS (no real-time interpersonal comms baked in) → CVAA route does **not** fit OpenAI's consumer chatbot. Siri: voice assistant embedded in telephony (ACS on iPhone) — partially plausible for the transcription-refusal leg, weaker than Meta.
- **Private rights:** none for §255/§716 in court; **but** two administrative channels exist (per 47 C.F.R. Part 14, captured + FccEnforcement leg): (1) **§14.35(a) Register of Disabilities Access (RDA) informal complaint** → provider must respond within 15 days (§14.35(b) per §618), then FCC complaint; (2) **§14.38 formal Enforcement Bureau complaint** (fee); (3) Disability Rights Office informal complaint. Outcomes: FCC orders, potential forfeiture (NAL), and — relevant to the *behavior* complaints — §618 authority.
- **Comparative verdict:** **FCC RDA/Part 14 complaint is the highest-probability enforceable pathway** for the Meta leg: no standing/jurisdiction fight, deadline-driven response, creates a federal record of the *same conduct* (denied telephone support as accessibility failure). DOJ ADA Title III complaint remains the narrative vehicle but with slow, discretionary processing. Private litigation: DTPA (damages), contract; **not** ADA Title III in the 5th Circuit. Recommended sequence for counsel: (1) file FCC RDA complaint on Meta ACS accessibility; (2) file DOJ CRT complaint (Title III + Section 504-adjacent framing) attaching the chat; (3) preserve DTPA/contract claims for court; (4) capture SSA/VA documents to convert status claims VERIFIED.

---

## 6. Consolidated theory table (elements → evidence → gap → tier)

| # | Theory | Elements (statutory) | HIS captured evidence | Missing | Tier | Verdict |
|---|---|---|---|---|---|---|
| 1 | ADA Title III — Meta | covered individual; discrimination; place of public accommodation; owner/operator; reasonable mod feasible | 2026-11-11 chat: accommodation demand, refusal ×14, no interactive process | **Place-of-accommodation nexus (5th Cir. *Magee*)**; SSA letter capture | Capture VERIFIED; law VERIFIED | **Blocked as private suit in 5th Cir.**; keep as DOJ-complaint predicate |
| 2 | ADA Title III — OpenAI | same | flagging/termination narrative captures | everything above + no physical place at all | Capture VERIFIED (conduct), law VERIFIED | **Non-route** |
| 3 | §504 (29 USC 794) | recipient of FFA; program/activity; denied benefits solely by reason of disability | none linking consumer product to federally assisted program | program-activity nexus; standing as non-beneficiary | Law VERIFIED; funding fact VERIFIED (DoD $200M OTA) | **Dead for consumer claims**; useful for federal-oversight narrative |
| 4 | DOJ CRT complaint (Title III framing) | n/a (administrative) | Meta chat + OpenAI pattern + Siri flags | complaint not yet filed; no timing stats exist | Portals/letters VERIFIED | **File**; expect referral/mediation; no guaranteed investigation |
| 5 | "Active interference with federally recognized rights" | needs a host statute | captured conduct supports narrative | **no cause of action**; Title III blocker | Analysis (SECONDHAND synthesis) | **Re-anchor** into DTPA + FCC RDA + public record |
| 6 | FCC CVAA §255/§716 (Meta) | provider of ACS; denied access/use; accessibility obligation incl. customer support; complaint channels | lockout + support-denial capture = direct | complaint not yet filed; ACS-scope analysis by FCC staff | Law VERIFIED (Part 14 captured); facts VERIFIED | **Primary practical route** for Meta leg (with DTPA for damages) |

---

## 7. Gaps the operator should close (nothing invented)

1. **Capture the SSA fully-favorable determination letter** (redact financial detail). Without it, every document reciting "federally recognized disabled individual" stays SECONDHAND-to-corpus.
2. **Capture DD-214 / VA disability letter / TBI medical records or line-of-duty documentation** for the "medically retired, service-connected TBI" representation counsel will need to plead standing and damages.
3. ~~OCR-verify the 4 image-only Siri PDFs formally~~ — **done this pass** (derived texts persisted at `derived_ocr_siri/t0-3_*.txt`, hashes in MANIFEST row 483). Outstanding flagging-admission exhibits should still be re-exported from the original device where possible for exhibit-grade capture.
4. **DoD-contract detail pull** (USAspending: award number for the $1,999,998 initial obligation under the $200M ceiling to OpenAI Public Sector LLC) if counsel wants the §504-funding fact at exhibit grade.
5. Optional: pull DPF (FCC) annual report and any 2026-2027 FCC accessibility rulemaking affecting support-channel duties (FccEnforcement leg has Nprm 26-76 etc.).

---

*Worker: AdoDojAnalysis. Statutory/regulation primaries, court-of-appeals opinion PDF, SCOTUS order list, DOJ amicus brief, complaint portals, CCD data letter, and DoD-contract primaries captured under `captures/statutes_fcc_dtpa_ada/doj_ada/` — see new MANIFEST rows appended by this worker. No changes to ledger.md/dossier.md per assignment.*
