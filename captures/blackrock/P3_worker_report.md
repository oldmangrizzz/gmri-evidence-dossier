# P3 — BlackRock's financial positions in the AI industry (worker memo, 2026-11-22)

Prepared by worker P3. All capture hashes verified against disk (see MANIFEST.md, rows 3–19, 2026-11-22).
Tier rule: VERIFIED = body captured on disk here. SECONDHAND = reporting about a primary, not captured.
No tier upgrades. Allegations attaching to named living persons are not treated as proven conduct
(not applicable here — no conduct allegations involved in P3; this memo is instrument-level only).

---

## Part 1 — OpenAI exposure (OpenAI is private; instrument-level facts)

### VERIFIED on disk (captured primaries)

1. **BTX — BlackRock Technology & Private Equity Term Trust** (closed-end fund, BlackRock Advisors LLC;
   registered CIK 1836057), SEC Form N-PORT-P, report date 2026-06-30 (filed 2026-08-25).
   - Capture: `captures/blackrock/btx_nport_2026-06-30.xml` (85,468 bytes, sha256 0901a12abecdf4c0).
   - Holding row (extracted from captured XML): `<name>OPENAI SERIES C</name> … <cusip>000000000</cusip>
     … <balance>33,445</balance> <valUSD>$22,999,688.37</valUSD> <pctVal>1.866038115696</pctVal>
     <fairValLevel>3</fairValLevel>` (Level-3 fair value; 1.87% of fund net assets).
   - Also in same capture (AI-adjacent private stakes): ANTHROPIC PBC $71.0M (5.76%), PsiQuantum $73.7M (5.98%),
     Databricks Series K $20.3M + Series L $1.1M, DeepGram $33.8M, Anduril $7.7M, Discord $7.8M.

2. **BST — BlackRock Science & Technology Trust** (closed-end fund, CIK 1616678), N-PORT-P, report date 2026-06-30.
   - Capture: `captures/blackrock/bst_nport_2026-06-30.xml` (90,216 bytes, sha256 076c488243946ac7).
   - Row: `<name>OPENAI SERIES C</name> <balance>43,625</balance> <valUSD>$30,000,341</valUSD>
     <pctVal>1.5888</pctVal> <fairValLevel>3</fairValLevel>` (1.59% of net assets).
   - Also: ANTHROPIC PBC $91.9M (4.87%), Anduril $73.1M across series, Databricks $84.5M, PsiQuantum $40.4M, SambaNova $33.5M.

3. **iShares A.I. Innovation and Tech Active ETF** (BlackRock ETF Trust, CIK 1761055; ticker IBOR),
   N-PORT-P, report date 2026-07-31 (filed 2026-09-25).
   - Capture: `captures/blackrock/ishares_ai_etf_nport_2026-07-31.xml` (52,055 bytes, sha256 80dfd1a27d92750f).
   - Row: `<name>OPENAI SERIES C</name> <balance>68,345</balance> <valUSD>$46,999,961</valUSD>
     <pctVal>0.3627</pctVal> <fairValLevel>3</fairValLevel>` (0.36% of net assets).
   - Also: ANTHROPIC SERIES G $109.0M (0.84%).
   - This is an actively-managed iShares ETF — i.e., retail-buyable AI direct private exposure.
   - NOTE: this filing was surfaced in-fixture via EDGAR full-text search (result list quoted verbatim in transcript),
     filing listed as `0001410368-26-099895:primary_doc.xml`, filed 2026-09-25, BlackRock ETF Trust (CIK 1761055).

### SECONDHAND (Bloomberg-reported, not BlackRock-primary; talks ongoing, not a deal)

4. BlackRock was reported (Bloomberg, via atlant-capital.ae and azrty.com summaries, Oct 5–6, 2026) to be
   "in talks" alongside Gulf funds (MGX-led syndicate, up to $10bn) to anchor an OpenAI round of ≥$30bn at
   ~$1.4tn pre-money valuation. "OpenAI and BlackRock declined to comment." **Nothing closed confirmed.**
   Status: UNCONFIRMED as a completed position — talks only, no BlackRock primary confirming participation.
   Not captured as a BlackRock primary; treated as reporting-about-reporting (SECONDHAND at best).

### No BlackRock 13F/N-PORT-verified direct equity stake in OpenAI beyond the fund vehicles above.
Search coverage: EDGAR full-text search `"OPENAI" formType:NPORT-P` June–Nov 2026 returned 176 filings,
4 by BlackRock-registered vehicles (BTX, BST, iShares A.I. Innovation and Tech Active ETF — captured here),
plus BlackRock ETF Trust filing 0001410368-26-066718 (June 2026, same series; not separately captured).
No BLK Inc. 13F row for OpenAI (private; not expected under 13F). BlackRock Global Allocation Fund and
BlackRock Strategic Income Opportunities (BSIIX) appeared in the SECONDHAND leveragedposition.com June-2026
roundup with OpenAI marks — their current N-PORT filings were **not** separately captured here (gap noted).

---

## Part 2 — Public-equity exposure via BlackRock funds (instrument-level)

### VERIFIED (captured primary): BlackRock, Inc. Form 13F-HR, Q3 2026 (filed 2026-11-13, accession 0002012383-26-003985)
   - Capture: `captures/blackrock/blk_inc_13fhr_Q3_2026_form13fInfoTable.xml` (23,440,363 bytes, sha256 40f4c99d600049b7).
   - Aggregate holdings across all BlackRock-advised discretionary accounts (13F = manager-level, covers BLK-advised
     accounts incl. iShares ETFs + active/institutional accounts; NOT a statement about one fund's position):
     - NVIDIA Corp: 1,944,804,615 shares; reported value $444,154,478,125
     - Microsoft Corp: 608,126,881 shares; $311,908,277,222
     - ALPHABET INC: 826,789,723 shares; $283,253,479,572 (combines GOOGL+GOOG class rows within the capture)
     - META PLATFORMS INC: 173,634,368 shares; $125,916,171,056
     - ORACLE CORP: 156,256,760 shares; $20,884,600,430
     - COREWEAVE INC: 29,719,011 shares; $2,589,120,251
     (Extraction method: XML parse, sums across duplicate issuer/class rows; script run logged in transcript.)
   - CAUTION (inference discipline): these are manager-aggregate positions across many client accounts; they do NOT
     mean "BlackRock the firm" owns all of this for its own account. They also do NOT break out index vs. active.

### VERIFIED (captured primary): iShares Core S&P 500 ETF Trust (IVV), N-PORT-P for 2026-06-30
   - Capture: `captures/blackrock/ivv_nport_2026-07-31_full.txt` (1,453,335 bytes, sha256 9d40ee48a6c088db).
     Retrieved from CIK 1100663 (iShares Trust), accession 0002071691-26-019760, filed 2026-08-27.
   - Rows extracted (regName = iShares Trust; report date 2026-06-30):
     - NVIDIA Corp.: 333,161,869 shares; $66,662,358,368.21; 7.506% of fund net assets (pctVal 0.07505932 of NA)
     - Microsoft Corp.: 102,180,706 shares; $38,115,446,952.12; 4.292%
     - Alphabet Inc. (GOOGL): 80,656,266 shares; $28,824,129,780.42; 3.245%
     - Alphabet Inc. (GOOG): 65,012,849 shares; $22,970,989,937.17; 2.586%  (combined Alphabet: 5.831%)
     - Broadcom, Inc.: 65,126,781 shares; $24,601,641,522.75; 2.770%
     - Meta Platforms, Inc.: 30,208,021 shares; $17,015,876,149.09; 1.916%
     - Oracle Corp.: 23,340,523 shares; $3,420,553,645.65; 0.385%
     - Marvell Technology, Inc.: 12,043,614 shares; $3,587,672,174.46; 0.404%
     - CoreWeave Inc: **0 shares** — no CoreWeave row in the 508 `<invstOrSec>` rows parsed (checked CUSIP 21873S108; absent).
   - Context: IVV's holdings are 14.9%–17.6% of BLK Inc.'s 13F aggregate for the five largest names — consistent with
     BLK Inc.'s 13F being a manager-level aggregate much larger than a single ETF. [INFERENCE, arithmetic shown above,
     computed from the two captured primaries; not asserted as an official ratio.]

### VERIFIED (captured primary): BlackRock Technology Opportunities Fund (BGHAX), N-PORT-P for 2026-08-31
   - Capture: `captures/blackrock/blk_tech_opps_nport_2026-08-31.txt` (585,207 bytes, sha256 7936472e331abf99);
     BlackRock Funds (CIK 844779), accession 0000940400-26-041352, filed 2026-10-26.
   - Rows extracted:
     - NVIDIA CORP: 3,669,206 shares; $810,087,301; **10.28%** of fund net assets
     - MICROSOFT CORP: 1,063,939 shares; $539,725,615; **6.85%**
     - ALPHABET INC: 655,998 shares; $222,612,921; **2.83%**
     - ORACLE CORP: 231,588 shares; $34,534,403; **0.44%**
   - This is an ACTIVE BlackRock mutual fund with concentrated NVIDIA/MSFT weights — demonstrates that BlackRock's
     active funds (not only index products) hold large AI-exposure weights.

### VERIFIED (captured primary): other captured BlackRock funds — CoreWeave rows
   - BTX (report 2026-06-30): CoreWeave Inc, 57,114 shares, $5,685,128, 0.4613% (Level 1)
   - BST (report 2026-06-30): CoreWeave Inc, 74,628 shares, $7,428,471, 0.3934% (Level 1)
   - iShares A.I. Innovation and Tech Active ETF (report 2026-07-31): CoreWeave Inc, 1,965,396 shares, $141,056,471, 1.0885% (Level 1)
     — all from the three N-PORT-P captures listed above.

### Coverage gap — recorded, not silence
No BlackRock Technology Opportunities / Large Cap Growth-type fund N-PORT was captured for Alphabet or Meta weight
comparability (the Technology Opportunities Fund is the one active-fund N-PORT captured this pass). No 5%+ beneficial
ownership (13D/13G) filing by any BlackRock entity on CoreWeave/NVIDIA/Microsoft/Alphabet/Meta/Oracle was found in
EDGAR full-text search (coverage: subject CIK 1769628 for CoreWeave — 33 13G-family filings, 13 filer groups, none
BlackRock; other issuers not exhaustively enumerated on subject-CIK basis — gap noted). Nonexistence of a >5%
BlackRock stake in these issuers is reported as: **EDGAR FTS-negative, not a verified null**.

---

## Part 3 — BlackRock's AI infrastructure financing vehicles (BlackRock's own communications first)

All captured on disk; all VERIFIED.

### A. GAIIP launch — 2024-09-17/18 (capture `blk_gaiip_launch_2024-09-18.htm`)
   - "BlackRock, Global Infrastructure Partners (GIP), Microsoft, and MGX announced the Global AI Infrastructure
     Investment Partnership (GAIIP) to make investments in new and expanded data centers…"
   - "$100 billion investment potential"; "initially seek to unlock $30 billion of private equity capital over time"
   - NVIDIA supporter; investments "chiefly in the United States"
   - Fink quote: "Mobilizing private capital to build AI infrastructure like data centers and power will unlock a
     multi-trillion-dollar long-term investment opportunity."
   - Footnote (page footer): "On September 13, 2024, BlackRock issued a press release announcing that it expects to
     close its previously announced acquisition of GIP on October 1, 2024" (GIP → BlackRock, completed 2024-10-01).

### B. AIP expansion — 2025-03-19 (capture `blk_aip_nvidia_xai_2025-03-19.htm`)
   - NVIDIA and xAI join the partnership (renamed AI Infrastructure Partnership, AIP); GE Vernova and NextEra Energy
     agree to collaborate on energy for AI data centers.
   - "The partnership will initially seek to unlock $30 billion in capital from investors… which in turn will mobilize
     up to $100 billion in total investment potential when including debt financing."
   - Fink quote verbatim (captured page): "AI has the potential to transform the global economy if we can build the
     necessary infrastructure to support it. We believe this unparalleled partnership of leading global companies
     across the AI ecosystem brings technology expertise together with private capital to meet this demand and
     creates unique investment opportunities for our clients."

### C. Aligned Data Centers acquisition — announced 2025-10-15, CLOSED 2026-07-21 (both captured: `aligneddc_acquisition_announce_2025-10-15.htm`, `aligneddc_acquisition_close_2026-07-21.htm`)
   - Consortium: **AIP + MGX + BlackRock's GIP**. Acquired **100% of the equity** in Aligned Data Centers from
     Macquarie Asset Management-managed funds + co-investors; enterprise value ~$40 billion.
   - Aligned at close: 51 campuses, >6.4GW operational and planned capacity (Northern Virginia, Chicago, Dallas,
     Ohio, Phoenix, Salt Lake City, plus São Paulo, Querétaro, Santiago).
   - "The transaction is AIP's first investment"; "In connection with the closing, the consortium has also committed
     an additional $5 billion of growth capital."
   - AIP's financial anchor investors include Kuwait Investment Authority and Temasek (per announcement release).
   - Note: This is the instrument-level, deal-level evidence that the BlackRock/GIP/AIP consortium HOLDS (post-close,
     2026-07-21) a direct, whole-company position in a major AI/data-center infrastructure operator. It is a fund/
     consortium position — not an owned BlackRock corporate asset.

### Stargate links
"Stargate" (OpenAI/SoftBank/Oracle AI infrastructure venture) is NOT named in any captured BlackRock primary as an
AIP/GIP/BlackRock investment. Search coverage: EDGAR FTS + BlackRock press-release pages captured; the diginomica
interview capture (below) includes Fink discussing "two more platforms throughout the world" but no Stargate mention.
SECONDHAND mentions (atlant-capital.ae; azrty.com) place MGX (not BlackRock) as a Stargate equity partner. Verdict
for P3-claim "BlackRock/AIP participates in Stargate": **UNCONFIRMED — no primary evidence found; no assertion made.**

---

## Part 4 — BlackRock statements on AI capex / financing risk (dated, verbatim; all captures on disk)

### A. Fink 2026 Annual Chairman's Letter (capture `blk_fink_annual_letter_2026.htm`, fetched today)
   - "Now AI threatens to repeat that pattern at an even larger scale — concentrating wealth among the companies
     and investors positioned to capture it." (letter section 3)
   - "When we talk about the economic disruption of AI, most of the conversation is about jobs." (section 3)
   - "AI may accelerate this trend further. The companies with the data, infrastructure, and capital to deploy AI
     at scale are positioned to benefit disproportionately." (section 3)
   - "One thing is clear: AI will create significant economic value. Ensuring that participation in that growth expands
     alongside it is both the challenge and the opportunity." (section 3)
   - "And when the Magnificent 7 companies build out data centers or power infrastructure, even they turn to the
     capital markets." (section 1, footnote 6 context; verbatim sentence on captured page)
   - "We cannot have just five companies or seven companies entirely buying out every chip production that is being
     produced right now." — from the CNBC/diginomica interview capture, not the letter (below)
   - Letter does NOT discuss AI-financing risk in the specific "circular financing" terms; its AI content is
     wealth-concentration/opportunity framing.

### B. Fink interview statements on AI financing risk (all via captured THIRD PARTY transcripts of interviews; quote content is Fink first-person, capture is SECONDHAND for the quote's verbatim-ness because I captured the news pages, not CNBC's raw footage)

   1. **CNBC-sourced capture** (`fink_cnbc_others_2026-08-12_nvidia_financing.htm`, CNBC 2026-08-12 by Tobias Burns):
      - CNBC paraphrase: "Larry Fink, CEO of BlackRock, one of Nvidia's financing partners, compared Nvidia's computing
        power assets to the 'mortgage-backed securities market in the 1970s.'" (this is a quote-of-attribution captured on CNBC's page)
      - "The financing announcement immediately raised questions about more circular financing, but investors say the
        bigger issue is how exactly to value the assets that will be used as collateral."
      - Michael Burry (in same capture, quoted): "This also has shades of Enron's effort to make wholesale power an
        investable class… Structuring unnatural credits to prolong momentum late in the bull phase is where the worry comes in."
      - Wells Fargo traders (same capture): "One outstanding question is whether this all means that AI factory loans
        will eventually become repackaged into [a] collateralized loan market."
   2. **diginomica capture** (`diginomica_fink_captial_shortage_2026-10-16.htm`):
      - Fink, verbatim in capture: "For the first time in my career, and that's 50 years of a career, I'm seeing genuine
        shortages of capital."
      - Fink: "I don't see us having the ability to raise trillions and trillions of dollars of bespoke transactions
        related to data centers."
      - Fink: "Compute capacity is now following a similar path, and we intend at BlackRock to be the center of it as
        we were then in the beginnings of the mortgage-backed securities market… As compute capacity emerges as an
        asset class, the markets will need trusted data, standardized performance metrics and a common framework for
        risk analytics."
      - Fink: "We're now seeing financing for the data centers that are based on the lease of the credit, but now what
        we are also witnessing the need to build out the scale of chips and compute. If we're going to democratize AI,
        the faster we could do this, the better we'll be in broadening economic success."
      - Fink: "We're actually looking at two more platforms throughout the world where we could play a larger, larger
        role. As one of the largest shareholders of every major public hyperscaler and technology platform, we're having
        broad-based conversations with all of them."
      - Fink: "If you think about a 1 gigawatt data center in the United States is about a $50 billion enterprise cost,
        40% of that is the cost of GPUs and chips. The other 60% is power, grid, core and shell."
      - diginomica paraphrase: "It's just one exemplar of what can be done… the example of his firm's work with Meta on
        financing its planned $14 billion data center in Texas." (paraphrase; capture text)
   3. **Yahoo Finance capture** (`yahoo_fink_moratorium_recession_2026-10-16.htm`):
      - Fink, quoted 2026-10-14 CNBC interview: "If we have a moratorium of some sort in this country, we will be in a
        recession." / "Data centers are not the problem. They're creating more new jobs than ever before."
      - Fink on AI bubble (per capture, May 2026 Milken panel): "I don't believe we're moving fast enough… There is not
        an AI bubble. There is the opposite. We have supply shortages. Demand is growing much faster than anyone has
        ever anticipated — and this is just a U.S. phenomenon."

---

## Part 5 — What P3 does and does not support (inference discipline, charter-compliant)

**Supported by VERIFIED instrument-level evidence:**
- BlackRock funds (BTX, BST, iShares A.I. Innovation and Tech Active ETF) hold SEC-reported stakes in OpenAI
  (OpenAI Series C) as of 2026-06-30/2026-07-31, totaling ≈$100M in fund-level fair value at Level 3 marks; plus
  ANTHropic Series G/H, PsiQuantum, Anduril, Databricks, Deepgram, SambaNova, etc., in the same captured filings.
- BlackRock Inc.'s 13F aggregate (Q3 2026) includes very large positions in NVIDIA/MSFT/Alphabet/Meta/Oracle and
  29.7M shares of CoreWeave ($2.59B reported value).
- The AIP+MGX+GIP consortium closed acquisition of 100% of Aligned Data Centers equity on 2026-07-21 (~$40bn EV),
  making this vehicle-level whole-company exposure to AI data centers, not an index holding.
- AIP (BlackRock/GIP/Microsoft/MGX/NVIDIA/xAI) is a formally announced financing platform targeting up to $100bn
  including debt, per BlackRock's own releases (2024-09-17, 2025-03-19).

**Not supported / not asserted:**
- "BlackRock owns the AI industry" — no. Captured evidence shows: (a) 13F positions are manager-aggregate discretionary
  holdings across clients, not BlackRock corporate assets; (b) IVV's own holdings are 14.9%–17.6% of those aggregates
  (arithmetic above) — i.e., index exposure is a large share of the manager-level totals; (c) the OpenAI and AI-venture
  positions are fund-level stakes, Level-3, small (1–6% of those individual funds' net assets); (d) Aligned/AIP is a
  consortium equity, not a BlackRock corporate asset.
- No evidence found in captured primaries that AIP/GIP/BlackRock is an equity partner in Stargate (MGX appears in
  secondhand reports as Stargate equity partner; BlackRock does not). UNCONFIRMED/no primary found.
- No completed OpenAI primary-round investment by BlackRock confirmed (the 2026 Oct "talks" reports are unconfirmed).

---

## Search-coverage log (what was actually tried, per B4 discipline)

- EDGAR FTS (`efts.sec.gov/LATEST/search-index`) queries run: `'formType:"SC 13G" "BlackRock" "CoreWeave"'` (0 hits);
  `"CoreWeave" forms=(SCHEDULE 13G, SCHEDULE 13G/A, SCHEDULE 13D)` (25 hits, 13 filer groups — none BlackRock);
  `"OPENAI" forms=NPORT-P startdt=2026-06-01` (176 hits; identified BlackRock-vehicle filings; all 4 captured).
  Full-text-search endpoint at `https://efts.sec.gov/LATEST/search-index` worked for these; a POST to the same
  endpoint (earlier in transcript) returned 0 — method noted per probe-vs-source discipline.
- EDGAR data.sec.gov submissions JSON API: BlackRock Inc (2012383) 13F-HR (captured latest, Q3 2026);
  iShares, Inc. (930667) 533 NPORT-P filings 2024-06-27→2026-11-13 (all 44 July-2026-27 filings listed & no
  S&P 500 trust among them); iShares Trust (1100663) 89 NPORT-P filed 2026-08-20→2026-09-01 (list captured);
  BlackRock Funds (844779) Technology Opportunities Fund N-PORT captured.
- Non-exhaustive (gap): 5%+ stake check (13D/13G) was run exhaustively only for CoreWeave; other issuers
  (NVDA/MSFT/GOOGL/META/ORCL) not exhaustively 13G-enumerated. Negative findings on those issuers = FTS-negative, not a verified null.
- SEC rate-limit block was hit during IVV retrieval (10-minute block, 2026-11-22 ~12:50 ET); block recorded in
  MANIFEST.md; IVV capture succeeded after backoff.
- No attempt made to read peers' files (charter discipline); no charter/prior-artifact edits.
