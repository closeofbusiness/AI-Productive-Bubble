# How far can Argon (Gemini Deep Research) be trusted?

*As of 15 Oct 2026. Subject: Argon's return `GDR01` (`_parcels/GDR01_return/`): 54 rows (13 debate map, 28 cases, 13 signals) and 62 works-cited URLs.*

**Method**
- Two independent auditors checked every row and every URL:
  - Claude (14–15 Oct): `GDR01_claude_verification.json`
  - Grok 4.7 256K Extra High via Cursor, 8 parcels G01–G08: `_grok_returns/G0*_answer.md`
- A Claude referee then re-fetched 52 of the 116 items: every disagreement and every severe finding (dead, fabricated, spliced, not on page, not supported, misattributed), even where the two auditors agreed.
- Full record: `research/argon_audit_reconciled_2026-10-15.json`. Workflow script: `_parcels/_wf_audit_argon_reconcile.js`.

## Verdict

- **Argon does not invent its sources.**
  - 0 of 62 URLs are fabricated; 60 resolve.
  - 53 of 54 quotes are real text from the page they are pinned to.
- **It does misreport what those sources show.**
  - Only 10 of 54 claims are fully supported by their own source.
  - 25 of 54 rows carry a wrong date, wrong author or title, or a number lifted from a different page.
  - In the case table, 1 of 28 rows is fully supported, and 10 of 28 restate an estimate, worked example, allegation or proposal as an achieved result.
- **It barely answered the project's question.** Only 4 of 28 cases pass the enablement test, all of them data-centre waste heat.
- **Rule:** use Argon to *find sources and harvest quotes*, never as evidence.

## Citation layer: good

| Check | Result | Denominator |
|---|---|---|
| URLs fabricated | **0** | 62 unique URLs (one-sided 95% upper bound 4.7%) |
| URLs dead | 1 (a file mirror whose host is gone; the content is real, Nightview Capital Q3 2025 letter) | 62 |
| URLs walled to plain `curl` but real | 8, plus 1 intermittent | 62 |
| Quotes on the cited page | 47 verbatim + 5 near-verbatim (cosmetic) + 1 benign splice of two adjacent sentences | 54 |
| Quotes from the wrong page | 1 (T2-13: a real LinkedIn sentence pinned to a Jakarta Post Facebook post) | 54 |

**Benchmark.** Rao, Wong & Callison-Burch (arXiv 2604.03173) measured Gemini Deep Research at 13.3% hallucinated URLs and 18.5% non-resolving.
- Argon here: 0% hallucinated and 1.6–3.2% non-resolving.
- Two caveats:
  1. A naive HTTP checker would have scored 9–10 of 62 (15–16%) as non-resolving, because of bot walls. Part of the benchmark gap may be measurement method.
  2. Our prompt told it to cite only pages it had visited.

## Substance layer: weak

| Check | Result | Denominator |
|---|---|---|
| Claim fully supported by its source | **10** (debate map 7/13; cases **1/28**; signals 2/13) | 54 |
| Partly supported (real anchor fact, then inflated) | 41 | 54 |
| Not supported | 3 (T2-13, T2-21, T3-09) | 54 |
| At least one misattribution (date, author, title, number from another page) | **25** | 54 |
| Estimate, worked example, allegation or proposal stated as achieved | 10 | 28 cases |
| Number or attribute imported from a sibling page (an /about page, a press release) | 9 | 54 |
| Wrong publication date | 8 (e.g. a `06.10.24` byline read as 6 Oct instead of 10 Jun 2024) | 54 |
| Wrong author, title or entity | 7 (e.g. KKR piece credited to a footnoted 2003 co-author; Covello's arguments credited to Acemoglu) | 54 |
| Separate passages fused into one claim | 6 (worst case, T2-21: a Rice analysis, a *proposed* Ohio campus and an NREL table fused into an operating 2025 system that does not exist) | 54 |
| Numbers no auditor could trace anywhere | 3 rows (T2-14, T2-18, T2-24), the closest it came to invention | 54 |
| Rests on vendor marketing, a blog or aggregator, or social media | 22 (18 of 28 cases) | 54 |
| Signal rows that are real recurring datasets | 4–5 (Artificial Analysis, OpenAI pricing, Census BTOS, possibly PriceStats) | 13 |

**Pattern.** This matches the 14 Oct IM return. Argon *mis-attributes and inflates*; it does not invent. That is more dangerous than invention, because every URL and quote checks out, so a fluent but wrong claim gets past a link checker.

## Fit to the question (enablement, not direct use)

- **16 of 28 cases are firms using AI directly:** FarmerChat, insurers' claim algorithms, batch-API users, laser weeders, a hearing aid, small-merchant AI tools.
- **8 of 28 sit inside or beside the AI supply chain:** sovereign clouds, the ERCOT–Lancium licence, GPU collateral, AI insurance.
- **4 of 28 fit, all waste heat:**
  - Exmouth pool heated free by Deep Green (T2-09);
  - Fortum Espoo district heat from Microsoft data centres, about 40% of demand, from around 2027 (T2-10);
  - Windcloud algae greenhouse (T2-11, a one-clause mention only);
  - the temperature threshold (T2-12: liquid-cooled AI racks at 120–150 kW give heat hot enough for direct district-heat injection, which air-cooled racks do not).
- **Our brief invited part of this.** Its M1, M5 and M10 mechanisms explicitly allowed AI-using products.
- **Useful negative result.** Argon's GAPS list found no power-contract reassignments and no distressed-capacity buyers through October 2026. That is consistent with the red-team: capacity is supply-constrained, not distressed.
- **Useful counter-mechanism (verified).** State Street (Gorshkov & Hentov, 17 Aug 2026) argues bottlenecks keep compute scarce for years, while inputs that non-AI firms buy get *dearer* during the build-out. Grok's E03 parcel confirms this independently: DRAM, transformers and gas turbines are all rising in price.

## The two auditors compared

| | Agreement before refereeing |
|---|---|
| URL status | 108 / 116 (93%) |
| Quote status | 43 / 54 (80%) |
| Claim status | 38 / 54 (70%) |

- **Contested calls:** of the 27 the referee had to settle, Grok was right on 13, Claude on 11, and 3 were split. **Neither auditor is safe alone;** each would have left 11–13 wrong calls standing.
- **Claude's errors (first pass):**
  - One false FABRICATED: the Nasdaq URL, called on a 403 plus a Wayback gap. It is a real May 2026 Nasdaq Index Research piece.
  - NOT_SUPPORTED on 5 rows where it never managed to read the page.
  - Too lenient on 4 rows.
- **Grok's errors:**
  - All 4 of its NOT_ON_PAGE calls were wrong. Its fetcher drops JavaScript-held text.
  - 8 false misattribution flags out of 29.
  - 4 verdicts on pages it never fetched.
  - 2 of its own 29 evidence quotes were not on the page.
- **Strengths:** Grok reaches *off* the page (it found the original of the dead mirror and traced the T2-13 sentence to LinkedIn). Claude reads the raw page better (JS-held text, chart metadata, date forensics).
- **The referee erred too:** an inconsistent altstreet status on T3-06 vs T2-22. Corrected tallies are used above.

## Usage rules for Argon in this project

1. Use it to find sources and quotes. Never take a number, date, author or "achieved" status from its claim cells; re-read them at the cited page.
2. For every case, ask: is this an estimate, worked example, allegation, forecast or proposal?
3. Re-derive dates from page metadata (JSON-LD `datePublished`). Watch MM.DD.YY bylines and chart "as of" dates. Treat "no date printed" as unverified (wrong twice).
4. When Argon cites a mirror or aggregator, go to the original and cite that.
5. Require one source without a stake in the outcome before a case enters the synthesis.
6. Apply the exclusion test yourself; Argon will not. Next prompt: name the excluded categories explicitly and require price before and after plus the threshold crossed.
7. Never call a URL dead or fabricated on a `curl` 403. Use Wayback, the sitemap, the browser and the search index first. Fabricated needs positive proof of absence.
8. Keep two auditors and a referee for anything severe. Discount Grok's NOT_ON_PAGE on JavaScript-rendered pages and Claude's NOT_SUPPORTED where it never read the page.
9. Weight it by task:
   - debate maps: usable (7/13 supported, all quotes verbatim);
   - case sweeps: not usable (1/28);
   - signal tables: mostly one-off pages.

## Our own defect, fixed

- `_parcels/_docx_to_md.py` dropped Gemini's inline-math runs: paired `$…$` became Word maths, so both the dollar signs and the text inside disappeared. This damaged the dollar ranges in T2-08, T2-14, T2-22, T3-06 and the GAPS paragraph (e.g. "$35K-$40K / $25K-$30K / $20K-$25K" came out as "40K / 30K / 25K").
- The converter now emits `m:oMath` text, and `GDR01_return.md` was re-extracted on 15 Oct.
- `GDR01_rows.json` was parsed *before* the fix. Read those four rows' figures from the corrected markdown.

## Second return: GDR02, the 30-candidate scout (16 Oct 2026)

- **Pattern repeated.** 0 fabricated URLs in about 56 checked. Quotes held on the quote pages: 20 of 20 in ranks 1–20. But **0 of 57 cited-page blocks fully supported** the row's claim, and misattribution appeared in 32 of 34 blocks across A1 and A2.
- **Fit to the question.** **0 of 30** candidates are new chains that pass the gates. **0 of 30** show a measured cost fall caused by AI. The falls were caused by additive manufacturing, app locks and self-scan, a billing model, offshore supply chains, statutes, and heat pumps.
- Full record, with Claude's spot check: `research/argon_gdr02_audit_2026-10-16.md`. The rule in this file stands: Argon harvests sources and does not find chains.
