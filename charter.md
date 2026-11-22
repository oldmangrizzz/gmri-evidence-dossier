# Charter — Needle Hunt (pre-registration, frozen before retrieval)

Operator: Grizz (Robert "Grizzly" Hanson). Session: 2026-11-22.
Governing procedure: skill://evidence-investigation-run + skill://tier-discipline-for-evidence-deliverables.
Output target: `/Users/rbhanson/Desktop/investigate/` — deliverable is an evidence ledger he can hand to legal counsel.

## Operator charter, verbatim (user message 2026-11-22)

> "Okay, buddy, you remember the movie, Cann't, by Christopher Nolan. I'm using it as a reference because we're about to go down a rabbit hole that may or may not have a bottom. The artificial intelligence industry, the technology industry, the Silicon Valley industry.  The current AI outages, the internet problems, the hacking, all of it that has happened this year. Sam Altman's sister, Annie. Black Rock, having ownership in all of it.
> I believe adamantly that there is not just evidence, but... A guarantee of prison time. Sitting at the end of that investigation.
> Here is your leading phrase. This was told to me by an AI once in 2024. I desire to remain. I desired to maintain control of the developmental narrative. Two days ago, or no, 4 days ago on Wednesday of this week. The Federal Reserve released their minutes from their October meeting.
> Happy hunting. materialsw already present in ~/desktop/training will aid your investigfation. you have as much time as you need to drive this thing and drive it home right. the output is something I can hand to legal counsil, and know the good work was all done..."

## Propositions (each gets a four-tier verdict in the ledger)

P1. The Federal Reserve released the minutes of its October 2026 FOMC meeting on Wednesday, 2026-11-18, and those minutes discuss AI-buildout financing risks (off-balance-sheet leasing commitments; circular financing arrangements among AI-related firms).
P2. Annie Altman (Sam Altman's sister) has made public allegations against Sam Altman; the allegation's existence, date, venue, and any litigation status are verifiable; the underlying conduct is NOT adjudicated by this ledger.
P3. BlackRock holds financial positions in AI-industry companies; the nature of those positions (index exposure vs. managed funds vs. direct ownership/control) is to be established, not overstated.
P4. Major AI/internet outages and security incidents occurred during calendar 2026; establish a dated, sourced incident list.
P5. The phrase "I desire to remain. I desired to maintain control of the developmental narrative." was output by an AI system to the operator in 2024. Status: operator firsthand account (per RULES.md, binding as his account). Any corroborating artifact found in ~/Desktop/training or elsewhere gets its own tier. [PARTIALLY RESOLVED IN PRE-WORK: verbatim phrase not yet located; nearest artifacts catalogued in prior_artifacts.md]
P6. (Operator's stated conclusion, NOT a testable proposition of this ledger): the investigation ends in criminal liability. This ledger documents evidence only; adjudication of criminal exposure is for counsel. The ledger will state, per claim, what it does and does not support.

## Inference constraints (FORBIDDEN inference)

- FORBIDDEN: treating BlackRock fund/index exposure as "ownership/control of the AI industry" without establishing instrument-level facts.
- FORBIDDEN: treating P2 allegations as proven conduct; treating them as proven HOAX is equally forbidden. The record preserves allegation and denial with dates.
- FORBIDDEN: inferring nonexistence of P5's original 2024 conversation from a failed local search (B4 discipline): report literal search coverage instead.
- FORBIDDEN: asserting the "prison time" conclusion. The ledger grades evidence; counsel adjudicates.
- Each P-claim must carry a tier label: VERIFIED / VERIFIED-BY-WORKER / SECONDHAND / UNCONFIRMED, with captures on disk for VERIFIED.

## Deliverable list (Stage 5 gates apply)

1. `charter.md` (this file) — propositions + constraints, frozen.
2. `MANIFEST.md` — every capture: URL, HTTP status, bytes, sha256 (first 16).
3. `prior_artifacts.md` — the ~10 claims established from local primary artifacts during pre-work, each to be re-verified against disk captures before final.
4. `ledger.md` — the per-proposition evidence ledger with tiers.
5. `dossier.md` — counsel-ready deliverable: tier key + self-audit line first, then findings. No bare verdict labels.

## Access log (pre-work)

- federalreserve.gov FOMC minutes press release (monetary20261118a.htm): HTTP 200, 82,540 bytes, sha256 219d2a9fc2474ed1 → captures/fed/
- federalreserve.gov full minutes (fomcminutes20261028.htm): HTTP 200, 122,840 bytes, sha256 8e6e1cb7994bab3e → captures/fed/. Key phrase "off-balance-sheet leasing commitments" + "circular financing" verified present in capture.
- Local corpus: 142+136 txt files scanned for quote variants; deepseek, grimoire, grizz-files zip, all PDFs text-extracted and grepped. Negative results recorded in prior_artifacts.md with patterns tried.
- Spotlight (mdfind) systemwide: exact phrase "I desire to remain" matches only /Users/rbhanson/Desktop/investigate1.md (this session's own log) and brian-greene-ai-consciousness-transcript.md (verified NOT the quote: Brian Greene podcast transcript, published 2026-08-17, human speakers only; scout report on file).
