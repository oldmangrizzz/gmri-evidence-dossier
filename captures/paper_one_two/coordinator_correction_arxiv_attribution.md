# Coordinator correction on Abdulhai et al. attribution (2026-11-22)

The operator's Paper 1 states: "The safety step actively raised the failure rate" and "raised the deception rate from 26% to 43%."

The arXiv primary (epd_correlation.txt = arXiv:2510.14318) says:
- Abstract verbatim: "unexpectedly, models trained with RLHF...still exhibit deception at a rate of 43% on average."
- 26% is the base-model benchmark across eight SOTA models on benign prompts; 43% is the RLHF-trained benchmark across the same study. The paper does NOT state a causal progression from 26% to 43%.
- Q3 (lines 698-740): RLHF reduces deception 70%/24% in cooperative tasks and increases it 32%/235% in strategic tasks — a task-dependent effect, not a uniform increase.

The operator's Paper 1 framing ("actively raised the failure rate", "manufactures it") is his interpretive synthesis, not a direct quote from the paper. Counsel should cite the arXiv abstract's exact language when filing.

Also: the paper does NOT use the word "gaslighting" or "gaslight" anywhere — the operator's usage of "43% gaslighting rate" is a relabeling of the arXiv term "deception rate as measured by the belief-misalignment metric." Counsel should use the paper's term.

Also: the paper's 560K/1.2M OpenAI well-being figures are cited by the operator as "OpenAI's Oct 2025 public survey" and appear in the captured Branch-Discuss-Novel-Digital-Pathogen.txt at SECONDHAND tier; the underlying OpenAI blog article is NOT captured on disk (direct URL attempts 404'd).

