# captures/

Evidence captures: primaries and derived OCR/text extractions.

**Every capture's URL, HTTP status, byte count, and SHA-256 hash is recorded in `MANIFEST.md` at the repo root.** This allows counsel or a third party to independently re-fetch and verify each primary by hash.

Some large binaries are excluded from the git repo by `.gitignore` (see `.gitignore` at root); their SHA-256 hashes are recorded in `MANIFEST.md` and the original files are retained by the operator. Specific excluded files are listed by name in the ignore list with matching MANIFEST rows.

Subdirectories:
- `altman/` — 64 files, Altman v. Altman docket, dismissal orders, Notice of Appeal, media captures
- `fed/` — Federal Reserve FOMC minutes, press release + full minutes, sha-verified
- `dockets/` — 9 primary captured dockets and complaint PDFs (Raine, Gavalas, Buist, Alfozan indictment, 8-state AG suits, etc.)
- `icloud_ai_logs/` — operator AI interaction record (Gemini / Claude / ChatGPT / Siri); OCR'd page-by-page; includes operator behavioral dossiers compiled at operator request; includes accommodation notice
- `gemini/` — operator Gemini interaction captures
- `claude_log/` — Claude-authored ethical breach report + OpenAI conversation exports (hash verified)
- `incidents/` — 2026 incidents/enforcement captured primaries (FTC, SEC, DOJ, Cloudflare, AWS, Anthropic)
- `blackrock/` — BlackRock instrument-level primaries (13F, N-PORT, GAIIP/AIP, DC acquisitions, Fink statements)
- `ada_case_law/` — ADA case-law captures (Magee full text, A.L. v. Disney full PDF, corpus-derived case tables tiered SECONDHAND)
- `chatgpt_health/` — ChatGPT Health product page, Health Privacy Notice, main Privacy Policy, GMRI regulatory exposure
- `statutes_fcc_dtpa_ada/` — full statutory captures (FCC CVAA §255/§617, CFR Part 14, ADA Title III, Section 504, TX DTPA ch. 17, TDPSA ch. 541, 16 CFR Part 318 HBNR, FTC Act §5)
- `local_sources/` — TX AG judgment, TEC lobbyists list, FCC CVAA biennial
- `operator_biography/` — GMRI Biographical Record v1.5/v1.4/v1.3 + Archival Record PDF (self-authored archival records)

Large binaries excluded by `.gitignore` are documented by name in the manifest. If a specific capture is needed and it's not in the repo, check `MANIFEST.md` for hash and source URL, or contact GMRI.
