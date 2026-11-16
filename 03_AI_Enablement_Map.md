# AI Enablement Map: what AI makes viable that is not AI

*Version 1.5 · 15 October 2026 · Claude (Opus 5.5). Answers the project owner's question of 15 Oct. v1.4 applied the F01–F08 follow-up round; v1.5 applies the F09–F15 round (§9, §10).*

> **Note, 16 Nov 2026:** `05_Mission_Statement.md` governs where it differs from this map. Web fiction (C-1) did not pass (05 §5.6, §7.1(c)). Rule (d) is not an exclusion: chains it removed go to a kept-and-scored second book (05 §4, §9 item 1, decided 16 Oct 2026). The findings below are unchanged.

**Basis:** 14 Grok research parcels, E01–E14, and 15 follow-up parcels: F01–F08 answer the v1.3 §9 next steps, F09–F15 the v1.4 ones. Materials are in `_parcels/E*_material.md` and `_parcels/F*_material.md`; returns are in `_grok_returns/E*_answer.md` and `_grok_returns/F*_answer.md`.

**Checks run on this map:**

| Pass | What it did | Result | Record |
|---|---|---|---|
| Verification (29 agents) | re-fetched all 578 evidence items; re-checked every calculation; re-judged ~95 candidates; cross-parcel critic | 567 verbatim, 1 same fact in other words, 10 behind bot walls, **0 spliced, invented or dead**; 11 arithmetic slips (§10) | `research/enablement_verification_2026-10-15.json` |
| Fact-check of v1 (8 agents) | 595 claims | 56 fidelity findings, 16 consistency issues, 8 readability notes, 8 evidenced leads | `research/enablement_mapcheck_2026-10-15.json` |
| Fact-check of v1.1 (5 agents) | 434 claims | 41 findings; 17 consistency issues (21 rows re-checked, 7 placements flagged) | `research/enablement_recheck_v11_2026-10-15.json` |
| Final check of v1.2 (2 agents) | fix application, and the line applied row by row | 15 fix-application gaps, 24 line issues | `research/enablement_finalcheck_v12_2026-10-15.json` |
| Follow-up round F01–F08 | re-fetched all 234 evidence items; re-checked every calculation; re-judged each answer and candidate under §0 | 218 verbatim, 16 behind bot walls (not used), **0 spliced, invented or dead**; 1 immaterial arithmetic slip (§10) | workflow `verify-followups` (`_parcels/_wf_verify_followups.js`) |
| Follow-up round F09–F15 | re-fetched all 216 evidence items; re-checked every calculation; re-judged each answer, candidate and lead under §0, with a counter-evidence search per candidate | 212 verbatim, 1 same fact in other words, 2 behind bot walls (not used), 1 not found as claimed (Grok's "404" for METI's results page, which is live), **0 spliced, invented or dead**; no arithmetic slips (§10) | workflow `verify-followups-r2` (`_parcels/_wf_verify_followups_r2.js`) |

- The findings of all four checks, and of a last look at v1.3 (`research/enablement_lastlook_v13_2026-10-15.json`), are applied, except the items listed under *Open* in §10.
- **The decisive change in v1.3** is rule (d) in §0. Only a **general-purpose** cost counts, the way bandwidth did for Netflix. That keeps all four of the project owner's excluded examples out, and it narrows the survivors.

**Labels:** every figure comes from a page a Claude agent re-fetched, unless marked:
- **VENDOR**: the company's own claim.
- **PRESS**: press only.
- **CALC**: our own arithmetic.
- **LEAD**: from a fact-check critic. The quote was checked, but the lead has not been researched in depth.

Candidate IDs C-0 to C-9 are stable across versions (C-3b, added in v1.4, is a sub-row of C-3, on the watch list since v1.5); research parcels are E01–E14 and F01–F15. Verdicts are Claude's judgement and name **candidate business classes, not picks**.

**Glossary** (terms from `01_Historic_and_Logic_Map.md`):
- **R1** write-down with transfer of control.
- **R4** price set by statute or contract.
- **R5** by-product sold at disposal value.
- **J3** energised data-centre capacity sold at ≤⅓ of undepreciated cost to a buyer outside AI.
- **Screen 10** a free layer the builder can withdraw.
- **L5** value goes to the scarce complement.
- **Map**, **01**: `01_Historic_and_Logic_Map.md` (the historic map; its §6 is the separate *strict third-claim* analysis).

---

## 0. The question, the tests, and the DIRECT line

> *"I am looking for business that are 'enabled' to grow on the back of AI building the backbone or bringing down
> cost in a way that enables a business that would not have worked before. For example Netflix … could not have
> been build as business platform without the internet fibre build-out. … I want to understand what businesses could
> become viable thanks to AI because AI brings some kind of overall cost down enough to allow for other services to
> become cheap enough for broader adaption …"* (the project owner, 15 Oct 2026)

**Tests**, applied in order to the enabled business and its customer:

| # | Test | Question |
|---|---|---|
| 1 | **Not DIRECT** | the line below |
| 2 | **New output** | Does something exist that did not pay at the old cost? An existing firm that merely saves money fails. |
| 3 | **Netflix test** | Does the end customer buy that output for a value unrelated to AI? |
| 4 | **Threshold** | Was the enabling cost (or constraint) binding, and has its fall crossed the point where the output pays? |
| 5 | **One step further** | What grows *downstream* of the enabled business? |

**The DIRECT line.** A business is DIRECT and excluded if **any** of these holds. Who runs the AI does not matter (Netflix runs its own content-delivery network).

- **(a) The customer buys AI-generated judgement or content:**
  - advice;
  - a claims or credit decision, even when the customer buys cover or a loan;
  - tuition or AI-authored lessons;
  - a warning.
  - *Rendering or carrying a human-authored work (translating a novel, voicing a book) is not (a).*
- **(b) AI makes an existing operation cheaper or better, with the same output as before:** weeding fields that were already weeded, processing claims already processed, translating listings already translated.
- **(c) The seller is AI-native** (its pitch is the AI). The enabled business, if there is one, is that seller's *customer*, and it must be named.
- **(d) The AI is a sector-specific tool inside the enabled firm's own production:** a weeding robot, a farm-advice app, a claims engine, a sports camera, a protein-design engine, a CAM programmer. **Only a general-purpose cost that falls across industries counts:** translation, speech, general coding, compute, or a by-product such as heat. This is your "overall cost" and Netflix's bandwidth.

> *Note, 16 Nov 2026: 05 governs this DIRECT line. Rule (d) is not an exclusion; 05 §4 sends those chains to the second book, kept and scored.*

**Your four examples fail:**
- farm advice: (a) and (d);
- insurers processing claims: (a), (b) and (d);
- weeding robots: (b), and (d) even where they would enable an organic plot that did not pay before;
- tutoring: (a).

**Channel 2** (AI as the anchor buyer of a physical input, such as geothermal or iron-air) has no AI input. It is judged on tests 2–5.

---

## 1. The answer in eight lines

1. **AI's cheap residue is general capability, not hardware.** The price of a fixed level of AI performance falls ~13× a year (Epoch AI, 22 Sep 2026). Physical inputs are getting *dearer* for everyone else (§5).
2. **The build-out's candidate enablement is narrow: long-form text and speech.** A fixed cost *per title or per language* (shape S1) collapses on a general-purpose service, and the long tail of an existing category gets made. The F rounds measured consumption, and it splits the rows:
   - **C-1 Translated long-form fiction:** EMERGING, PLAUSIBLE (unchanged by F09–F10). *[16 Nov 2026: 05 §5.6 holds that web fiction did not pass; 05 governs.]* At WebNovel consumption follows the titles in share: AI-translated works earned 40% of its novel revenue in H1 2026, against >35% a year earlier (VENDOR filing, unaudited interim). New output is now bounded: the human pipeline (~1,000 titles a year) stopped in 2024, and ~69% of 2024's and ~90% of 2025's AI additions exceed it (CALC, upper bound). But revenue per AI title fell ~70% in 2025 (CALC), no WebNovel revenue line exists, and Storytel's post-edited series read as faster substitution (F10).
   - **C-3 Auto-dubbed creator video:** EMERGING, now WEAK. The >6M daily viewers are real but platform-wide; the long tail's share and any money are not shown.
   - **C-2 Synthetic-narration audiobooks:** HYPOTHESIS, WEAK. AI-narrated titles drew .03% of APA-reporting publishers' 2025 receipts (APA survey, Jun 2026). The self-published Virtual Voice, Spotify and Google tail is probably outside that survey and unmeasured (F11), and publishers report realised AI savings of only 20–50% (Frankfurt Book Fair study, Sep 2026): the crossing rests on the free self-publishing layers.
   - None is STRONG. C-3b catalogue dubbing moves to the watch list (line 4).
3. **A related mechanism (S8) already worked once, before the build-out.** C-0: eBay's 2014 machine-translation upgrade raised US exports to Spanish-speaking Latin America by 10.9%. That was a quality step on a free platform layer, not a fall in fixed cost per title.
4. **Watch list:**
   - C-3b catalogue film and TV dubbing (moved from survivors, F12): rights holders are named and the human cost did bind, but no fee, ad revenue or commercial viewing is shown. The one volume figure (~100M cumulative views on 20 Korean AI-dubbed FAST channels, Dec 2025–Apr 2026, PRESS) comes from a state-funded programme, and the strongest licensee quote from a firm Cineflix took a stake in;
   - C-6 manga: Japanese licensors are now named (VENDOR and PRESS), but no sales are shown; the only volume figure is a tracker estimate of the whole store's Android installs (F13); and a METI localisation subsidy (Jun 2026) is a competing, non-AI explanation;
   - C-7 short-run instruments: the firmware cost has not crossed;
   - C-9 hosts on liquid-cooled waste heat, WEAK and weakened again (F14): AI heat reaches one existing fish farm as a cost saving (Nscale, Glomfjord), and no new-output food host operates. Two dated hosts sit on AI sites: Lévis, Québec (strawberries expected winter 2026–27, not yet shown operating) and Ølgod (pre-FID; financial close targeted Dec 2026; a planning condition ties the data centre to the greenhouse, R4). Neither uses the 45–70 °C liquid-cooling premium. Hima Seafood operates, but on a 2021 cost-saving deal, so it is not an AI effect;
   - leads: indie games, and rights holders' own manga editions (WEAK, F13: no edition is shown to exist because of AI). The archives lead moves to the rule-(d) table (F15).
5. **Excluded by rule (d).** F07 tested what relaxing (d) would add. Only one row:
   - **C-4** unstaffed school and amateur sport streams returns, EMERGING. New sub-varsity streams are now shown at a named school and named districts (school page and trade press, 2018–19), and paid demand is real (LiveBarn revenue "in the $80-million range", PRESS, Jan 2026). But its crossing (free cameras, the staffing constraint) came in 2017–20, before the build-out.
   - **C-5** designed-protein reagents would not reach the watch list: the named buyers (Bio-Techne, Gator Bio) are incumbents improving existing products (rule b).
   - **C-8** one-off machined parts would fail test 4: no series shows one-off prices falling (machine-shop PPI +8.4% nominal, about −2.5% real, Jan 2023–Aug 2026, CALC).
   - **Handwritten archives** (lead, moved here by F15) would not reach the watch list either: every searchable index found is built with handwriting-specific recognition inside its seller's own production, every named use is rule (b), and no new paid work was found after two parcels.
   - The robot-weeded organic plot would be decided the same way.
   - This is your Q1 (§9).
6. **Counter-case: the flooded tail is rationed (LEAD).** Fully AI-generated music reached 44% of Deezer's daily uploads by Apr 2026 and drew ~1–3% of streams, mostly fraudulent and demonetised. AI-narrated audiobooks show the same pattern among reporting publishers (.03% of their 2025 receipts, APA; a different measure; the self-published tail is unmeasured); WebNovel's translations show the opposite in share, though revenue per AI title fell ~70% in 2025 (CALC, F09). No book, audiobook or video platform yet rations AI output the way Deezer does (F01). **Count consumption, not titles.**
7. **The physical channel runs in reverse.** AI bids up DRAM, transformers, fibre, gas turbines and electricians, and the curves it rides were paid for by EVs, shale and car driver-assistance (ADAS).
   - **In trade finance, insurance and compliance the AI routes are DIRECT** (credit, claims and KYC decisions: rules a and d). The record also shows cognition was not the binding cost: banks rank dollar liquidity and counterparty risk first, and KYC first only for just over 15% of banks (ADB, 2025 survey).
   - The cost falls that did happen came from statutes and public rails (TReDS, Aadhaar, SEC Rule 6c-11, EMIR Art. 9(1a)) and, in insurance, from smartphones replacing field visits.
8. **Value goes to whoever distributes the tail:** YouTube, Kindle Direct Publishing, WebNovel. These platforms often supply the AI layer free, and they can withdraw it. Storytel owns 38% of its own post-editing supplier, Nuanxed (VENDOR filing, Mar 2026).
   - **Timing:** in §2 the input crossed its threshold about 1–5 years ahead of the flagship business (fibre → YouTube ~3 years, → Netflix ~5; M-PESA → M-KOPA 4). 2023–26 crossings should therefore show businesses through about 2024–31 (CALC: 2023+1 to 2026+5).
   - Early entrants are visible in long-form translation and absent in trade finance.

---

## 2. What enablement looked like in history (parcel E01)

| Chain | Input: before → after | Crossed | Flagship (date) | Verdict (Grok → Claude) |
|---|---|---|---|---|
| Fibre → streaming | US transit $1,200 → $200 → $25 per Mbps-month (1998 → 2002 → 2007) | ~2002 | Netflix streaming (Jan 2007), YouTube (2005) | PLAUSIBLE → **STRONG** |
| M-PESA → pay-as-you-go solar | person-to-person transfer of ~$20: ~25% (bus fare) → ~2% (30 KSh SMS fee) | 2007 | M-KOPA (2011) | PLAUSIBLE → PLAUSIBLE (**STRONG pending** the fee on a KES 40 paybill instalment) |
| AWS → startup experiments | no up-front servers; EC2 at 10¢/hour (Aug 2006) | 2006 | more, younger startups; accelerators | PLAUSIBLE → **STRONG** |
| Jio → mobile video (India) | Rs 226 → Rs 11.78 per GB (2015 → 2018) | 2016–18 | MX TakaTak, Moj, Josh | PLAUSIBLE → PLAUSIBLE |
| Containers → global sourcing | handling: loading 15.8¢/t vs $5.83/t break-bulk (1956); port costs ~49% of a 1960 door-to-door shipment | 1960s | multi-country supply chains | WEAK → PLAUSIBLE |
| SNP databases → forensic genealogy | consumer genotype files pooled in GEDmatch | 2018 | forensic genealogy (Golden State Killer, Apr 2018) | PLAUSIBLE → PLAUSIBLE, forensic step only |
| GPS accuracy → ride-hailing | the measured gain was Uber's own matching (UberX utilisation +30% by time, +50% by miles), not a fall in a general input | — | Uber | FAILS → **FAILS** |

**Fibre**
- At 1998 transit, a month of Netflix viewing (18 h at 3 Mbps = 24.3 GB) cost **$90 to deliver, 5.0× the $17.99 plan** (CALC). At 2002 prices it was ~$15; at 2007 prices, $1.88.
- Lit fibre averaged ~2.7% utilisation, against a ~15% norm in the 1980s (Merrill Lynch, 2001). A route study at the time disputed a glut on major routes.
- YouTube's bandwidth bill "may be approaching $1 million a month" (2006; PRESS relaying Forbes).
- One step further: the creator economy, not sized in this round.

**M-PESA**
- M-KOPA collects KES 40 a day, against ~KES 50 a day for kerosene.
- The fee M-KOPA's customers paid per KES 40 instalment was **not established**. The threshold is shown on person-to-person transfers, so it is UNCERTAIN on M-KOPA's own unit.
- 10M customers since 2011 (VENDOR, Oct 2026), ~3.4M active at end-2025 (PRESS, LaunchBase, Oct 2026).
- $4.8m net profit in 2025, after a restated 2024 loss of $21.2m. Expected credit losses ran at 38.5% of interest income, so credit binds now (PRESS, same source).

**AWS**
- First VC rounds fell ~20% and initial investments per year nearly doubled (Ewens, Nanda & Rhodes-Kropf, JFE 2018, causal).
- The same paper names accelerators as the next layer.

**Jio**
- 2018 usage at 2015 prices would have cost ~19× the actual bill (CALC). The short-video trio had 553M downloads in 12 months (PRESS).
- UPI is not Jio's child: it launched 5 months earlier.
- "Vernacular content production" is a 2019 forecast quoted by TRAI, not an observed step.

**Containers**
- The cost that fell was **handling**. Ocean rates did not fall.
- The causal trade effect was ~700% over 20 years for **North–North trade**; it was much smaller and faded after 5–10 years elsewhere (Bernhofen et al.).
- Fast fashion is an air-freight story.

**Genomics**
- 23andMe's own customers bought the genotype read-out, the technology's own output. That link fails the Netflix test, as AlexNet does.
- The forensic step passes: genealogists build the trees. 23andMe filed Chapter 11 in Mar 2025.

**GPS**
- Geocaching began on 3 May 2000, about a day after Selective Availability was switched off. It remains the template for a free capability crossing a quality line (S8).

**Controls**
- LEDs → vertical farms: energy alone matches the lettuce price; AeroFarms filed Chapter 11 in 2023.
- Smallsats → index insurance: it ran on **free NOAA rainfall data**.
- Gaming GPUs → AlexNet: fails the Netflix test.
- The anchor-buyer template is better shown by **smartphones → drones**. GPS that cost "tens of thousands of dollars" in the 1990s could be had "for as little as $10" by 2012 (WIRED, Jun 2012, by Chris Anderson, founder of a drone maker).

**Lesson**
- The input crossed its threshold years before the flagship business. Other complements then set the timing: last-mile broadband and licences for Netflix, credit for M-KOPA.
- Where the enabler was physical capacity, it came after a glut or a public price (fibre; Jio). AWS and M-PESA needed no glut.

### The recurring shapes

| # | Shape | Best historic example | AI reading, Oct 2026 |
|---|---|---|---|
| **S1** | **Fixed cost per unit of variety falls → the long tail gets made** | AWS (cost of a first experiment) | build-out: **C-1, C-2, C-3**; watch: C-3b, C-6, C-7; excluded by (d): C-4 (crossed 2017–20), C-5, C-8, archives |
| S2 | Metered price falls until heavy use fits a mass budget | Jio data; US transit | cloud video understanding is ~$26 (CALC: older Flash-Lite tier, input only) to $65–86 per camera-month, against a ~$5 threshold. It is DIRECT anyway (§6) |
| S3 | Fixed cost per transaction falls → small tickets pay | M-PESA | **all fail** (§6): credit, liquidity, regulation |
| S4 | Time or distance collapses → new geographies | containers; air freight | C-0; customs and logistics now bind |
| S5 | The cost of trust falls → strangers trade | M-PESA; SNP databases | **mixed**: deepfakes raise the cost of a trusted check (FinCEN, Nov 2024) |
| S6 | Anchor buyer pays for a learning curve others inherit | smartphones → drone parts | EGS, iron-air: both fail (§6). InP optics: plausible later (§5) |
| S7 | **Crowding: the anchor un-enables others** | — | **the dominant physical reading now** (§5) |
| S8 | A zero-price capability crosses a quality line | GPS → geocaching | C-0 (eBay 2014); YouTube auto-dub and the Kindle Translate beta (C-1, C-3): real, but the platform's, and revocable |
| S9 | By-product sold at disposal value (R5) | naphtha; half-price daytime radio | C-9 waste heat (watch, WEAK); statutes in Germany and France (LEAD), Denmark and Finland, and Ølgod's planning condition, make it partly R4. Where a district network bids, the data centre is paid (~400 SEK/MWh, Stockholm, Feb 2023, CALC). Food hosts take 34–40 °C heat, not the 45–70 °C premium (F14) |
| S10 | Glut residue sold below cost (R1) | 2001 fibre | conditional on a bust; J3 is not firing. **The memory glut fails test 2** (F08): the 2019 and below-cost 2023 DRAM gluts restored existing products (§6) |
| S11 | Statute or public rail that *looks like* a cost fall (R4) | 1868 UK press telegraph rate | a **screen** (L16), not a source of candidates |

---

## 3. Where AI's cheap input actually is

**Model price at fixed capability:** −47% a quarter, ≈13×/yr, on broad benchmarks. Only −27.5% a quarter on SWE-bench Verified (Epoch AI, 22 Sep 2026).

**Posted service prices have not followed:**
- Google machine translation: $20 per million characters in Mar 2014 and again in Oct 2026. That is two endpoints, not a continuous series. Google's LLM tier is priced "cost equivalent with NMT".
- *Newer* Gemini Flash input (3.6/3.8) doubles from $0.75 to $1.50 per M tokens on 1 Jan 2027.
- Gemini 2.5 Flash-Lite stays at $0.10; newer Flash-Lite tiers list at $0.25–0.30.
- Under scarcity, cheap capability arrives through older tiers, open weights and free platform layers.

**Before the build-out:**
- eBay's 2014 machine-translation **upgrade** raised US exports to Spanish-speaking Latin America by **10.9%** (published, Management Science 2019). The 2018 NBER working paper had 17.5% overall and **19.3% for items of $50 or less**.
- That was a quality step on a layer that was already free (S8).

**The build-out's own crossings:** long-form text and speech.

| Production step | Before | After | Fall |
|---|---|---|---|
| Literary translation, 80k-word novel, per language (C-1) | ~£90–100 per 1,000 words (Translators Association guidance via English PEN) → **~£7,200–8,000** | raw machine translation ~$9.60 (CALC); free to authors in the Kindle Translate beta. **Sellable quality = machine translation plus human post-editing**, ~90% below human cost (China Literature, VENDOR) | ~99.9% raw (CALC); **~90% at sellable quality** |
| Audiobook narration per finished hour (C-2) | ~$400 (ACX rule of thumb); ≈$2,600 for a 60k-word book (CALC) | near zero with a free synthetic voice (Virtual Voice; Spotify, up to 5 titles; Google Play). Publishers adopting AI report realised savings of 20% (year 2) and 50% (year 3), against the 85–95% vendors promise (Frankfurt Book Fair/Dosdoce study of 85 experts; PRESS: PublishNews, 9 Sep 2026) | ~two orders of magnitude on the free self-publishing layers; **20–50% for publishers** |
| Dubbing per finished minute per language (C-3) | studio €80–150 (PRESS) | AI draft €3–8, or €8–15 with human QA; API list $0.33–2.20 (VENDOR); $0 to the creator on YouTube | **~80–98% effective**; ~98% at list price |

---

## 4. The enablement map

### Survivors

| ID | Enabled business: its customer buys… | Shape | Status | Verdict (Grok → Claude) | One step further (downstream) |
|---|---|---|---|---|---|
| **C-1** | authors' and web-novelists' foreign editions: **the story** | S1/S8 | EMERGING (revenue share at WebNovel only, VENDOR filing; Storytel strand WEAK, F10) | WEAK → PLAUSIBLE (F01/F02: strengthened on WebNovel only; F09–F10 unchanged, Grok: strengthens) | licensing and adaptation of translated IP (untested; Yuewen's overseas print, manga and screen counts are cumulative and mostly pre-AI, F09) |
| **C-3** | creators' foreign-language audiences: **the programme** | S1/S8 | EMERGING (platform-wide only) | PLAUSIBLE → **WEAK** (F03 settles the E02/E11 contest) | language spin-off channels; local sponsors |
| **C-2** | audio editions of backlist and self-published books: **the book** | S1 | HYPOTHESIS (~0.03% of reporting publishers' receipts; the self-published tail unmeasured, F11) | not assessed → **WEAK** (F01; was PLAUSIBLE; F11 unchanged, Grok: weakens) | not evidenced; plausibly backlist and foreign audio rights |
| *C-0* | *cross-language marketplace sellers: the object* | *S8/S4* | *happened, 2014–17* | *PLAUSIBLE, confirmed causally at the margin* | *parcel consolidators, returns, payments (now closing for US duty-free entry)* |

C-3b (catalogue film and TV dubbing) moved to the watch list in v1.5 (F12).

The input layer these rest on is the platforms' translation and voice services and a post-editing labour market (e.g. Fluent Planet, Nuanxed). That layer is the AI supply side, not an enabled business.
- Among literary translators the post-editing pool is not shown to grow: ~10.6% of CEATL's 2026 respondents were offered post-editing and did not refuse, about the 10% ever asked in 2023 (CALC; self-selected samples). ~30% lost full-translation work (CEATL 2026).
- Fluent Planet post-editing paid 3 euro cents a word, against 10–15 for technical translation (PRESS: ATLF via Livres Hebdo, 16 Dec 2025).

### C-1 Authors' foreign editions

*Note, 16 Nov 2026: 05 §5.6 holds that web fiction did not pass, and a content tail is never the delivered list (05 §7.1(c)). 05 governs.*

**Threshold**
- "Historically less than 5% of titles on Amazon.com available in more than one language" (Amazon). At human prices, fewer than 1 title in 20 paid for itself.
- At sellable quality the cost of translation is now ~90% lower (§3).

**Uptake**
- WebNovel: >7,200 AI-translated works, >70% of its translations (interested parties via Xinhua, Oct 2025).
- AI-translated share of WebNovel's bestseller lists: 21% of the top 100 (Dec 2023, PRESS) → 42% (Nov 2024) → nearly 40% of the top 200 (H1 2025). It has stopped rising (F09).
- Kindle Translate: thousands of authors in six languages by Jun 2026, "millions of pages" read (VENDOR, page updated 30 Jun 2026). Engagement, not revenue.

**Consumption (F01, F02, F09): the first revenue shares, issuer narrative only**
- FY2025: >17,000 AI-translated works; their revenue +39% y/y and more than one-third of WebNovel's *total* revenues (China Literature annual results, 17 Mar 2026, VENDOR filing).
- H1 2026: >30,000 works, contributing 40% of WebNovel's *novel* revenue (interim, unaudited, auditor-reviewed, 11 Aug 2026, VENDOR filing). The bases differ, so one-third → 40% is not a series, and the RMB amount is undisclosed. The two same-base pairs both rise: platform revenue >30% (FY2024) → >1/3 (FY2025); novel revenue >35% (H1 2025) → 40% (H1 2026) (F09).
- **Revenue per AI-translated title is falling** (F09). On one base it can be computed: AI-translated revenue rose 39% in 2025 while the AI stock grew ~4.5× (~3,800 → >17,000), so revenue per title fell ~70% (CALC). The marginal titles earn little.
- Counts may include language versions from H2 2025: >17,000 AI works (end-2025 filing) against >13,600 translations of all kinds (Dec 2025 report) (UNCERTAIN, F09).
- The opposite of Deezer (44% of uploads, 1–3% of streams): at WebNovel consumption follows the titles in share, though not per title.
- **Less-commonly spoken languages:** revenue +160% y/y in H1 2026, an increase AI "facilitated" (same filing). Not a clean new-output signal (F09): it covers all works in those languages, including human translations and local-language originals; the Chinese release names Yuewen, not WebNovel, as the base; no RMB base or language split exists. It does not continue 2024's +350%, which counted AI-translated non-English works only.

**Scale and new output (F09)**
- **No WebNovel revenue is disclosed** for FY2024, FY2025 or H1 2026. It sits inside "online business on self-owned platforms", which fell 7.0% to RMB 1,623.4m in H1 2026 (interim, 11 Aug 2026): a mostly domestic line, not a proxy.
- **The only third-party scale is flat:** WebNovel's US app-store consumer spend was ~$245–321K a week in Q2 2023 and ~$260–350K in Q3 2024, ~$13–18M a year across the start of AI translation in English (Sensor Tower estimates; gross spend, app stores only; CALC).
- **The human pipeline ran at ~1,000 titles a year and stopped in 2024:** ~1,700 translations (Oct 2021) → ~2,900 (end-2022; PRESS: Xinmin via chinawriter, 13 Mar 2023) → ~3,600 (Oct 2023) → ~3,800 (end-2023). In 2024 net additions (~3,000) roughly equalled AI additions (~3,200), so ~1,000 titles a year are substitution (rule b).
- **New output, upper bound:** ~69% of 2024's and ~90% of 2025's AI additions exceed the old human capacity (CALC; counts may include language versions).
- **Test 4 has a non-issuer statement:** translator scarcity pushed WebNovel from training translators to cultivating native-language authors (a Peking University professor in Guangming Daily, via chinawriter, 6 Dec 2025, PRESS); originals were ~100× translations by end-2024 (same page).
- **The enabled party is invisible:** no figure exists for Chinese authors' overseas earnings. The one documented author who used ChatGPT to serialise abroad kept only her WebNovel serial and refocused on China after two months (PRESS: Red Star Capital via The Paper, 27 Jan 2024; n=1).

**New output vs substitution (LEAD)**
- *New output.* Veen Bosch & Keuning announced in Nov 2024 a plan to AI-translate fewer than 10 commercial-fiction titles whose English rights were unsold: "we don't foresee the opportunity to sell" them (Publishers Weekly). **Still no outcome as of 15 Oct 2026** (F02); the last dated status is about ten books in progress with author consent (Trouw, 7 Apr 2025). Weak negative evidence, not a finding of failure.
- *Substitution (rule b).* HarperCollins France is testing machine translation with post-editing on Harlequin titles it already translates, to hold a €4.99 price (PW, Jan 2026). Harlequin France has since partnered with Fluent Planet and "terminated a number of translators' contracts" (PW, 11 Sep 2026).
- *Substitution on present evidence: Storytel (F10, WEAK; was undetermined).* Storytel "automated its translation publishing workflow" with Nuanxed and names time, not money, as the constraint (PW, 8 Oct 2026); in Mar 2025 it cited money and time (Yle).
  - **Selection is the head, not the tail:** "If something really thrives, those are the markets we target first" (same PW interview).
  - **The named Nuanxed titles continue a pre-AI operation:** Lind & Co (70% Storytel-owned since 2021) already published in NL, PL, FI and NO in 2018–19 (Storytel release, 18 Mar 2021).
  - **Interested party:** Storytel owns 38% of Nuanxed (associate; AR 2025, Note 23, VENDOR filing, 26 Mar 2026); the PW speaker sits on Nuanxed's board, and Nuanxed's CEO is a former Storytel regional manager (PW, 19 Nov 2024).
  - **The only quantity points the wrong way for scale:** Storytel's purchases of translation services from Nuanxed fell from TSEK 17,045 (2024) to 9,609 (2025), −44% (same note; CALC).
  - No count, listening share or margin effect for translated titles appears in AR 2025 or the Q1 (28 Apr) and Q2 (28 Jul 2026) reports.
- *Open (LEAD, F10): Gummerus's digital-only backlist series.* Gummerus (Storytel group) publishes Nuanxed post-edited genre series in audio and e-book only: Lucy Score's eight-part Blue Moon, EN→FI, a volume a month ("we do not save euros but time"; PRESS: Suomen Kuvalehti, 11 Apr 2024), and Julia Chapman's Dales Detective (Yle, 20 May 2025). Yle reports these are older backlist, not new releases, and Gummerus calls Blue Moon an addition to its list (publisher claim). Against: Gummerus human-translated two other Score novels in the same season. No listening or revenue figure. Check its JUJU genre imprint (Mar 2026) in Storytel's Q3 report (27 Oct 2026).
- No publisher title list separating new from substituted translations was found (F02); none exists at Storytel, BookBeat or Nextory either (F10).
- **Author consent** is a scarce complement for trade backlist (Authors Guild model clauses, Apr 2026). The real tail is self-published and rights-reverted titles. No service built on reverted rights plus AI translation was found; a reverted author can go straight to Kindle Translate, where no data is published (F02).

**Against**
- Volume and revenue-share data come from interested parties; there is no independent revenue per title.
- Overseas web-fiction revenue was CNY 5.07bn in 2024, up >25% but slowing from ~40%, while AI titles multiplied. In 2025 it was CNY 5.64bn, +11.2% (PRESS: CASS via China Daily, 14 Apr 2026), while exported works rose from ~40,000 to >130,000 (PRESS, Aug 2026; definitions may differ). The 2024 base conflicts with the trade association's RMB 4.815bn (F09). Titles are outrunning revenue, so part of WebNovel's 40% is likely redistribution (rule b).
- China Literature's online-business revenue was flat in 2025: CNY 4,047.0m against 4,030.6m (+0.4%). Group revenue fell to RMB 7,366.2m from 8,121.1m (audited annual results, 17 Mar 2026); in H1 2026 the self-owned-platform line, which holds WebNovel, fell 7.0% (F09).
- Revenue per AI-translated title fell ~70% in 2025 (CALC, above), and AI's share of the bestseller lists has stopped rising at ~40%.
- At WMT24, humans were still in the winning cluster for 7 of 11 language pairs.
- The flooded-tail risk (below).

### C-3 Creators' foreign-language audiences

**Uptake**
- >6M daily viewers watch over 10 minutes of auto-dubbed content (Dec 2025 data; 27 languages; YouTube blog, 4 Feb 2026, VENDOR). Floor: ≥60M minutes a day (CALC). It covers all channel sizes and counts viewers, not revenue.
- Dubbed views hold ~75% of the original view duration: a platform average (PRESS relaying YouTube, Feb and May 2026).
- Through 2025 auto-dubs played by default, with no global switch for viewers (PRESS: heise, Mar 2025; MediaNama, Sep 2025), so part of the Dec 2025 count is default exposure. A preferred-language setting now exists (help page, undated).
- "Millions of channels" use auto dubbing (VENDOR, May 2026), but the feature is "enabled by default for eligible creators": enrolment, not demand.

**The long tail (F03)**
- The only measured channel under 100k subscribers (8,800+) got 0.2% of its watch time from its English auto-dub over 28 days (6 Sep–3 Oct 2026), at ~26% of the original's view duration (CALC: 1:12 vs 4:38). n=1; VENDOR (the operator runs an AI-tool affiliate site).
- For most non-English originals, auto-dub produces **English only** (YouTube help page, fetched 15 Oct 2026). The 27-language reach applies to English-language creators.
- No RPM for dubbed tracks exists from any source, and YouTube makes no monetisation or RPM-parity statement.
- Distribution binds on the audio-track route: one creator's AI dub drew 32 views in 90 days as a track on the main channel, against 3,897 on a dedicated Spanish channel (~122×, CALC; VENDOR, n=1, a 162k-subscriber main channel). New output shows in language spin-off channels, not in tracks.
- **Lead (F12): Goalcast's French spin-off channel.** "Showdown en Français", dubbed with Adapt and Dubformer, "generated 9 million views and 100,000 subscribers within its first weekend of launch" and crossed Facebook monetisation thresholds, with no sum given (VENDOR, 20 Apr 2026; views platform-counted; whether Goalcast already had French output is not stated). A digital publisher's own catalogue, not a licensed film library.

**Against (the E02/E11 contest is settled toward WEAK, F03)**
- The ">25% of watch time from non-primary languages" figure applies to pilot creators who **uploaded their own dubs** (MrBeast, Mark Rober), not to auto-dub.
- The dub is labelled and audible.
- The flooded-tail risk applies.
- Consumption is real platform-wide; the paying side is not shown for any channel size.

**C-3b Catalogue film and TV (sub-row, HYPOTHESIS; on the watch list since v1.5, F12)**
- Prime Video began AI-aided dubbing on 12 licensed titles "that would not have been dubbed otherwise" (Mar 2025, VENDOR). That means no dub *on Prime Video*; no viewing result was published.
- In late Nov 2025 it added "AI beta" dubs to five anime. By 4 Dec 2025 it had removed the English tracks on all four titles that had them, and the Latin American Spanish tracks on three of the five (Banana Fish, No Game No Life Zero, Vinland Saga); removal on the other two is unreported (PRESS: Anime News Network, which Kadokawa majority-owns). No Game No Life Zero already had a human English dub (2017), so that track was rule (b). Kadokawa said it had not approved an AI dub in any form, and HIDIVE, the English-dub licensee, was not told in advance (PRESS: ANN, 3 Dec 2025). ANN reports the objections and the removals without linking them causally. Licensor consent binds here, as author consent does for C-1.
- **Named enabled parties (F03):**
  - Love TV Channels licensed Cineflix Rights factual series "never dubbed into Spanish, Italian, or French" for European FAST channels (Love TV's CEO in Deepdub's joint release, 23 Feb 2026, VENDOR). The >80% cost cut is Deepdub's benchmark; the 25M monthly viewers are Love TV's whole audience ("viewers" in that release, "households" in Cineflix's). **Not arm's-length (F12):** Cineflix commits 500 hours in French, Italian and Spanish "in return for a stake in the business" (Cineflix release, 10 Feb 2026, which does not mention AI), so no cash licence fee is implied.
  - Seven.One Studios International says dubbing cost "has traditionally held back" foreign-language distribution and "this is changing"; it sold German TV films and series to DubMe IO to AI-dub into 30 languages on YouTube (company release, 9 Jun 2026; PRESS: Señal News, 10 Jun 2026). Forward-looking (DubMe IO "will turn" the package into 30-language assets); DubMe IO is both the AI supplier and the licensee; the other buyers of the 500+ hours are not described as using AI (F12).
  - Cineflix Rights put >100 of Mayday's 240 hours into neutral Spanish with Papercup and landed one linear licence, fee undisclosed (PRESS: C21, 12 Mar 2025); it now runs its own Spanish channel. Spanish novelty is not shown: the series already circulated in Spanish as "Mayday: catástrofes aéreas". Its digital distribution revenue grew "double-digit", with no AI split (Cineflix release, 10 Feb 2026).
  - Korea's state K-FAST programme: 20 AI-dubbed channels on Samsung TV Plus and LG Channels, ~1,200 titles in English, Spanish and Portuguese, ~100M cumulative views in 22 countries, Dec 2025–Apr 2026 (PRESS: Seoul Economic Daily relaying the science ministry, 9 Jul 2026). Cumulative views, not people (~1M per channel-month, CALC); funded at 230M won per channel in 2026 (L16); 2025 rights holders unnamed; no ad revenue. The 2026 round names one: CJ ENM (K-DANCE, with Hudson AI).
- No licence fee or ad revenue exists for any catalogue AI-dub deal; the only viewing figure is the state programme's (F12). Cineflix's MIPCOM release (14 Oct 2026) lists only conventional sales.
- **France (CNC/Audiens note, Oct 2025; interview-based):** AVOD services carry only catalogue that was already dubbed, so the human cost did bind; but distributors that tested synthetic voices quickly backed away, no synthetic-voice case was reported for French TV or film, and AI dubbing appeared only at the margin (YouTube catalogue channels, documentary voice-over).
- Union rules mostly do not bind on catalogue: SAG-AFTRA's consent rule for dubbing with a digital replica applies only to pictures starting principal photography from 1 Jul 2027 (contract excerpt dated 11 May 2026), and a generic synthetic voice is not a performer's replica.
- Excluded: Prime Video's AI lip-sync of human dubs on Maxton Hall (Sep 2026) is rule (b) and (d).
- Reading: this works for low-attention factual catalogue and meets resistance where fans are engaged. **Moved to the watch list (F12):** like C-6, the licensors are named and the human cost did bind, but the output is not shown to pay (test 4), and the one volume figure carries a subsidy confound. C-2 and C-3 stay survivors because their enabled parties pay ~nothing on free layers, so any sale pays; C-3b's per-minute cost is positive (€3–15, §3).

### C-2 Audio editions of books that never had one

**Threshold.** About **1M audiobooks against >40M e-books** (PRESS: PPC Land, Oct 2026, relaying Spotify, Sep 2026). The blocked market is measured in titles.

**Evidence so far.** Amazon's Virtual Voice had made >40,000 Audible titles by May 2024 (PRESS: Publishers Lunch citing Bloomberg, 6 May 2024) and >50,000 labelled "Narrated By: Virtual Voice" by May 2025 (PRESS: TechCrunch, 13 May 2025). No newer count exists, and Apple, Spotify and Google publish none (F11, 15 Oct 2026). Sales per title are unknown, so the status is **HYPOTHESIS**.

**Consumption (F01, F11): tiny among reporting publishers, so the verdict falls to WEAK; the self-published tail is unmeasured**
- "AI sales revenue amounted to .03% in 2025" (APA Sales Survey, 5 Jun 2026). The base is **publisher receipts**: "Publisher receipts in 2025 totaled 2.43 billion dollars" (APA research page), so .03% ≈ $0.73m of reporting publishers' receipts (CALC), not a share of the US market. The last published method (2023 sales; SSRS, 6 Jun 2024) surveyed APA member publishers: 27 respondents, Audible, Inc. among them. Self-published Virtual Voice, Spotify and Google sales count only if a reporting member includes them; that is not established (F11).
- The same release says consumption of AI-narrated titles rose in 2025, while willingness to try fell from 70% to 61%. 16% of listeners have ever heard one (a headcount).
- Audible: >50M minutes of "AI generated content" listened to, period not given (PRESS: The Bookseller, 2 Jun 2026). Against Audible's >5bn hours of listening in 2024 (VENDOR), that is ≤~0.02% of a year, if the minutes span at least a year (CALC). The minutes cover all of Audible's AI output, including the AI production and translation service it sells publishers (launched May 2025), not Virtual Voice alone (VENDOR: Audible's Lee Jarit in PW, 1 Jun 2026). Spread over ≥50,000 Virtual Voice titles they would be ≤~1,000 minutes (~17 h) per title (CALC, upper bound). The same executive says AI narration is "opening up a whole catalog of content that previously had no audio life at all" (VENDOR, no figure).
- Spotify: audiobook hours +60% y/y with no digital-voice split (VENDOR, 21 May 2026). Its ElevenLabs-powered creation tools opened as an invite-only beta in Jun 2026 and to US self-published authors on 9 Sep 2026: English only, up to 5 projects per account, labelled "Narrated by Digital Voice". No author, title, hour or revenue figure exists (F11, 15 Oct 2026).
- Author surveys (Written Word Media 2025, n=1,346; ALLi; Kindlepreneur) report no synthetic-narration earnings (F11).
- Reading: on the free self-publishing layers the cost has crossed (any sale pays) and the enabled party (KDP authors) is visible; uptake is missing, and the one survey that measures it probably leaves them out. It stays a survivor, not watch (F11; Grok: weakens).

**Against**
- Titles are labelled, and listeners have asked for a filter to hide them.
- Author consent binds.
- **The flooded-tail counter-case applies most here.**
- **Publishers save far less than two orders of magnitude:** 20% in the second year of AI adoption and 50% in the third, against the 85–95% vendors promise (Frankfurt Book Fair/Dosdoce, 85 experts; PRESS: PublishNews, 9 Sep 2026). Half the barriers to wider use come from agents, publishers and authors (same study).
- **Listeners choose narrators:** 65% sought a narrator they liked (NielsenIQ survey commissioned by Audible, relayed by ALLi, 13 Oct 2026).
- **The free layer predates the build-out:** Google Play auto-narration was open to publishers in six countries by Apr 2022, free for a limited time, with a 52% revenue share (PRESS: PW, 26 Apr 2022), and "thousands of publishers" had used it by Nov 2022 (VENDOR). No market was ever measured, so C-2 is not HISTORIC. Mass uptake followed Amazon's own Virtual Voice, while ACX still requires human narration "unless otherwise authorized" (ACX page, 15 Apr 2026). Platform access, not the build-out's cost fall, may be what bound (L17; open).

### C-0 Cross-language marketplace selling: already happened (2014–17)

**What the evidence measures.**
- eBay's 2014 upgrade raised US exports to Spanish-speaking Latin America by 10.9%, a quality step on a free machine-translation layer (S8).
- For scale, a 100-word listing costs ~$21 to translate by hand, about 84% of a $25 order, against ~$0.012 by machine (CALC, illustrative sizes).
- Vestiaire Collective's 82% cut in description-translation cost (VENDOR) is substitution, rule (b). It is not evidence of new output.

**Since 2024: no new step.**
- Etsy's non-US share of gross merchandise sales was 26% in both 2024 and 2025.
- Customs now binds. US de minimis ended on 29 Aug 2025, and a $23.19 benchmark broker fee is 93% of a $25 order.

### Counter-case: the flooded tail (LEAD)

**Music is the 2025–26 control for S1.**
- Fully AI-generated tracks were 28% of Deezer's deliveries with ~0.5% of streams (Sep 2025).
- By Apr 2026 they were 44% of daily uploads with "about 1 to 3 percent" of total streams, mostly fraudulent and excluded from royalties (PRESS relaying Deezer).
- Spotify removed "over 75 million spammy tracks" in the 12 months to Sep 2025 (VENDOR).
- The Authors Guild now sells a "Human Authored" mark against "the glut of AI-generated books" (Mar 2026).

**Reading.** Music platforms answer a cost collapse by rationing attention. No such throttling is evidenced yet at YouTube, KDP, WebNovel, Audible or Spotify (F01, Oct 2026). They use disclosure, labels and distribution limits: KDP caps new titles at 2 per format a week (not framed as an AI rule); Spotify keeps digital-voice audiobooks from referral partners. The nearest analogue is YouTube's general rule, renamed "inauthentic content" on 15 Jul 2025, that mass-produced content cannot be monetised; it does not mention AI. **Count listening and reading, not titles.** Measured so far: audiobooks among reporting publishers follow the music pattern (.03%; the self-published tail is unmeasured); WebNovel's translations do not in share (40%), though revenue per title is falling (~−70% in 2025, CALC).

**Downstream.** Provenance and curation: certification marks, AI tags, human-narration labels.

### Watch list: passes the line, but not crossed, not yet shown to pay at a positive cost, or the enabled party not yet visible

| ID | Row | Why it is on watch |
|---|---|---|
| **C-3b** | Catalogue film and TV dubbing into new languages (sub-row of C-3; moved from survivors, F12) | Rights holders are named (Cineflix Rights, Seven.One Studios International; CJ ENM in Korea's 2026 programme), and the human cost did bind (Seven.One; CNC, Oct 2025: AVOD carries only catalogue already dubbed). **Test 4 is unshown**: no fee, ad revenue or commercial viewing. The only volume figure (~100M cumulative views, 20 Korean K-FAST channels, Dec 2025–Apr 2026, PRESS) comes from a state-funded programme (L16), and the strongest licensee quote (Love TV) from a firm Cineflix took a stake in. Same evidence position as C-6. Details in the C-3 block. |
| **C-6** | Mid-list manga reaching US readers (Orange Inc., emaqi) | The localiser is AI-native and sells to readers itself, so under rule (c) the enabled party is a **Japanese licensor**. **Licensors are now named** (F04): Shonengahosha, Futabasha, Akita and Nihon Bungeisha (VENDOR and PRESS, 2024–26), and Shinchosha and Houbunsha, whose Oct 2026 titles are "being released in English for the first time" (PRESS relaying emaqi, 6 Oct 2026): up to 11 titles, since the claim covers only three publishers' titles, none checked against a bibliography (F13). COAMIX also licenses to emaqi (PRESS: ANN, 3 Sep 2026). It stays on watch because **test 4 is unshown**: no sales, subscriber or MAU figure; the company declined, citing only "steady growth in monthly active users" (PW, 1 Jul 2026). The only volume proxy is a tracker estimate: 388K+ cumulative Google Play installs since Apr 2025, +8.2K in the last 30 days, down 8% (AppDashboard, fetched 15 Oct 2026). It covers the whole store, which mostly resells publisher-supplied English editions ("our role there is simply retail", CEO, VENDOR, Aug 2025), so it does not measure demand for first-English titles (F13). ~100 exclusives sit inside a 400+-title subscription (ANN, 5 Jul 2026, company email); the store has ~2,500 series (PW, Jun 2026). v1.4's ~4% mixed the two bases and is withdrawn; exclusive ≠ first-English. emaqi "uses AI-assisted programs to translate, letter, and produce its manga exclusives" (PW). Confounds: METI's menu-8 subsidy (½ of localisation cost, ≤¥40m a company, to Feb 2027) funds rights holders' own localisation, and no row names AI (official results, 25 Jun 2026: 20 adopted of 86 applications; manga rows Bushiroad Works, Bunkasha, Comisma, Amazia, Poplar, JadeComiX; round 3 results late Nov 2026); Shueisha's free Manga Million brought ~300 first-time translations, all by professional translators (Shueisha guide, updated 7 Aug 2026; AI offered and declined, PRESS: Forbes Japan, 31 Aug 2026). No US publisher says it uses AI for titles it would not otherwise publish (Media Do, Seven Seas' owner: "absolutely no plans"; PRESS: ANN, Mar 2026). Orange says ~2% of Japanese manga has an official English edition, **by volume**, and claims one-tenth of the human time (VENDOR). |
| **C-7** | Short-run instruments, via cheap firmware (general-purpose coding) | Firmware is 29.2% of engineering cost, ≈$1,620 per unit at a batch of 100 (CALC; Apr 2024 survey). It must fall 5–10×; measured hours fall ~21%. AI also raises memory costs: the Raspberry Pi 5 16GB went from $120 to $205. |
| **C-9** | Hosts on liquid-cooled waste heat: **a winter vegetable or a farmed fish** (a pool only if it opens or stays open because of the heat) | **WEAK (F05), weakened again (F14): no new-output food host runs on AI data-centre heat** as of 15 Oct 2026. One existing fish farm takes ~34 °C cooling water from Nscale's Glomfjord AI site as a cost saving (VENDOR, Nov 2025; §6). Free heat at 45–70 °C would shrink the heat pump (R5), but no host uses that premium: Ølgod's plan lifts data-centre heat to >40 °C with heat pumps, Nscale supplies ~34 °C, Deep Green markets 30–40 °C (F14). **Two dated new-output hosts on AI sites.** (1) **Lévis, Québec:** Innoserres / Les Fraises de l'Île d'Orléans, 12 ha of greenhouses next to QScale's "centre de traitement de données d'IA", expected to supply strawberries "l'hiver prochain", i.e. winter 2026–27 (a Québec environment-ministry officer in Vecteur Environnement, Mar 2026). Not shown operating: Québec's electricity aid (40% of the bill, up to 10 M$) is paid only once it operates (PRESS: La Presse, 9 Feb 2026); heat capture rests on a 40 M$ provincial grant, and QScale gives its heat free at the gate (PRESS, Mar 2023): partly R4. (2) **Ølgod**, Danish winter vegetables with atNorth (DEN02, marketed for AI and HPC; it "will accommodate" direct liquid cooling, no share stated, VENDOR) and Selected Group. Local plan approved 6 Oct 2026 (company-reported); heat, land and grid agreements secured; still **pre-FID**: financial close targeted Dec 2026, first growing season Q3 2028 (developer targets, VENDOR, 14 Oct 2026); Varde municipality expects the whole project built in 2030. The plan sizes the greenhouses at 4 × 10 ha, and the minister's zoning exception (26 Jan 2026) lets the data centre be built only once the greenhouse exists or alongside it (Varde local-plan proposal, Apr 2026): heat-led siting imposed by planning (R4). Selected Group already runs the model on paper-mill heat at Frövi (tomatoes in stores since Aug 2024, VENDOR), so AI adds heat sites; it does not enable the model. **Hima Seafood leaves C-9** (§6): its heat deal dates from 28 Jun 2021 and was framed as "a significant cost saving" (PRESS). Existing pools that save money fail test 2: Trafford saves ~£80k/yr (VENDOR). District heat fails test 2: Fortum/Microsoft, 2027 onwards. **Uithoorn is substitution:** existing gas-heated growers switch, keep CHP and boilers for backup, and take water under 30 °C from a dry-cooled site, lifted to 70 °C, with an SDE++ subsidy (PRESS, 23 Jul 2026). **Heat is not free where a district network bids:** the data centre is paid, ~400 SEK/MWh in Stockholm (≈€35–37, CALC; sheet dated 15 Feb 2023). No price to a food host is published (F14: Green Mountain and QScale give heat free at the gate; Nscale and Ølgod state no price). **Lead:** Salfjord, a salmon company that wants to build a data centre as a heater for its fish, first farm phase 2028 (PRESS: TU, 15 Apr 2026; paywalled, headline and caption only; AI load unknown). **Statute screen:** under Germany's EnEfG §11(2) (LEAD), data centres starting from 1 Jul 2026 must reach ≥10% reused energy within two years of commissioning, with planned shares of ≥15% from 1 Jul 2027 and ≥20% from 1 Jul 2028. §11(3) no. 3 exempts an operator whose at-cost heat offer a nearby network does not accept within six months. France has had an obligation since 1 Oct 2025 (LEAD). Denmark (Order 1167, from 11 Oct 2025) and Finland (Act 1382/2025, from 1 Jan 2026) impose a reuse duty above 1 MW with a cost-benefit escape (Denmark exempts heat already used in district heating); the Netherlands only requires reporting so far (bill 36868 in the Senate). German, French, Danish and Finnish cases, Ølgod included, are therefore partly R4. |
| lead | Indie-game localisation: a partial crossing | Machine translation plus post-editing cuts cost 40–50% on text-moderate games, but "roughly zero on the narrative layer" (Alconost, Jul 2026, VENDOR). Simplified Chinese passed English on Steam in 2024 (33.7% vs 33.5%). |
| lead | Japanese rights holders' own English or cross-border manga editions (F04; **WEAK**, F13) | The non-AI-native route C-6 needs. **No rights holder shows an edition that exists because of AI, and none reports sales** (F13). **Bushiroad Works** is funded by METI (25 Jun 2026) to expand English titles on its Comic Growl service to 50+; the ministry's own row names no AI and gives anti-piracy and monetisation as the aims (METI results page, 25 Jun 2026); the English shelf held 28 series on 15 Oct 2026, the complete count. Mantra is named only for Ancient Magus' Bride, which already had an English edition (rule b), and Ghost and Witch (Dec 2023). Ghost and Witch's Mantra simulpub was its first official English, but Seven Seas licensed it on 7 May 2025 for print in Feb 2026 (VENDOR): AI changed when English appeared, not whether. Bushiroad's stated reason was piracy (PRESS, Dec 2023). **Square Enix** said cost still leaves languages untranslated (26 Jun 2024), but as an investor quoted in Mantra's own funding release (VENDOR, interested party), naming no title. **Shueisha** uses Mantra for part of MANGA Plus (VENDOR, Jun 2024), and its METI menu-5 row targets rapid multilingual release of untranslated works, naming no AI: this reopens v1.4's dropped "Shueisha via Mantra" as an open question. **BOOK☆WALKER** has offered ~340 eligible doujinshi titles across the Japan–Taiwan border with Mantra's on-screen translation since 15 May 2026, citing "the high cost of translation" as the creators' hurdle (VENDOR, 14 May 2026). **TO Books' Corona EX**, a rights holder using Google Translate (a general-purpose cost, the cleanest §0 fit), machine-translated one of four launch titles in Apr 2024, to quality complaints; its English subdomain did not resolve on 15 Oct 2026. No sales for any. **Rule (d):** Dwango calls Mantra a manga-only ("マンガ専用") system, so the Mantra routes inside rights holders' own production (Bushiroad Works, MANGA Plus) are excluded; BOOK☆WALKER's viewer overlay is too if (d)'s general-purpose clause covers a third party's layer (§9 Q1). The lead rests on general-purpose routes: TO Books' Google Translate, LLM localisation. METI's menu 5 (not menu 8) envisages AI-assisted localisation ("AIも活用したローカライズ"), so a later award may name it. |

### Excluded by rule (d), with possible new output: what changes if you relax (d)

| ID | Row | New output | Why (d) excludes it | Evidence |
|---|---|---|---|---|
| **C-4** | Streams of school, club and venue games nobody filmed | **yes, at a named school and named districts** (F07): Pierre SD: "Now, middle school games, and junior varsity and sophomore teams are broadcast" (PRESS: District Administration, Feb 2019); Bishop Lynch HS added JV, sophomore and freshman streams to select varsity (school page, Sep 2018). Also one partner's schools going 20 → 100+ live events per season (VENDOR). No 2024–26 national share of sub-varsity or practice streams exists. | The sports camera is a sector-specific tool in the stream's own production, like a weeding robot. The crossing came in **2017–20, before the build-out**: Pixellot cameras became free to users by 2020, with nearly 10,000 US installations (PRESS: SBJ, Apr 2026). Staffing bound: Novi and Cheyenne could not find enough students. The cost per event did fall at high use: Pierre paid a ~$3,500 flat annual fee for ~400 games, ~$9 a game, hardware excluded (CALC, 2019). The earlier "no cost fall" against the $90 district-staff videographer rested on Pixellot's 2020 quote of $40–100 a game (VENDOR). | Pixellot ~1.5M games in 2025, Hudl >1M (doubled in two years), ~600,000 Pixellot games via the NFHS Network (PRESS: SBJ's own tally, 20 Apr 2026; games, not viewers). Hudl "1M+ games … a majority captured automatically" (VENDOR). LiveBarn revenue "exceeded $50-million in 2023" and is "now in the $80-million range" (PRESS: Globe and Mail, Jan 2026, citing Deloitte; currency unmarked); sold to GTCR for US$400M-plus (PRESS, Apr 2026). It has >4,000 surfaces in ~2,270 venues (PRESS, Jan 2026) and removes the operator mostly with a fixed panoramic rig, so AI's share there is partial. NFHS Network/PlayOn, LiveBarn and Hudl disclose no subscribers or sub-varsity share. Much of the volume is **substitution**: ECNL games were filmed by travelling team cameras before; NFHS varsity streams ran on student crews from 2013; Pierre uploaded stationary-camera video to YouTube before. The scarce complements are playoff media rights and exclusive venue rights. SBJ's "$10 billion" headline is TeamSnap's CEO, an interested party: not used. |
| **C-5** | Reagents from designed proteins, for small test makers | for targets with no usable antibody; **none shown** | Protein design is a sector-specific engine, and the seller (Monod Bio, via Fisher) is AI-native. **The named buyers are incumbents improving existing products** (rule b, F07): Bio-Techne licensed NovoBody Duo molecules "to Expand Recombinant Protein Portfolio" (18 Nov 2025, VENDOR; >$1.2bn FY2025 net sales); Gator Bio's HIS XT probes (launched 18 Feb 2026, VENDOR) replace its antibody-based His probes. The only point-of-care test is Monod's own (preeclampsia; $750,000 Gates Foundation Grand Challenges grant, Oct 2025: rule c). No veterinary, food-safety, environmental or point-of-care test maker is named. Relaxing (d) would not move it to watch. | Designs per campaign fell from >10,000 to ~10, about three orders of magnitude. There is no all-in invoice, and the $450-per-96-test kit is ordinary ELISA pricing. No volumes or revenue are disclosed. |
| **C-8** | One-off machined parts for low-volume hardware | only for variants that did not pay before; none named | AI CAM is a sector-specific tool. For variants already made, it is rule (b). **Relaxing (d) would not help: it fails test 4 on present evidence** (F07). | Programming time fell from 45–60 to 5–10 min per part variant (VENDOR, one case), but no observed price shows it. BLS machine-shop PPI 197.858 (Jan 2023) → 214.450 (Aug 2026), +8.4% nominal, about −2.5% real against CPI-U (CALC; FRED, updated 10 Sep 2026); it covers all machine-shop output. Protolabs revenue per customer contact $9,425 (2023) → $9,716 (2024), a mix measure (VENDOR filing, Feb 2025). A private 3-part repeat-quote basket rose ~8% at Xometry US in 4Q24, confounded by a faster delivery tier (Industrial Analyst, Jan 2025; series ends 2024). No series measures a one-off part price, and no hardware maker credits cheaper one-offs. |
| lead | Handwritten archives → searchable records (moved from the watch list, F15) | heir searches on small estates, house and local histories, deed services: **none shown after two parcels** (F06, F15) | Every searchable index found is built with handwriting-specific recognition inside its seller's own production: ARCHION runs a Transkribus model "auf historische Handschriften ausgerichtet" (VENDOR, undated page); ArkivDigital runs Riksarkivet's HTRflow, "anpassad för svenska dokument från perioden 1650–1900", and Swedish Lion (Riksarkivet annual report 2025, Feb 2026); Ancestry's recognition is proprietary (since 2021). Each adds to an existing product (rule b): ARCHION's €4.90 top-up for 25 pages (~€0.20 a page, CALC) is sold only with an existing church-book pass; ArkivDigital adds search to images it already sells by subscription (8.7M images, ~15,000 volumes by 14 Aug 2026, VENDOR); Riksarkivet indexed ~17M property files (1971–2008) to speed its own case handling. A downstream firm using such an index faces a sector-specific cost too. **Relaxing (d) would not move it to watch** (like C-5): test 2 is unshown and every named use is rule (b). | The input crossed: FamilySearch ~2.3B AI-transcribed images by 2026 (PRESS, Mar 2026); list-price cost per page fell ~23–46× (Transkribus) to ~625–3,160× (general vision models) against commercial transcription (CALC on 2024 prices, review excluded). The one professional firm found does existing work faster (Legacy Tree, VENDOR, Apr 2026: rule b). Consumption does not follow: Riksarkivet put ~3M AI-transcribed pages online, and visits to its search service fell from 3.8M to 3.1M in 2025 (−18.4%, CALC; partly outages; annual report). Finland's +24% research-database growth comes from the Karelia and Soviet-fate databases, not the content-search demo (opened Oct 2025). The heir floor did not bind: probate researchers "regularly investigate small estates … (often under £10,000)" on no-win-no-fee terms (Finders International, VENDOR; published May 2024, modified Apr 2026). Ancestry credits its Italy launch and about half a dozen more countries partly to AI translation of its site and partly to its own handwriting recognition; neither is isolated and no market is quantified (PRESS: Semafor, Apr 2026; Business Insider, Jun 2026). No archive or professional body reports lost paid work. |

---

## 5. The physical channel: the build-out is raising costs for everyone else

| Input | Direction now | Reading (as of) | Who actually paid for the curve |
|---|---|---|---|
| Commodity DRAM | **UP** | DDR4 8Gb chip contract $1.50 (Oct 2023) → $25 (late Aug 2026), 16.7×. Conventional DRAM contracts +93–98% q/q in 1Q26 (TrendForce, Jun 2026). Memory and storage together are ~35% of HP's PC bill of materials, an FY2026 estimate, up from ~15–18% (HP's CFO, 24 Feb 2026; press reported it as DRAM). Memory is 30–40% of a smartphone's bill of materials, up from ~10–15% (TrendForce, Feb 2026). HBM is forecast at ~22% of the top three suppliers' wafer input by end-2026, for ~9% of bits (TrendForce forecast, Jun 2026). Suppliers see tightness through 2027–28 (Micron, 30 Sep 2026, VENDOR; Samsung, Jul 2026, PRESS) | crowding by HBM |
| Large transformers and switchgear | **UP** | power-transformer unit cost +77%, 2019–2025. Lead times: ~120 weeks (2024 global average) → 128 for power transformers and 143 for generator step-up units (US, Q2 2025) → step-up units >160 weeks (Q1 2026) | none (custom units) |
| Gas turbines | **UP** | US turbine capex doubled in two years. Global average combined-cycle cost +16% to $102/MWh (2025); US costs "far above global averages" (BNEF, Feb 2026) | utilities; AI is the marginal buyer |
| Optical fibre | **UP** | ~$6.30 per fibre-km, +70% from the 2021 trough (May 2026) | telecom; AI now crowds it out |
| Electricians | **UP** | one Abilene, Texas contractor pays $20/h against up to $35/h on data-centre jobs, ~75% more (PRESS, Apr 2026). Electrical work is 45–70% of data-centre build budgets | crowding |
| SiC and GaN power chips | DOWN | 6-inch SiC substrates below $500 (Q4 2024), ~$400 (2025) | **EVs** and Chinese overcapacity; AI inherits |
| LFP storage cells | MIXED | stationary packs $70/kWh in 2025 (−45%); then Chinese storage cells +22% (Oct 2025–Apr 2026) | **EVs**, China |
| Lidar | DOWN | Hesai average price ~$530 → ~$260 (2024–25) | **ADAS**; FMCW photonics firms pivot *into* AI optics |
| InP lasers and coherent optics | UP now; plausibly DOWN later | demand exceeds supply by 30%. Nvidia invested $4bn in Lumentum and Coherent, plus separate multi-year deals for priority laser access (Mar 2026) | **AI**: one of the few inputs where AI is plausibly the anchor of a later decline that telecom would inherit |
| Enhanced geothermal, iron-air | unit cost falling or unknown; price to others rising or unpublished | both fail as enablement (§6) | EGS drilling-cost fall came from **shale** practice and DOE FORGE, pre-AI; AI co-finances the next rung |
| Data-centre waste heat | DOWN (free) | C-9 (watch) | by-product |

**The third derivative in reverse:** product classes being *un-enabled* by the build-out.
- **Sub-$500 PCs**, which Gartner expects to disappear (PRESS: The Register relaying Gartner, 26 Feb 2026; Gartner's own pages were bot-walled in F08). PC shipments fell 20.1% y/y in Q3 2026, to 62.7M (IDC preliminary, 8 Oct 2026); IDC cites AI-driven supply constraints and prices as well as a first-half pull-in.
- **Small single-board computers**: Raspberry Pi price rises, including a further $12.50 on 2GB Pi 4 and Pi 5 boards (1 Oct 2026, VENDOR). A 1GB Pi 5 was launched at $45 on 1 Dec 2025, a downgrade because memory got dearer.
- **New entry smartphones**: India's refurbished-phone volumes rose 13% in H1 2026 while new-phone volumes fell ~11%, on "rising memory prices" (PRESS: Counterpoint via ETV Bharat, 2 Sep 2026).
- **Renewables and EV depots** waiting on transformers. Wood Mackenzie put up to 25% of renewable projects at risk of delay (2024).
- **Housing**, which competes for electricians.
- **Industrial sites moving into AI:**
  - Hawesville's interconnection went to TeraWulf;
  - Alcoa is selling 10 sites to data centres;
  - Hy2gen cancelled its 240 MW Sauda ammonia project after losing its grid allocation, and is exploring a data centre there.

This is S7 at full strength, the mirror image of J3.

---

## 6. What failed, by the single test or constraint that binds

### DIRECT under the §0 line

**(a) The customer buys AI judgement or content**
- **Lenders running their own credit models:** Sea Monee, Amazon seller lending, Apollo, Drip Capital.
- **Microinsurance with AI claims decisions.**
- **Camera-monitoring services:** the warning *is* the product.
- **AI-authored language courses (LEAD):** Duolingo built 148 courses in about a year (VENDOR). The content is AI-authored, not a human work rendered.

**(b) An existing operation made cheaper**
- **Robot cells in existing small factories.**
- **Walmart's AI supplier negotiation (Pactum).** It lengthened payment terms by ~35 days on average (VENDOR, undated), so it runs *against* small suppliers.

**(c) The AI-native seller captures the growth**
- **Xometry's custom-parts marketplace:** revenue +45% y/y, ~35% gross margin (Q2 2026). Its instant quoting also predates LLMs (2019).

**(d) Sector-specific tools:** C-4, C-5, C-8 and the handwritten-archives lead (§4). With (d) relaxed, C-5 and the archives would still fail (b), and C-8 test 4 (F07, F15); only C-4 would return, on a 2017–20 crossing.

### Not an AI effect

- **Photo-verified crop insurance (ACRE Africa).**
  - Severe damage was visible in farmers' photos at 71% of affected sites, against ≤34% for index products (India pilot, Ceballos, Kramer & Robles, 2019).
  - Experts read the photos, so the cost that fell is the field visit, replaced by **smartphones**.
  - An insurer that ran a model on the photos would be DIRECT under rule (a).
- **Pay-as-you-go asset finance and tractors.** These run on device locks, mobile money and GPS telematics.
- **Hima Seafood trout on Green Mountain data-centre heat (Rjukan).** The heat deal was announced on 28 Jun 2021, before the build-out, as "a significant cost saving" (PRESS: Fish Farming Expert); the site was chosen for cold, pure water. The farm operates (900 t in 2025, PRESS) and the up-to-1.75 MW heat loop has been in a test phase since autumn 2025 (PRESS relaying Green Mountain, Feb 2026). Fails test 2.
  - A pre-build-out precedent of the same kind: White Data Center's eel farm on server-warmed snowmelt at Bibai, Hokkaido, commercial by Jul 2024 (PRESS: Hokkaido Shimbun). Like C-0, it shows the mechanism, not AI.
  - Green Mountain also delivers its cooling water free to a land-based lobster farm at Rennesøy (PRESS: Politico, 29 Aug 2023); no AI load is shown, and current production is unverified (F14). Green Mountain hosts AI/HPC at two unnamed Norwegian sites (VENDOR, Feb 2024), so Rjukan's AI load is unshown too.

### Capital, credit, liquidity and regulation bind

- **Enzymatic PET recycling.** Capital binds: Carbios's plant missed financial close.
- **Custom medical devices.** Regulation binds: verification and the regulatory file.

**Trade finance** (also DIRECT at test 1: credit and KYC decisions, rules a and d; the ranking below shows cognition was not binding anyway)
- The gap reached $2.5tn by 2023 and is unchanged in ADB's 2025 survey (2023–24 data; bank views from H1 2025). Those data predate most bank AI deployment, so the flat gap alone does not prove failure.
- **Banks' own ranking does:** dollar liquidity and counterparty risk come first. KYC is ranked first by just over 15% of respondent banks.

**Small US banks**
- Compliance averaged 8.7% of noninterest expense for banks under $100M in assets, against 2.9% at $1–10bn (2014 data; St. Louis Fed, Jul 2016).

**Truck back-haul without brokers**
- The broker spread pays for quick-pay, credit and liability. Convoy died on capital.

### The cheapened input never bound, or was already cheap

- **AI-handled contact on a new microinsurance product.** It passes the line (general-purpose text and speech, new product) but fails test 4. One human assisted contact costs $6.60 (Deloitte global cross-industry average, Mar 2024 survey), about half of the $13 weighted average premium per person covered (RFILC Landscape 2024, 2023 data). But low-touch insurers already sell cheaply: Turaco averages ~$2 a policy. 58% of agricultural microinsurance products are subsidised (RFILC Landscape 2024, 2023 data).
- **Precision fermentation.** Feedstock, capital and conversion make up more than two-thirds of the cost drivers.
- **n-of-1 antisense drugs.** Development and manufacturing cost ~$1m per patient.
- **AI-screened materials.** 736 made, none sold (WEAK).
- **Welsh-language TV.** The programme service is 77.3% of S4C's Public Service Fund allocation (2024–25). Dubbing was never the binding line.
- **Small-business acquisitions.** Quality-of-earnings work is ~0.3–3% of the price on $500k–$2m deals (CALC on VENDOR price bands, Sep 2026).
- **First-time fund managers.** Platform administration is ~$20–35k a year on a $10M fund (AngelList's current, undated tariff).
- **Retrofit CNC and open hardware.** Control software has been free since NIST's EMC in 1994.

### A statute or public rail did it (R4)

- **Micro-firm invoice finance:** India's TReDS.
- **Cheap KYC:** Aadhaar.
- **Peer-to-peer energy sharing:** Austria's 2021 law.
- **Small US fund sponsors:** 433 entered in 2014–24 at the old cost. The ETF wave rests on SEC Rule 6c-11.
- **Mid-cap hedging:** EMIR Art. 9(1a), inserted by Reg (EU) 2019/834 and applicable from 18 Jun 2020, shifted reporting of OTC derivatives with an EU financial counterparty onto that counterparty for NFC- firms (below the clearing thresholds). NFC- firms still report exchange-traded and other trades themselves.
- **Captioning (LEAD).**
  - ADA Title II creates the demand. Ohio State took every uncaptioned video in its secure library offline in summer 2025. Compliance dates are 26 Apr 2027 and 26 Apr 2028.
  - AI lowers the first pass, but the per-title human accuracy check binds. This is a statute crossing running in reverse.

### Fails the new-output or threshold test (physical)

- **Enhanced geothermal inherited by industry.** ~$107/MWh (Lazard illustrative, Jul 2026), against $30–40/MWh for smelters and ≤$40/MWh for ammonia. Even the utility pay point (~$100) is not crossed without subsidy: **Google pays the premium** under NV Energy's Clean Transition Tariff. Grok and the reviewers rated the *mechanism* PLAUSIBLE; this map rates the inheritance as failing test 4. It is tracked only as a signal (§8).
- **Iron-air storage inherited by utilities.** A utility buying cheaper storage for the same electricity fails test 2. The first anchor was itself a utility (Great River Energy, 2020).
- **AI data-centre heat to an existing fish farm (Nscale, Glomfjord; F14).** Nscale, an AI GPU cloud, says its ~34 °C cooling water warms a nearby fish farm's tanks, which "saves the farm from expending its own energy on heating" (VENDOR, 17 Nov 2025; farm unnamed, no capacity or start date). Real AI heat reaching a food producer, but an existing operation made cheaper: fails test 2.
- **Desalination for staple crops.** Fails a ~€0.30/m³ water price.
- **Hydrogen-DRI steel.** Fails a $490–520/t blast-furnace benchmark.
- **Memory-glut residue (S10, conditional on a bust).** Fails test 2; test 4 is not crossed (F08).
  - The last two gluts restored existing products. In 2019 the price fall (contract ASP down >20% in 1Q19) "did not stimulate a recovery in demand" (TrendForce, Mar 2019). What followed was more memory per phone (~5GB in Q4 2020, +22% y/y, Counterpoint; 2020 is confounded by the pandemic) and a cheaper existing 2GB Raspberry Pi 4 ($45 → $35, Feb 2020, VENDOR).
  - 2023 was below cost (Micron FQ2 FY2023: GAAP gross margin −32.7%, $1.43bn inventory write-down, VENDOR filing; DRAM and NAND together), the S10 mechanism itself. The forecast response was again more memory per phone (+14.3%, TrendForce, Aug 2023).
  - The products memory-bound now (PCs, entry phones, single-board computers) paid at 2025 cost shares. No product is named that pays only below the 2023 trough. The one class wanting more memory than 2023 configurations is on-device AI, which is DIRECT (a).
  - If HBM's wafer share fell back to its 2023 level, conventional bits would rise by ~19% of end-2026 supply gross, ~12.5% net of the HBM bits given up: about one year of normal growth at once (CALC on TrendForce forecasts; mixed bases).
  - No 2026 forecaster puts a down-cycle before 2028. Bernstein's 2028 SK hynix price of ~$1.05/GB (−50%) still leaves ~86% gross margin (PRESS, Jul 2026).
  - Tracked only as a signal (§8).

### Same-market, or AI substitutes for the product

- **Agent-to-agent payment protocols.** The agents buy AI services; x402 daily volume fell ~95% from Jan to Sep 2026.
- **Small freelance markets** shrink rather than open. Fiverr's active buyers fell 21.9% y/y (Q2 2026).

---

## 7. Logic: four new rules (added to map §4 as L14–L17)

- **L14. Fixed cost per unit of variety.**
  - Cheap general capability enables businesses where a fixed cost per title or per language was binding.
  - The result is a longer tail of an *existing* category: the AWS shape, with more experiments and more failures.
  - **Count consumption, not titles.** A tail can flood, as music did in 2025–26 (LEAD).
- **L15. Crowding: the reverse threshold.**
  - During scarcity, the anchor buyer bids away inputs it shares with others, and un-enables product classes.
  - Apart from by-product heat (R5), physical enablement needs an AI-anchored decline that reaches others, or a bust (J3). For memory, the 2019 and 2023 record says a bust restores existing products rather than enabling new ones (F08, §6).
- **L16. A statute that looks like a cost fall.**
  - Every measured cost collapse among this round's finance, compliance and energy-sharing candidates came from a statute or public rail.
  - Statutes also *push* heat reuse (EnEfG, LEAD; Denmark's Order 1167 and Finland's Act 1382/2025, F05; Ølgod's zoning permission makes the data centre conditional on the greenhouse, F14) and *pull* captioning (ADA Title II, LEAD). Public money carries some candidates outright: Korea's state K-FAST dubbing channels (F12), Québec's heat-capture grant at Lévis (F14), METI's localisation subsidy (F04, F13).
  - Check for a concurrent rule change before crediting AI.
- **L17. The free layer is the platform's.**
  - When a builder or distributor supplies the AI layer at zero, the enablement is real for producers, but the rent stays with the platform and the layer can be withdrawn.
  - Where a tail floods, platforms ration attention. So far this is seen in music (LEAD); book, audiobook and video platforms use labels and distribution limits only (F01).
  - Platform access can bind before cost: Google's free auto-narration (2020–22) left no measured market, and ACX still requires human narration unless authorised (F11). Storytel owns 38% of its translation supplier (F10).

---

## 8. Dashboard: enablement signals to watch

| Signal | Row | Reading (as of) | Enablement shows as |
|---|---|---|---|
| Fixed-capability model price | all | ~13×/yr down; GPQA-Diamond $0.30 → $0.0004 per question (Epoch AI, 22 Sep 2026) | pass-through into *posted service* tariffs |
| Posted AI service prices | all | Google machine translation $20/M characters (Mar 2014 and Oct 2026); newer Gemini Flash input doubles on 1 Jan 2027 | a first cut in a service list price |
| AI-translated long-form | C-1 | WebNovel >30,000 AI-translated works, 40% of its novel revenue (H1 2026, against >35% in H1 2025; VENDOR filing, unaudited interim, 11 Aug 2026); revenue per AI title ~−70% in 2025 (CALC); works in less-common languages +160%, all works, not AI-only (base undisclosed); US app-store spend ~$13–18M a year, flat 2023–24 (Sensor Tower estimates, CALC); Storytel's Nuanxed purchases −44% in 2025 (VENDOR filing); Kindle Translate "millions of pages" (VENDOR, Jun 2026) | independent revenue per title (still none); a WebNovel revenue line; a named Storytel series and its listening (Q3 report, 27 Oct 2026); Amazon's multi-language share ≫5% |
| YouTube auto-dub | C-3 | >6M daily viewers ≥10 min (YouTube blog, VENDOR, Dec 2025 data); one sub-100k channel: 0.2% of watch time from its English dub (VENDOR, Oct 2026); no RPM from any source (F03) | ad revenue per thousand views from dubbed views, for channels under 100k subscribers (still unfilled) |
| Audiobooks vs e-books | C-2 | ~1M vs >40M (PRESS relaying Spotify, Sep 2026); AI-narrated titles .03% of APA-reporting publishers' 2025 receipts (APA, Jun 2026); Virtual Voice >50,000 titles (PRESS, May 2025); Spotify's tools open to US self-publishers since 9 Sep 2026, no uptake figure | a measure of the self-published tail (APA's questionnaire, or whether Audible reports Virtual Voice receipts); Spotify digital-voice uptake |
| AI share of long-tail consumption | C-1 to C-3 | Deezer: ~0.5% of streams on 28% of deliveries (Sep 2025) → ~1–3% on 44% of daily uploads (Apr 2026) (LEAD; PRESS relaying Deezer). Audiobooks .03% of reporting publishers' receipts (APA, 2025); Audible ≤~0.02% of a year's listening (CALC). WebNovel 40% of novel revenue (VENDOR filing, H1 2026), revenue per AI title ~−70% (2025, CALC) | streams and reads rising with titles, or not |
| Catalogue AI dubbing | C-3b (watch) | Love TV / Cineflix Rights series in Spanish, Italian and French on FAST channels (VENDOR, Feb 2026; content for equity); Seven.One Studios International → DubMe IO, 30 languages on YouTube (company release, Jun 2026; forward-looking); Korea's state K-FAST channels ~100M cumulative views, Dec 2025–Apr 2026 (PRESS, Jul 2026; state-funded) | a licence fee or ad revenue for a dubbed catalogue title; commercial viewing outside a state programme |
| First-English manga | C-6 | ~100 emaqi exclusives in a 400+-title subscription (company, Jul 2026); up to 11 first-English titles (PRESS, Oct 2026); no sales or MAU; emaqi Android installs 388K+ cumulative, +8.2K in 30 days, −8% (tracker estimate, whole store, fetched 15 Oct 2026); Comic Growl 28 English series against a METI-funded 50+ target (15 Oct 2026) | sales or MAU; a licensor's own statement; whether subsidised titles use AI (METI menu-8 round 3, results late Nov 2026) |
| Waste-heat new-output hosts | C-9 | Lévis (Innoserres next to QScale): first strawberries expected winter 2026–27, not shown operating (Québec ministry officer, Mar 2026). Ølgod: local plan approved 6 Oct 2026 (company-reported), pre-FID, financial close targeted Dec 2026, first season Q3 2028 (VENDOR, 14 Oct 2026). Nscale Glomfjord: ~34 °C to an existing fish farm (VENDOR, Nov 2025). NTT Docomo Business data-centre heat to a land-based shrimp demonstration, Oct 2026–Mar 2028, framed as a cost saving (VENDOR, 7 Oct 2026). Uithoorn is substitution | Lévis commissioning (or Québec's first electricity-aid payment); Ølgod's financial close; NTT's interim report (late Mar 2027); a published heat price to a food host; a host that exists because of *AI* heat |
| Automated sport production | C-4 (excluded by d) | Pixellot 163,185 games in the last month (VENDOR, Oct 2026); ~1.5M in 2025, Hudl >1M (PRESS: SBJ, Apr 2026); LiveBarn revenue in the $80M range (PRESS, Jan 2026) | a 2024–26 third-party count of streams below varsity level that did not exist before |
| DRAM and HBM wafer share | §5, §6 | DDR4 8Gb $25 (late Aug 2026); HBM ~22% of top-three wafer input by end-2026 (forecast, Jun 2026); suppliers see tightness through 2027–28 (Micron, 30 Sep 2026, VENDOR); earliest named oversupply 2028 (Bloomberg Intelligence, PRESS, Jul 2026) | HBM share reverting and prices below 2024: relief for the products in §5 (S7 reversing). On the 2019 and 2023 record a glut restores; it does not enable (F08) |
| Transformer lead times | §5 | step-up units >160 weeks (Q1 2026) | shortening as the 2027–29 factories open |
| Optics gap and fibre price | §5 | InP short by 30%; fibre +70% from the trough (May 2026) | forecast price declines; telcos adopting 800G ZR |
| Firm clean power vs pay points | §6 | EGS ~$107/MWh (Lazard illustrative, Jul 2026); firm clean energy "can command" $100–130/MWh (Rystad via Fervo's S-1/A, May 2026, VENDOR filing) | a non-AI industrial contract below $80/MWh |
| Reverse flow (mirror of J3) | §5 | Hawesville, Alcoa and Sauda moving *into* AI (to Mar 2026) | energised capacity sold to a **non-AI** buyer at ≤⅓ of cost |
| Reverse enablement in services | §6 | Fiverr active buyers −21.9% y/y (Q2 2026); deepfake suspicious-activity reports rising (FinCEN) | small-deal markets shrinking; trust costs rising |

---

## 9. Questions for the project owner, and next steps

**Q1. Rule (d): general-purpose costs only?** *[16 Nov 2026: decided in 05 §9 item 1 (the project owner, 16 Oct 2026): rule-(d) chains are kept and scored in a second book, not delivered.]* F07 tested the relaxed branch. It now changes the answer by one row, and that row crossed before the build-out. The sub-question on rule (a) below now carries more weight.
- **Keep (d)**, the strict Netflix analogy: the build-out's candidate enablement is long-form text and speech. C-1 is the strongest; C-3 and C-2 are weaker, and C-3b is on watch.
- **Relax (d)**, so that sector-specific AI tools count when they create new output:
  - C-4 unstaffed school and amateur sport returns, EMERGING. New sub-varsity streams are shown at a named school and named districts (a school page and trade press, 2018–19), and paid demand is real (LiveBarn revenue in the $80M range, PRESS, Jan 2026). But the crossing came in 2017–20, from free cameras and the staffing constraint, before the build-out. It would sit beside C-0 as a pre-build-out S1 case, not as a build-out enablement;
  - C-5 designed reagents stays out: the named buyers (Bio-Techne, Gator Bio) are incumbents improving existing products (rule b), and no new test maker is named;
  - C-8 one-off parts fails test 4: no price series shows one-off parts getting cheaper (machine-shop PPI about −2.5% real, Jan 2023–Aug 2026, CALC);
  - consistently, a robot-weeded organic plot would be judged the same way.
- **On present evidence, the (d) choice decides how C-4 is filed, not what the build-out enables.**
- **Scope of (d), sharpened by F13 and F15.** Does (d) cover a sector-specific AI layer run by a third party (Mantra in BOOK☆WALKER's viewer; a handwriting index sold by ArkivDigital or ARCHION), or only tools inside the enabled firm's own production? This map applies (d)'s general-purpose sentence, so both are excluded. Read narrowly, both revert to leads at WEAK; neither changes the answer, because neither route shows new paid output.
- **Sub-question on rule (a):** §0 treats AI *rendering* of a human work (translation and voice alike) as not AI content, like a printing press.
  - If all rendering counts as AI content, C-1, C-2, C-3 and C-3b all fall, and nothing from the build-out survives.
  - If only synthetic *performance* counts (a voice the listener hears), C-2, C-3 and C-3b fall and C-1 remains. Its sellable form keeps a human post-editor. After F01–F03, C-1 is also the row with the strongest consumption evidence.
  - F10–F12 bear on this: customers notice the synthetic performance (Prime Video's AI anime tracks removed by 4 Dec 2025; French distributors that tested synthetic voices backed away, CNC, Oct 2025; 65% of listeners sought a narrator they liked, NielsenIQ for Audible, Oct 2026), while C-1's post-editor is credited by name (Gummerus credits the post-editor plus Nuanxed, Apr 2024).

**Q2. The working question.** *[16 Nov 2026: 05 governs; 05 §5.6 records that web fiction did not pass.]* The evidence suggests asking: *which general-purpose fixed costs per title or language has AI collapsed, who controls distribution of the resulting long tail, and does consumption follow the titles?* Adopt this? The F rounds answered the last part: yes at WebNovel in share (40% of novel revenue) but not per title (~−70% in 2025, CALC); no among reporting audiobook publishers (.03%), with the self-published tail unmeasured; not measurable for YouTube's long tail or catalogue dubbing.

**Research round F01–F08: done** (dispatched 15 Oct on your go-ahead; Cursor Included 56% before).
1. **Done (F01).** Listening and reading share of AI-made titles: WebNovel 40% of novel revenue (H1 2026); audiobooks .03% of revenue (2025); YouTube publishes no share.
2. **Done (F02).** Independent revenue per AI-translated title: none exists; WebNovel's share is issuer narrative; VBK's outcome is still unreported.
3. **Done (F03).** Auto-dub revenue for small channels: no RPM from any source; one in-band case at 0.2% of watch time.
4. **Done (F04).** Named Japanese licensors: six named; no sales; no US publisher uses AI for titles it would not otherwise publish.
5. **Done (F05).** Waste heat: no FID; district-heat prices only; Hima is not an AI effect; Denmark and Finland mandate reuse with a cost-benefit escape, the Netherlands only reporting.
6. **Done (F06).** Archives: no new paid work found.
7. **Done (F07).** If (d) is relaxed: see Q1.
8. **Done (F08).** HBM-reversion glut: restoration, not new output; filed in §6.

**Research round F09–F15: done** (dispatched 15 Oct on your go-ahead; Cursor Included 57% before).
1. **Done (F09).** WebNovel: no revenue line and no split by language exist; the +160% covers all works in less-common languages, not AI-translated ones only; the human pipeline (~1,000 titles a year) stopped in 2024, and ~69–90% of AI additions exceed it (CALC, upper bound); revenue per AI title fell ~70% in 2025 (CALC).
2. **Done (F10, ahead of the Q3 report).** Storytel: faster substitution, WEAK; one open strand (Gummerus's digital-only backlist); Storytel owns 38% of Nuanxed, and its Nuanxed purchases fell 44% in 2025.
3. **Done (F11).** APA measures reporting publishers' receipts, so the self-published tail is probably outside; Spotify's tools, open to US self-publishers since 9 Sep 2026, have no uptake figure.
4. **Done (F12).** No fee or ad revenue for any catalogue AI dub; Korea's ~100M cumulative views are state-funded; Love TV is a Cineflix affiliate. C-3b moves to watch.
5. **Done (F13).** No emaqi sales or MAU (a tracker shows the whole store's Android installs); no Bushiroad title is shown first-English *because of* AI; METI's official row names no AI.
6. **Done (F14).** No FID at Ølgod yet; no heat price to a food host; a second dated host at Lévis (winter 2026–27); AI heat reaches one existing fish farm as a cost saving.
7. **Done (F15).** Archives: no new paid work after two parcels; every index uses handwriting-specific recognition; moved to the rule-(d) table.

**Next round (proposed, not dispatched).** Q1 and Q2 stay open for you.
1. Storytel's Q3 report (27 Oct 2026): a named translated series (language, prior human edition); which associate was divested in Q2 (−SEK 0.7m; if Nuanxed, the interested-party link changes); JUJU's translated titles; the Publishing margin explanations (C-1).
2. WebNovel's app-store spend in 2025–26 (Sensor Tower): does the flat 2023–24 US series move after the AI scale-up (C-1)?
3. Whether Audible reports Virtual Voice receipts to the APA survey, or APA's 2026 questionnaire (C-2).
4. A fee, ad revenue or viewing figure for Cineflix's Spanish Mayday channel or Love TV's dubbed hours; K-FAST ad revenue net of subsidy (C-3b).
5. METI menu-8 round 3 (results late Nov 2026) and any menu-5 award naming AI; Comic Growl's English count against 50+ (C-6 lead).
6. Ølgod's financial close (Dec 2026); Lévis commissioning or the first electricity-aid payment; the QScale sale; Salfjord's data centre (ownership, AI load, temperature) (C-9).
7. Ancestry's new-country launches: which countries, and whether translation (general-purpose) or handwriting recognition (rule d) was the binding cost (new lead).

---

## 10. Verification record

**Evidence**
- 578 items: 567 verbatim, 1 the same fact in other words, 10 bot-walled, 0 spliced, invented or dead.
- My own spot checks: Hudl "1M+ games … a majority captured automatically" and ECNL "more than 1,200 games", both found on the live pages.
- Most pro-enablement evidence comes from interested parties: YouTube, Amazon, China Literature, Pixellot, Deep Green, Orange, Monod Bio, Storytel (38% owner of Nuanxed), Cineflix (stakeholder in Love TV). **Independent revenue data is the main gap.** The F rounds did not close it: the first revenue share (WebNovel, 40%) is issuer narrative in an unaudited interim, and the independent figures (APA's .03% of reporting publishers' receipts, the machine-shop PPI, Sensor Tower's flat WebNovel US spend, Riksarkivet's falling search visits) point against enablement or away from it.

**Corrections across the three fact-checks**
- **Pairing errors.** Deezer's 44% of uploads (Apr 2026) goes with ~1–3% of streams; 0.5% belongs to Sep 2025.
- **Forecasts stated as results:** PC DRAM, the HBM wafer share.
- **Dropped caveats:**
  - fibre's 2.7% utilisation;
  - containers' North–North-only effect;
  - M-KOPA's cumulative vs active customers and its restated profit history;
  - the trade-finance survey's data years.
- **Unlabelled vendor claims:** Pactum, the manga 2%, the dashboard counters.
- **Factual errors:**
  - the $90 videographer is district staff;
  - Nvidia's $4bn was an investment;
  - web-fiction revenue was for 2024;
  - Google, not utilities, pays the geothermal premium;
  - EnEfG's "at cost" clause sits in §11(3) no. 3.
- **Comparator.** Translation is compared at sellable, post-edited quality (~90%), not raw (~99.9%).
- **Line and placement.**
  - The DIRECT line now has four rules, and all four of the project owner's examples fail it.
  - C-4, C-5 and C-8 are excluded by (d) and shown separately.
  - C-6, C-7 and C-9 are on the watch list.
  - Iron-air, geothermal, bespoke supply and crop insurance are filed once each in §6.
  - GPS → ride-hailing reverts to FAILS.
  - Containers: 01 §2 (H15) rejected them under the strict test. Under 03's test 4 ("or constraint") they pass on handling cost.
  - M-PESA → pay-as-you-go solar: STRONG is held pending the paybill fee.
  - Consumer genomics fails the Netflix test; only the forensic step passes.

**Arithmetic slips in Grok's returns (11)**
- **E01:** delivery exceeded the plan only through 2001 (~$15 at 2002 prices, already below $17.99). The lag from the 2002/2006 price breaks to 2007 is 1–5 years, not 5–9.
- **E02:** a "hundred-fold" gap contradicts the return's own 500–2,500× bound. One $6.60 contact is about half of a $13 premium, not all of it.
- **E03:** AI's share of the EGS contract book was ~19% (115 of 610.5 MW), not 0.57%.
- **E06:**
  - $45/MWh misses every ammonia threshold;
  - 6.6¢/kWh is above the 5–6¢ desalination reference;
  - a 25% green-steel premium implies a ~$520/t benchmark, not $490.
- **E10:** two flagged lines, one issue: the hourly break-even was stated ~2× too high.
- **E14:** Grok compared a DDR4 *chip* with a *module*. The like-for-like chip series is $1.50 → $25.

**Follow-up round F01–F08 (v1.4)**
- 234 evidence items re-fetched: 218 verbatim, 16 behind bot walls, **0 spliced, invented or dead**. One immaterial slip (F04: Japan's 2033 target is "more than threefold, to 20 trillion yen", not "above 20 trillion").
- **Not used (bot-walled):** Iyuno's dubbing quote (Slator); emaqi's BusinessWire releases (13,000 volumes, "nearly 50 exclusives", the never-before-translated list; launch facts survive via ANN); Protolabs FY2025 and all Xometry figures at the cited IR pages (SEC copies agree); MHSAA's 33,056 streamed events; six Gartner items (2019 price fall, PC memory share, sub-$500 PCs by 2028, Q3 2026 shipments, DRAM 5×, refurbished phones).
- **Corrections to v1.3:**
  - Prime Video's AI Spanish dubs did not stay: removed on three titles by 4 Dec 2025.
  - HP's 35% is memory *and* storage, an FY2026 estimate of HP's own bill of materials, not DRAM alone.
  - Orange's ~2% is the share of Japanese manga with an English edition **by volume**, not of titles reaching the US.
  - The >6M auto-dub viewers are on YouTube's own blog (VENDOR); the ~75% duration is a PRESS-relayed platform average.
  - LiveBarn: ~2,270 venues and >4,000 surfaces (Jan 2026), not ~3.6k venues.
  - C-4's "no cost fall" rested on a 2020 vendor quote; at Pierre's volume a game cost ~$9 (CALC, 2019).
  - Hima Seafood is operating, not unverified, but on a 2021 cost-saving deal: out of C-9.
  - Ølgod's Q3 2028 is a developer target, pre-FID; the municipality says 2030.
  - FamilySearch: ~2.3B AI-transcribed images by 2026, not "nearly 2 billion".
- **Placement changes:** C-2, C-3 and C-9 to WEAK; catalogue dubbing from LEAD to sub-row C-3b (HYPOTHESIS); Hima to §6; the memory glut to §6 (fails test 2); C-5 and C-8 no longer reach the watch list if (d) is relaxed; a new lead for rights holders' own manga editions.
- **Leads dropped:** Ailaysa (rule c; a showcase title about AI), Audible publisher narration and speech-to-speech translation (nothing to place; belongs to C-2), Shueisha via Mantra (rule b), Manga Million (free; AI disputed), OldNews.com and Storied (printed archives searchable before AI: rule b), SoFast (supply layer), BallerTV, Arzeda and FloSports (rules b, c, d). Refurbished phones and the 1GB Pi 5 are S7 evidence (§5), not candidates.

**Follow-up round F09–F15 (v1.5)**
- 216 evidence items re-fetched: 212 verbatim, 1 the same fact in other words, 2 bot-walled and not used (AppBrain's emaqi page; DCD's Google Hamina page), 1 not found as claimed (Grok said METI's results page was a 404; it is live and is now cited). **0 spliced, invented or dead**; no arithmetic slips.
- **Corrections to v1.4:**
  - APA's .03% is a share of reporting publishers' 2025 receipts, not of 2025 audiobook sales revenue; the self-published tail is probably outside it.
  - Audible's >50M AI minutes cover all its AI output, publisher-side production and translation included, not Virtual Voice alone.
  - Spotify's ElevenLabs tools: invite-only from Jun 2026, open to US self-publishers since 9 Sep 2026.
  - The +160% is not WebNovel's sharpest new-output signal: it includes human translations and local-language originals, and the Chinese release names Yuewen as the base.
  - Revenue per AI title can be computed on one base: ~−70% in 2025 (CALC), replacing "cannot be computed".
  - Storytel: not only "its CCO sits on Nuanxed's board". Storytel owns 38% of Nuanxed, and Nuanxed's CEO is ex-Storytel.
  - emaqi: "~100 of ~2,500, ~4%" mixed a subscription count with a store count and is withdrawn; "11 more first-English titles" is "up to 11".
  - Manga Million: "denying AI use; disputed" becomes all professional translation (Shueisha guide), AI offered and declined.
  - C-9: "no food host runs on AI heat" becomes no *new-output* food host (Nscale's AI site warms an existing fish farm). DEN02's "cooling type not stated" becomes "will accommodate" direct liquid cooling, no share.
  - C-3b: the Love TV quote comes from a Cineflix affiliate (content for equity); Seven.One's source is its own release (9 Jun 2026).
- **Errors in Grok's returns, caught in review:** the seed's "3,600 by end-2022" dates from Oct 2023 (end-2022: ~2,900); the end-2024 non-AI stock is ~3,000, not ~3,600 (CALC); a 2024 flow was compared with a 2026 stock, and a platform-revenue share with a novel-revenue share; Nuanxed's homepage does show HarperCollins, Blackstone and Natur & Kultur (only BookBeat is absent); Kristoffer Lind founded Lind & Co, not Nuanxed; Storytel's AR 2025 does quantify a translation cost; Cineflix's "5 00 hours" was an extraction artifact; Prime Video's Spanish-track removal is reported for three titles, not five; the Uithoorn deal was signed the week before the 21 Jul 2026 release; Ølgod's 174 ha is the plan area, not greenhouses (4 × 10 ha); METI's results page is not a 404.
- **Placement changes:** C-3b to the watch list (test 4 unshown, as for C-6); the archives lead to the rule-(d) table; the Storytel strand of C-1 to WEAK; the rights-holder manga lead to WEAK; Nscale Glomfjord to §6 (fails test 2); Green Mountain's Rennesøy lobster farm to §6 (not an AI effect). C-1, C-2, C-6 and C-9 keep their placements.
- **New leads:** Gummerus's digital-only backlist series (C-1); Goalcast's French spin-off channel (C-3); Lévis (C-9 host); Salfjord, a salmon company building a data centre as a fish heater (C-9); Ancestry's country launches (unresearched).
- **Leads dropped:** GoodNovel and BueNovela (no firm-level AI link); print and audio editions of WebNovel originals (no translation cost; a pre-AI path); Yuewen's overseas print, manga and screen editions (cumulative, mostly pre-AI); Kindle Translate authors, indie foreign editions and YouTube auto-dub creators (duplicates of C-1 and C-3); Nuanxed's publisher clients (supply side); Danish post-editing publishers (rule b); Kobo synthetic audiobooks and resale of Google auto-narration (production routes into C-2); Watch the Skies (Flawless lip-sync, rule d; the actors re-recorded in English); the IP360 menu-5 platforms (rule b, no AI named); Square Enix (a comment, no output); Comisma (subsidy, no AI); the Southern Virginia farm park (no site; a gas-CHP design); ArkivDigital and ARCHION as candidates (rules b and d).

**Open**
- M-PESA's threshold on M-KOPA's own unit: the paybill fee per KES 40 instalment was not fetched.
- Dubbing (C-3): settled toward WEAK by F03 (one in-band case, default-on enrolment, no RPM).
- Rule (d) at the archives' index layer and on Mantra: resolved toward exclusion (F13, F15). Every index found uses handwriting-specific models, and Dwango calls Mantra manga-only. What remains is the scope of (d) for a third party's sector-specific layer (BOOK☆WALKER's overlay; a bought index): §9 Q1. General vision models are cheaper per page (CALC, 2024 list prices), but no index in the record is built on them.
- C-3b's placement: if you prefer the C-2 rule (cost crossed and enabled party visible is enough), it returns to the survivors; v1.5 applies the stricter one (a positive cost must be shown to pay), as for C-6.
- WebNovel's counts: from H2 2025 the filings may count language versions (>17,000 AI works against >13,600 translations of all kinds); the ~90% upper bound for 2025 inherits this.
- Part of WebNovel's new output may be licensed replacement of unlicensed machine-translated reading, which predates the build-out (reviewer's note; not sourced this round).
- Lévis: the ministry's "l'hiver prochain" (Mar 2026) is unconfirmed; La Presse corrected an earlier version of its story, and links a 6 Feb 2026 story on QScale weighing a sale.
- Ølgod's 6 Oct 2026 local-plan adoption is company-reported; no Varde adoption notice was found.
- Storytel's ~85% of listening tied to local authors and languages (which caps all translated listening at ~15%) needs a dated source.
- The cloud video cost per camera ($26 vs $65–86) depends on resolution tier and model. That class is DIRECT anyway.

