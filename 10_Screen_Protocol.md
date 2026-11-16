# Screen protocol

*v0.1 · 18 Oct 2026; edited 6 Nov 2026 (56 series added) and 15 Nov 2026 (class 11 joins the context classes, §4); checked 16 Nov 2026 · drafted by Grok (SC1, no web) from 05, 07 and 08; checked by Claude. The first screen is at the end of March 2027, then every two months.*

## 1. PURPOSE

The screen is the two-month procedure that re-reads the blocker classes, appends each blocker's observation log, and orders a cross-map scan only for a class that moved. A full chain brief is prepared only for a chain whose blocker reading moved or whose dated event falls before the next screen, and a locked forecast whose date has passed resolves as 0 or 1 and is scored. The first screen runs at the end of March 2027, after the forecasts lock on 31 January 2027, and every screen after it follows this procedure.

## 2. INPUTS

**What to store.** Prices with no as-of date are stored at each screen, because the pages keep no archive. For every series below, store the figure, the unit, the fetch date, the page name, and whether the figure is a stock, a flow, a forecast, or a CALC, with numerator and denominator. Append the new line. Leave the previous line as it was. Where a page has no new print, store "no new print" and the last stored value. The four series that the blocker register says still need building have no page yet: the sub-10 kW roof file, the stall-book fee in rupees, the specialist's day, and the rupee eligibility file. Store "unbuilt" until a page is named. Round PS (6 Nov 2026) has since built a first reading for each of the four (08 §Round PS; listed under "Series added after 18 October 2026" below); the "unbuilt" rows in the panel are the 18 Oct 2026 baseline. The same store rule is applied here to the speech-watch pages. **Assumption:** those pages are stored like prices, because the files do not say they keep an archive.

The price panel is the set of posted prices. The class series overlap it. Each series is stored once. Comparison baselines for the first screen are the values below. Later screens compare with the latest stored line.

### Price panel

Latest panel date in the files: 17 October 2026, except where a row has its own date. Source pages are the product or institution named in the files. No row gives a URL.

| Series | Class | Source page | Unit | Last value in the files |
|---|---|---|---|---|
| OpenAI gpt-realtime-translate list price | 10 | OpenAI price page | USD per audio-minute | $0.034. Hourly one-way equivalent $2.04, CALC. Claude verified the page on 17 October 2026 |
| Wordly purchased low-stakes package | 10 | Wordly pages | USD per hour, CALC | about $150. Class series dates it 16 October 2026. One product, not the market |
| Call2Me two-way phone interpreter | 10 | Call2Me pages | USD per minute | Phone $0.33 ($19.80/h, CALC). Browser $0.25. Claude verified on 17 October 2026 |
| Bilingo two-way phone | 10 | Bilingo pages (page name only) | USD per minute | From $0.30 ($18/h, CALC) for US, MX and BR destinations. ID and TH at $0.45. Claude verified on 17 October 2026 |
| Google Cloud Translation NMT (control) | 10 | Google machine-translation list price | USD per million characters | $20. Same posted price in March 2014 and October 2026 |
| SolarAPP+ administration fee | 1 | SolarAPP+ (page name only) | USD per residential permit | $35. Non-AI template. The US rooftop file is already templated at this fee |
| DuraPlus Dutch heat-loss file | 1 | DuraPlus (page name only) | EUR per existing dwelling, incl. VAT | €157.30 |
| Pilot Essentials monthly close | 13 | Pilot (page name only) | USD per month | $99, for monthly expenses at or under $100,000 |
| Farmonaut Mini satellite advisory | 4 | Farmonaut (page name only) | USD per hectare-month | $1.00, from $4.99 for 5 ha. Minimum 5 ha |
| YouWish first water-based cosmetic formula | 3 | YouWish | EUR per formula, excl. VAT, a floor | from €619.42. Class series dates it 16 October 2026 and reads it quarterly. Cognitive slice 24.2% of that floor |
| Google Document AI Form Parser | 6 | Google Document AI | USD per 1,000 pages | $30 |

### Speech watch list

Re-read every screen, with the class 10 prices above.

| Series | Source page | Unit | Last value in the files |
|---|---|---|---|
| Output-language list | OpenAI price page | list of languages | Thai is not an output language on the cheap API or in Call2Me's list. The rest of the list is not printed in the files |
| WMT interpreting results | WMT | seconds of lag, plus similarity band | August 2026, general Spanish conference speech. gpt-realtime-translate inside the professional similarity band. Lag 5.3 s against 3.2 s for a human. The machine output was not expert-rated. An invented ending is documented. No numeric similarity score is stored |
| IWSLT interpreting results | IWSLT | not stated | No figure is stored in the files |
| Call2Me and Wordly pages | Call2Me pages and Wordly pages | as in the price panel | As in the price panel. WHO graded Wordly 1 of 90 at a 75% bar (2024). That grade is the last stored quality result on Wordly |
| Buyer-grade score for business calls | no page yet | score, if a page appears | No independent buyer-grade score exists for English with Brazilian Portuguese, Mexican Spanish, Indonesian, or Thai |
| Unassisted-English buyer screen | no single page named | whether buyers still require it | D01: where the buyer screens on an unassisted English test plus a US-client record, class 11 sits above class 10. No case of buyers dropping the screen is recorded |

The speech cap used as the margin is $37.50 an hour. Call2Me at $19.80/h and Bilingo from $18/h are already under it, as is the API at $2.04/h. The purchased card at about $150/h has not followed the API. Price is no longer the blocker. The stack now on record is quality, then trust and reliance (class 11), then latency, then privacy rules.

The draft forecast, for the lock, is P = 0.40 that by 30 June 2028 Call2Me's phone interpreter meets the stated bar for EN–ES or EN–PT. The reference is 0.36 (Nimdzi, November 2025, the share of providers expecting to deploy machine interpreting within a year). Using a different measure as the reference is marked UNCERTAIN in the files. The 24-call pilot is a design, not a series the screen runs.

Last deployment reading, stored with class 11 and opened only if a class 10 or class 11 scan is triggered: Krisp/AHS, vendor figures, 90% of calls stayed with the machine, 57% fully accurate on critical information, CSAT from 81% to 86%. Every deployment found keeps a human fallback. **Assumption:** this page is not on the every-screen watch list, so the screen does not re-fetch it unless that scan runs.

### Class series

The priority table says these are tracked every screen. Rows already in the price panel are stored once.

| Class | Series | Source page | Unit | Last value in the files | Print rhythm in the files |
|---|---|---|---|---|---|
| 1 | Berkeley Lab installed price and soft-cost share | Berkeley Lab | USD per watt, and a share of the residential price | Soft costs plus balance-of-system about 80% of the 2024 residential price, median $4.0/W. The 80% includes acquisition, labour, finance and profit. The cognitive slice is unpriced | Annual |
| 1 | IRENA installed cost | IRENA summary, read on a mirror; Claude re-checked the PDF | USD per kW, utility PV | $5,283 to $691/kW, 2010–2024 | Not stated as a screen rhythm |
| 1 | Posted permit or interconnection fee for a sub-10 kW roof | unbuilt | not set | No value. Closest stored posted fee is SolarAPP+ at $35 | To be built |
| 1 | Dutch heat-pump installed cost | page not named | EUR per installation | €6,800 to €4,800, 2023 Q1 – 2024 Q4 | Endpoints only |
| 10 | USD per purchased hour of commercial machine interpreting, and the NMT control | Wordly, Call2Me, Bilingo, Google NMT | as in the price panel | as in the price panel | Wordly marked quarterly in 08 (16 Oct 2026); now read at every screen |
| 13 | Billing cost per primary-care physician-year | page not named in these files | USD per physician-year | $99,581, 2018 anchor. Measured AI cut about $2,008 a year, 2.0% of that stack. Nabla −9.5% of note time is a stored cut, not this series | Anchor, not a live feed |
| 13 | Accountant's fee against a stall's monthly invoices | unbuilt | INR | No value | To be built |
| 4 | Specialist's day against one herd, one Sentinel tile, one lidar cloud | unbuilt | not set | No value | To be built |
| 4 | NHGRI genome cost (control) | NHGRI | USD per genome | $3,970 to $562, January 2015 – May 2022 | Historical endpoints |
| 3 | YouWish floor | YouWish | as in the price panel | from €619.42 excl. VAT | Quarterly |
| 3 | Weeks per part-number qualification | page not named | weeks | Last removal on record: re-certification onto already-qualified material, 5 weeks, −45% non-recurring cost. Reuse of the factory file €290. No separate current weeks reading is stored | Not stated |
| 6 | SVAMITVA loans ÷ cards | parliamentary answer | ratio | See the outcome series | At each parliamentary answer |
| 6 | UIDAI fee | page not named | INR | No separate figure. The last identity-check price stored in the class is e-KYC at ₹1–3 | Named, unnumbered |
| 6 | Rupee eligibility file | unbuilt | INR per file | No value | To be built |

Other class 3 levels stored as the stack, not as the quarterly series: K09 paperwork is 24% of the floor and €119 is the figure named as needed, on an order of about 124 units. Clinical evidence is €125,000–1.5 million per package, about €500,000 for a class IIa investigation (Commission SWD, December 2025). The one priced AI cut on that file is a vendor clinical-evaluation draft at $7,750 against €20,000+ for a human. In 8 of 8 held qualification chains the physical sample or test binds first. Round CT (3 Nov 2026) qualifies this for EU and UK electrical goods: the law asks for a self-declared assessment, so what binds is liability and the presumption of conformity that only the standard's test gives; statute requires the test only for US radio (08 §Round CT). Class 4's last cost share on the herd is about 4% of operating cost per cow. A stall under ₹40 lakh is exempt from GST registration, so class 7 sits above class 13 on that margin.

### Series added after 18 October 2026

Compiled 6 Nov 2026 from `08_Blocker_Register.md` by Gemini 3.8 Flash High (G02, `_grok_returns/PS_G02_answer.md`), de-duplicated by Claude; round PS added at the end. 56 series. The first screen stores each on the same rules as the panel above. "Verified" means Claude read the value on the page; * marks a class or unit Gemini marked UNCERTAIN. Dropped: the MS02 floor share (08:522). Corrected: the round SE £2,600 Wi-Fi line, now the £5,000 radio test.

| Class | Series | Unit | Last value | Value date | Verified by Claude | Where |
|---|---|---|---|---|---|---|
| 1 (file after fabrication) | HWE-Bench best-model fully correct schematic rate (arXiv 2603.18102) | share of 300 tasks | 8.15% | Mar 2026 | no | 08:299 |
| 1 | Human simple-board design file, for someone who can sketch (pintergabor.eu) | per design | €300 | undated | no | 08:300 |
| 11 | EquipBook remote machine write-up | per machine | $99 against a $500–700 field inspection | undated | no | 08:301 |
| 1* | 3Shape Automate crown price and acceptance | per crown / % acceptance* | $2.99 (90 s) / $1.99 (10 h), >94% | 26 Oct 2026 | yes | 08:336 |
| 1* | 3Shape human crown design | USD per crown* | from $5 | 26 Oct 2026 | yes | 08:337 |
| 1* | VerilogEval-Human v1 best pass@1 | pass@1 %* | 90.8% | Jun 2026 | no | 08:338 |
| 1* | PhIDO photonic end-to-end pass@1 | %* | 47% | undated | no | 08:339 |
| 1* | MUSE best-model manufacturability (named judge) | % manufacturable* | 48.58% (Gemini judge) / 66.98% (GPT judge) | undated | no | 08:340 |
| 1* | Socket shape error, median | mm | 1.24 mm | undated | no | 08:341 |
| 1 (or 5)* | Gene synthesis list price (Twist) | not stated | per Carlson, and the Twist list (the fabrication control) | undated | no | 08:342 |
| 8 (or 1)* | Photonic MPW shuttle cell | EUR per standard cell / half block* | VLC standard cell from €5,500; imec Passives+ half block €6,700 | undated | no | 08:343 |
| 1* | CADWorld (arXiv 2609.16251) | % of tasks (success rate) | 17.5% (against an 87.0% expert reference) | undated | yes | 08:362 |
| 1* | MUSE manufacturability | %* | about 67% for the best model | 28 Jun 2026 | no | 08:363 |
| 1* | Blueprint-Bench | score* | GPT-5 scores 0.431, against 0.547 for humans | undated | no | 08:364 |
| 1 (or 3)* | AutoImplant on real defects | Dice score and HD95 (mm) | Dice 0.63, HD95 6.32 mm | undated | no | 08:365 |
| 1* | Human-file control: the Lion's Tower miniature CAD | GBP per miniature | £400 per miniature | undated | no | 08:366 |
| 1* | Human-file control: advanced jewellery CAD | USD* | $1,200 | undated | no | 08:366 |
| 1* | Human-file control: SECalcs beam pack | GBP per pack | £300 per pack | undated | no | 08:366 |
| 1* | Human-file control: Metal Casting Development | USD* | $595–995 | undated | no | 08:366 |
| 15 (folded to 1 in round X) | CloudNC Quote Agent, per part quoted, human edit required | per part quoted | $2.50 (overage $3.75) | 28 Oct 2026 | yes | 08:425 |
| 15 (folded to 1 in round X) | Grant Hero, AI draft of an Innovate UK application | per application* | £175 | 22 May 2025 | no | 08:426 |
| 16 (provisional) | Easy Song custom licence, human paper | per job (up to 5 songs) | $399 per job (up to 5 songs) + 30% of publisher fees | undated | no | 08:427 |
| 18 (folded to 4 in round X) | Eldris map of 3 markets, human review included | per map* | £195 | 26 Sep 2026 | no | 08:428 |
| 18 (folded to 4 in round X) | Mangold device classification | per classification* | €98 unvalidated against €1,500 validated | undated | no | 08:429 |
| 18 (folded to 4 in round X) | Zonos Classify, HS codes | per month | from $500 a month (from $1,000 with confidence scores); 29.4% fewer errors than its previous model (vendor, 22 Sep 2026) | 22 Sep 2026 | no | 08:430 |
| 19 (folded to 8 in round X) | Lindy agent credits (send waits for approval) | per 1,000 credits | $10 per 1,000 credits | undated | no | 08:431 |
| 16 (or 7)* | works registered on the EUIPO Out-of-Commerce Works Portal | works | 2.7M | May 2026 | no | 08:483 |
| 16 (or 7)* | EUIPO Orphan Works Database works (control) | works | 7,597 | 5 Oct 2022 | no | 08:483 |
| 1* | Machining posted refusal | share of 40 suppliers | 19/40 = 47.5% (platforms 16/19, shops 3/21) | 30 Oct 2026 | no | 08:540 |
| 1 | Machining AI sketch-to-CAD offered | share of 40 suppliers | 0/40 | 30 Oct 2026 | no | 08:541 |
| 2 (or 8)* | UK repairs photo or remote quote | share of fixed UK sample | 3/15 = 20% | 30 Oct 2026 | no | 08:522, 542 |
| 2 (or 8)* | UK repairs median posted floor | GBP | £84 | 30 Oct 2026 | no | 08:522, 542 |
| 1* | Freelancer proposal count (depth gauge for human design route, sub-$100 design jobs) | proposals per job | 10–91 proposals each, on 8 pages | 1 Nov 2026 | no | 08:598 |
| 1* | MUSE joint success, best model (reliability gauge) | ratio | 61/106 | May 2026 version | yes | 08:601 |
| 1* | Cheapest posted human sketch-to-STEP for a simple part | USD per part* | $30 (Cad Crowd) | 1 Nov 2026 | yes | 08:602 |
| 1* | Cheapest posted AI file | USD per job / free tier* | Backflip Fast, about $2; QuantCAD free tier | 1 Nov 2026 | no | 08:603 |
| 1* | Instant-quote platforms offering automated sketch-to-CAD | ratio | 0/10 | 1 Nov 2026 | no | 08:604 |
| 1 | Protomolecule scan-to-CAD, simple part | GBP per part* | £55 | undated | yes | 08:641 |
| 1* | JLCPCB PCB layout minimum | US$ per job | US$100 per job | undated | yes | 08:642 |
| 1 (or 5)* | Checkatrade average UK metal staircase | GBP | £6,000 (ESTIMATE; not readable by Claude) | undated | no | 08:643 |
| 1* | Destatis new-dwelling construction prices | % y/y | +5.5% y/y | Aug 2026 | no | 08:644 |
| 1 (or 14)* | Tabletop Analytics pledged per tabletop project | USD per project | $45,094 | 2025 | no | 08:645 |
| 3* | CASS, single sample: EMC basic, battery device with no cables | GBP per single sample | £2,600 | undated | yes | 08:693 |
| 3* | CASS radio equipment testing (single sample) | GBP per single sample | £5,000 | undated | yes | 08:693 |
| 1* | Flux AI price per 1,000 design changes | USD per 1,000 design changes | about $330 | Oct 2026 | no | 08:695 |
| 3 (or 7)* | Germany, inspected products non-compliant, 2024 (EMC and radio) | share / % of inspected products | EMC 54.3% of 1,167; radio 69.9% of 1,297 | 2024 | yes | 08:759 |
| 3* | Signed cosmetic safety report, lowest posted (low-risk bar soap / CPSR) | GBP per report* | £75 | undated | yes | 08:760 |
| 1 | Tampa residential photovoltaic trade permit (human leg; SolarAPP+ is paid on top) | USD per permit | $120 | fetched 6 Nov 2026 | yes | 08 §Round PS |
| 13 | FilingBase Starter, books plus GSTR-1/3B, up to 100 transactions | INR per month + GST | ₹2,999 | fetched 6 Nov 2026 | yes | 08 §Round PS |
| 13 | HelloBooks Pro, AI, unlimited transactions, GSTR-1/3B | INR per month per entity + GST | ₹499 | fetched 6 Nov 2026 | yes | 08 §Round PS |
| 4 | Vision Research Park scouting, three visits a season | USD per acre per season | $2.75 | fetched 6 Nov 2026 | yes | 08 §Round PS |
| 4 | BIMIT 300 architect-assisted scan-to-model | USD per sq ft (floor) | from 27¢ | fetched 6 Nov 2026 | yes | 08 §Round PS |
| 4 | BIMIT 100 fully automated scan-to-model | USD per sq ft | 4¢ | fetched 6 Nov 2026 | yes | 08 §Round PS |
| 6 | Paper lines of a small loan file (e-KYC, CKYC, CIBIL ₹164, 13-year encumbrance certificate) | INR per file | ₹349.85 (UIDAI line unverified) | fetched 6 Nov 2026 | partly | 08 §Round PS |
| 6 | ICICI property valuation | INR per property | ₹2,500 | fetched 6 Nov 2026 (Grok) | no | 08 §Round PS |
| 6 | INK account-aggregator statement pull | INR per fetch, up to 7 months | ₹6.55 | fetched 6 Nov 2026 | yes | 08 §Round PS |

### Outcome series

| Series | Source page | Unit | Last value in the files | When it is re-read |
|---|---|---|---|---|
| SVAMITVA loans ÷ cards | parliamentary answer | loans over cards | 11,147 / 27,229,538 on 11 August 2026. The chain table rounds this to 11,147 loans on 27.2 million cards (0.04%). 8,808 of the 11,147 loans are in Rajasthan | Every screen: store the new answer, or "no new answer" |
| Locked forecast outcomes | the lock sheet of 31 January 2027 | 0 or 1 | No resolution is stored yet. Draft speech probability P = 0.40 by 30 June 2028, reference 0.36 | When that event's date has passed |
| K02 lot splits | page not named in the chain table | completed splits over eligible parcels | 25 completed of 6.1 million eligible parcels, to end-2023 | When K02 is read, not every screen |
| California accessory-dwelling permits | HCD handbook of March 2026 | permits | 1,336 (2016) to 30,354 (2024). Claude's own fetch hit a bot wall | When that class 1 or class 7 chain is read |
| Unattended shops in Sweden | class table, with Veckholm 2020 and Evansville 2021 | count of shops | 205 in 2023. Evansville population 632 | When a class 2 chain is read |

**Assumption on the clock page.** The mission keeps a clock page and five reverse-row indicators on the screen design, so they are inputs even though they sit outside the price panel. Scraped clocks named there: the Epoch fixed-capability series, DRAM, transformers, and interconnection. Epoch, 22 September 2026: about 47% a quarter (about 13× a year) since 2023; about 66% a quarter (about 75× a year) for a level just at the frontier; about 32% a quarter (about 4.7× a year) two years later. The vintage slowdown shows on three of five main benchmarks. This series is a clock, not a chain's price. GPU-hour: B200 at $7.83 against $4.75 on 13 October 2026. J3's lead trigger is an H100 30-day median below $2.60 plus a covenant or debt-service breach. On 14 October 2026 J3 was NOT FIRING, precursors only. No median is stored. Same-day dashboard: J1 EARLY, acceleration FAILS; J2 NOT FIRING; J4 EARLY; J5 NOT FIRING; J6 FIRING only inside the excluded set. DRAM has no number in these files. Interconnection has no number in these files. Reverse indicators: PC shipments and the sub-$500 forecast, no number; Raspberry Pi board price, no number; transformer lead times, step-up units above 160 weeks in Q1 2026; named sites Hawesville, Alcoa and Sauda, no figures; housing, no instance yet, with electrician pay on data-centre jobs as a labelled proxy and no pay figure stored.

## 3. STEPS

The first screen's date is 31 March 2027. **Assumption:** "end of March" means 31 March 2027, and the later 2027 screens fall on the last calendar day of May, July, September and November. The window opened on 1 February 2027, the day after the lock. A dated event on or before 31 March is resolved at this screen. A dated event after 31 March and on or before 31 May is briefed now and resolved at the May screen.

**Assumption on briefs.** The mission both asks Grok for a one-page brief per live chain and limits full briefs to a chain whose blocker reading moved or whose dated event falls before the next screen. The second rule is the one this procedure runs. Live chains are not briefed merely because they are live. The numerical cap of 12 is not used. The live set remains every chain whose crossing window falls inside the next eight quarters, with no maximum count. The pen is touched once a year. These files do not name the yearly month, so this screen does not read the pen except where a date below already pulls a chain in.

**Assumption on review dates.** A review date is a date to re-read. It becomes a kill only when the named complement window has passed and the constraint still binds, or the receipt is an AI product. The project owner makes that call. A small cost share is a grade.

Standing constraints on every Grok parcel: read-only web access; fetches identify the client generically; a timeout, a bot wall, or a curl 403 is an open gap. The scan question is written before the parcel returns. After the project owner adjudicates, Claude is the only writer: Claude appends the register line and the change log. Forecast lines are append-only.

1. **Re-read the panel.** Grok re-reads every price-panel series, every speech-watch item, every class series, and the SVAMITVA outcome, and stores the fields in §2. Parcel: one. Output: `_grok_returns/SC_2027-03_panel_answer.md`. ESTIMATE: one parcel, 705–948 seconds, the only parcel duration on record (the 14-parcel round of 16 October 2026). Applying that range to this parcel is an ESTIMATE.

2. **Clock page.** Grok re-reads the Epoch series, DRAM, transformers, interconnection, the J1–J6 readings, and the five reverse indicators. Parcel: one. Output: `_grok_returns/SC_2027-03_clock_answer.md`. ESTIMATE: one parcel, 705–948 seconds, on the same basis as step 1. A J reading stays on the clock page and is not copied onto a chain.

3. **Spot-check the two reading parcels.** Claude opens one source on the panel parcel and one source on the clock page, and checks the denominator of each figure those sources support. Claude does not re-fetch the parcel. Output: a spot-check note in `SC_2027-03.md`. ESTIMATE: no duration is recorded in the files. **Assumption:** each of these two parcels counts as one brief for the one-source rule. The source is taken from a series that moved, or from one load-bearing posted price if none moved.

4. **Log observations.** Claude drafts four lines for each blocker whose series was re-read: what we know, what we predicted, what we observed, and what worked. The predicted line is the locked line, quoted and dated, not a new probability. What worked records what removed the blocker, whether or not that was AI. As of 17 October 2026 the baseline is that AI had removed 0 of the marginal blockers. Output: the draft log in `SC_2027-03.md`. The append to `08_Blocker_Register.md` waits for step 12. ESTIMATE: no duration is recorded in the files.

5. **Check the chains in the window.** Claude lists every chain whose review date or forecast date falls inside the window, plus any chain whose class trigger in §4 has already fired on this reading. Killed chains are left off the list. For 31 March 2027 the date list is K07 (API, January 2027), D03 (review 17 December 2026), D16 (review 17 December 2026), G03 (review 31 January 2027), G01 and G04 (review 31 March 2027), D02 (review 31 March 2027), D13 (review 31 March 2027), D18 (review 31 March 2027), and D04 (review 17 April 2027, briefed because it falls before the May screen). **Assumption:** D03 and D16 are still open, because these files contain no resolution of them. K03 (January 2028), K08 (September 2027) and K09 (2027, no month) are not March briefs unless a trigger fired. Output: the chain list in `SC_2027-03.md`. ESTIMATE: no duration is recorded in the files.

6. **Write the briefs.** Grok writes one one-page brief per chain on that list. Seven parcels for this screen. Output: `_grok_returns/SC_2027-03_<chain>_answer.md` for each of K07, D02, D03, D04, D13, D16 and D18. ESTIMATE: seven parcels, 705–948 seconds each, on the same basis as step 1.

7. **Spot-check the briefs.** Claude opens one source per brief and checks the denominator. Output: one note per brief in `SC_2027-03.md`. ESTIMATE: no duration is recorded. The bound is one source and the denominator, not a second fetch. Seven checks at this screen.

8. **Rule the triggers.** Claude applies §4 to the stored values and writes, before any scan parcel, which classes get a full scan and which stay a reading. Output: the trigger block in `SC_2027-03.md`. ESTIMATE: no duration is recorded.

9. **Run the scans that tripped.** Grok runs one web scan per class that step 8 marked for a full scan. The scan prices the blocker, counts the margin, and records the stack for the industries on that class's cross-map. Parcel: one per tripped class, and none if step 8 tripped none. Output: `_grok_returns/SC_2027-03_class<nn>_answer.md`. ESTIMATE: 705–948 seconds per scan parcel. A full pass of the top six was about 6–10 parcels when it was done as a campaign. That campaign has already been run once, on 17 October 2026, so it is not repeated as the base screen. Claude then spot-checks one source and the denominator on each scan. ESTIMATE for that check: no duration is recorded.

10. **Adjudicate.** The project owner rules on each brief and each scan: the 0 or 1 for every locked forecast whose date has passed, any status change, any kill, any new chain accepted for a full record, and any rule change. A rule change is his, dated, and applied going forward. Output: his decisions written into `SC_2027-03.md`. ESTIMATE: 4–6 hours, the only adjudication figure in the files, from the capped quarterly design, and marked UNCERTAIN there. The files say the hours are measured on the first screen. This figure is replaced by that measurement. The December 2026 and March 2027 dates are in this sitting. D04 is briefed and is not resolved until May.

11. **Add the chains he accepted.** Grok builds one full chain record per candidate the project owner accepted. A candidate needs a sellable-quality price, a date, and a conjunction before it is built. The base screen accepts none in advance. Output: `_grok_returns/SC_2027-03_<new-id>_answer.md`, then Claude's one-source spot-check and denominator check. ESTIMATE: 705–948 seconds per accepted chain, and no duration for the spot-check. Zero parcels unless step 10 accepted one. The reference line for a new event is written before the parcel, with a source. A bare 0.5 is not a reference. An S4 chain gets one beneficiary line per fork.

12. **Resolve and score.** Claude writes 0 or 1 on each locked event whose date has passed, using the project owner's call, and scores only events that have a probability frozen on 31 January 2027. A review date with no locked probability is logged and is not scored. **Assumption:** the probabilities themselves live on the lock sheet, which these three files do not contain, apart from the speech draft P = 0.40. Brier is the mean squared error of the probability against the 0/1 outcome, and it is the score to show. The log score is the mean of o·log(p) + (1−o)·log(1−p). Skill is one minus the Brier score divided by the Brier score of the reference forecast frozen on the lock date. Calibration is reported by probability bin. **Assumption:** bins are 0.1 wide, because the files name bins and do not set the width. A raw hit rate is recorded and is not the test. **Assumption:** a hit means the locked probability and the outcome fall on the same side of 0.5. Lead time is the months between the date a locked probability first exceeded 0.7 and the date a public source names the same beneficiary. Lead time of zero means the map is late. If no scored event resolved, publish the probability mass placed on resolution by this screen date. Output: the score block in `SC_2027-03.md`. ESTIMATE: no duration is recorded.

13. **Publish.** Claude writes the screen report, appends the new lines to `07_Chain_Register.md` and `08_Blocker_Register.md`, appends each register's change log, and appends resolution lines to the lock sheet without editing locked lines. A nine-layer map is updated only if a status changed and only for a chain that is already one of the five. None of the five is a content tail. Killed rows stay on the register and are not re-read at the next screen. Output: `SC_2027-03.md`. ESTIMATE: no duration is recorded. **Assumption:** these file names are the protocol's names. The files do not yet name a screen report. Publishing means the report and the register appends exist in the project. No other channel is named.

Later screens repeat steps 1–13. The chain list in step 5 is the one in §7 for that month. The comparison baseline is the latest stored line, not the October 2026 column.

## 4. TRIGGER RULES

A full re-scan is a cross-map scan of every industry listed for that class, or a one-page chain brief. A reading is the stored series plus the four log lines, with no scan and no brief.

**Chains.** A chain gets a full brief if its review date or locked forecast date falls before the next screen, or if the class rule below fires for its binding blocker. Otherwise a live or held chain gets a reading only, through the class series already stored. A killed chain is not read. A pen chain is read at the yearly touch. It is briefed sooner if its complement date falls before that touch or before the next screen. A gate-failed row stays logged blocker data and is not briefed again. A later scan may look at the same industry.

**Classes 10, 4 and 3.** These get a full cross-map scan if any of the following is true against the last stored line. Otherwise they get a reading only.

- A posted price moves by more than 20%. **Assumption:** the files say the series "moves" and do not state a percent. Twenty percent is the threshold this procedure uses so the rule can be applied.
- AI's measured cut crosses the cut that chain needs. The chain's own distance field is the test. Where that distance is UNCERTAIN, a price move is not called a margin cross. For speech, the named cap is $37.50 an hour, and the purchased two-way products are already under it. A return of the purchased hour above $37.50, or a new measured quality result on one of the four unscored language pairs, is a move of the binding blocker.
- A statute, a fee, a licence, a buyer screen, or the output-language list changes. The language-list case is this procedure applying the rule-change trigger to the page the watch list names.
- The stack order at a margin changes. The order on record after a cognitive price crosses is quality, then trust and reliance, then latency, then privacy rules.
- Two consecutive trailing four-quarter log changes lie in the same direction. One quarterly print inside 20% is a reading only. The computation is the trailing four-quarter log change, the change in that change, and the change in the change. Raw third differences of quarterly prices are not used.

**Classes 1, 6 and 13.** The series are still read every screen. Class 1 is now a context class: no surviving chain in more than 190 cases with the whole order priced (08 §Round BF, §Round SE). **Assumption,** reconciling the two sentences in the blocker register: a price move, including a move of more than 20%, is logged and the stack is checked, and the cross-map is scanned only if the blocker above them has moved or the cognitive file is now the binding one. The later scan found the cognitive blocker on top in 0 of 35 industries in these classes. They matter when the blocker above them moves. Class 6's outcome is the loan ratio. Any new parliamentary answer is stored. The cross-map waits for the stack condition, or for a relative move of more than 20% in the ratio together with that stack condition.

**Classes 2, 5, 7, 8, 9, 11, 12 and 14.** These stay context. They are read when a chain in the window carries them, or when the blocker above a cognitive class moves. They get a full scan when a stack reorder puts them on top, or when their own non-AI unlock changes. Class 11 (trust and reliance) also gets a full scan when class 10 moves, since it sits directly above class 10 where a buyer keeps a screen (the project owner, 15 Nov 2026; spec 11 round LS, LS2-09). The 20% price rule applies where a posted series exists.

**Clock.** J3 is recorded as firing or not. A J verdict is never copied onto a chain. The complement-count series stays a design until four quarters exist, so it cannot by itself trip a scan.

## 5. OUTPUTS

### Screen report

File: `SC_2027-03.md`, and the same pattern for later screens.

```
# Screen report
## Window
## Series stored
## Observation log
## Chains checked
## Triggers
## Scans
## New chains
## Resolutions
## Scores
### Brier
### Log
### Skill
### Calibration
### Hit rate
### Lead time
### Probability mass
## Three outputs
## Adjudication
## Hours and tool budget
## Registers appended
```

The observation log uses the four lines: what we know, what we predicted, what we observed, what worked. The three outputs stay in that order: direct use excluded, diffusion as who captures now, and the find as new output plus the ecosystem. A content tail is never the delivered list.

### Registers

Claude appends, after adjudication:

- `08_Blocker_Register.md`: stored series, the four log lines, stack order, and any scan result. Its change log.
- `07_Chain_Register.md`: status, set, new chains, resolutions, and the counts. Its change log. Killed, failed, predates and second-book rows stay as separate counts from the in-book count.
- The lock sheet: new dated resolution lines only. Locked probabilities and dates are not edited.
- A nine-layer map, only on a status change, and only for a chain already among the five.
- The five reverse-row indicators, when the clock page has a new number. The housing row stays a labelled proxy until a housing series exists.
- The dashboard's J1–J6 lines, when the clock page has a new reading.

## 6. BUDGET

Tool use is budgeted per screen; the first screen records the parcel count and share used.

**Claude.** One source and the denominator per brief, and the same on the panel parcel, the clock page, and any scan. For March that is nine checks, plus one per scan and one per new chain. ESTIMATE: no hours are recorded for a spot check. Claude does not run a second full re-fetch.

**The project owner.** ESTIMATE: 4–6 hours for the March adjudication, the only figure in the files, marked UNCERTAIN there and estimated for a quarterly sitting of the older capped design. The first screen measures his hours and replaces this ESTIMATE. One owner-day a quarter is the binding constraint. In 2027 the third quarter has two screens, July and September, so those two sittings share that one owner-day. The measured March hours become the budget that later quarters are held to.

## 7. CALENDAR

Screen dates are the ends of March, May, July, September and November 2027. The lock on 31 January 2027 is not a screen. A month-only date is treated as passing on the last day of that month. A year-only date is not treated as 31 December. K09's EU and US border dates are written only as 2027, so each screen checks whether a day has been named and has passed, and the November report says so if the month is still unset. The speech CALC of about 11 months from 17 October 2026, if prices had followed the slow Epoch rate, is not a forecast date. The speech forecast date in the files is 30 June 2028. The October 2027 exam of thresholds and unlocks is in the mission, not as a chain date in the chain or blocker registers, and it falls between the September and November screens.

| Screen | Resolves, if still open | Briefs for the next screen | Does not resolve |
|---|---|---|---|
| 31 March 2027 | K07, API, January 2027. D03, review 17 December 2026. D16, review 17 December 2026. G03, review 31 January 2027. G01 and G04, review 31 March 2027. D02, review 31 March 2027. D13, review 31 March 2027. D18, review 31 March 2027 | D04, review 17 April 2027 | K08 (September 2027), K03 (January 2028), D14 (17 October 2027), D17 (31 December 2028), speech (30 June 2028) |
| 31 May 2027 | D04, review 17 April 2027 | G02, G05 and I02, review 30 June 2027 | The March set, already due earlier |
| 31 July 2027 | G02, G05 and I02, review 30 June 2027 | K08, card target, September 2027 | D14, which falls after this next-screen boundary |
| 30 September 2027 | K08, September 2027 | D14, review 17 October 2027 | K05 is not resolved here (the price has already crossed, per 08, so the 11-month CALC of the first-wave 07 text no longer applies) |
| 30 November 2027 | D14, review 17 October 2027 | K03, repair platform, January 2028. **Assumption:** the two-month cadence continues, so the next screen is the end of January 2028. These files stop the 2027 list at November | K09, unless a named day has passed. D17 and I04, 31 December 2028. Speech, 30 June 2028 |

Held chains with no review date in these files, and so with nothing to resolve in 2027 unless the lock sheet adds a date: D05, D10, D11, D12, C01, C04, G06, and the pen chains K01, K02, K04, K05, K06, K10, K11, K12 and K13. Failed rows are not on this calendar.

## 8. RISKS

**The pages keep no archive, so a missed store erases the move.** The guard is the store line at every screen, including "no new print" and "unbuilt". The first screen's baseline is the October 2026 column in §2.

**A small print is treated as a move, and the screen fills with scans until it is skipped.** The guard is the 20% rule and the two-consecutive-reading rule in §4. The parcel count is fixed before launch. The older uncapped reading was about 30 hours a quarter, which fails the one-owner-day constraint.

**A price that has already crossed is treated as the blocker lifting.** Speech is the case on record: the API and the purchased two-way products are under $37.50/h, and meaning on the call still binds, with class 11 above it where the buyer keeps an English screen. The guard is the stack order, and storing Call2Me, Bilingo and the API beside the $150 Wordly card.

**Classes that almost never sit on top are scanned in full every screen.** The guard is the narrower rule for classes 1, 6 and 13: read every screen, scan when the blocker above them moves or the cognitive file becomes the binding one.

**Passed dates are left open, or a review date is killed automatically.** D03 and D16 are dated 17 December 2026 and are easy to drop because they fall before the lock. The guard is the March list in §7. A kill still needs the named window to have passed with the constraint binding, or an AI receipt, and it needs the project owner's dated decision. The row then stays and is not re-read.

**Forecasts are edited, or a bare 0.5 becomes the reference.** The guard is append-only lines, the reference frozen on 31 January 2027, and Claude as the only writer after adjudication. If the lock sheet is missing on 31 March, the series are still stored and nothing is scored.

**Nothing has resolved, and a hit rate of zero is reported as the result.** The guard is the probability mass on resolution by that date. A high probability that misses scores worse than a low probability that is still waiting. The hit rate is recorded and is not the test. The eight-quarter intermediary test is not on the 2027 exam. Complement counts wait until four quarters exist.

**The third quarter spends the owner-day twice and the later screens are dropped.** July and September both fall in that quarter. The guard is to measure March hours, parcel count and tool budget in the report, and to hold later quarters to that measurement and to one owner-day. New-chain builds are the first work dropped if the second sitting does not fit.

**An unchecked page or a blocked fetch enters the score.** The guard is one opened source per brief and the denominator. A timeout, a bot wall, or a curl 403 stays an open gap. An Argon-sourced row is not used until a person or a second auditor has opened the cited page. Fetch headers carry no personal data.