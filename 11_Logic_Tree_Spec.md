# Logic tree: where AI could enable, industry by industry

*v0.4.0 · 15 Nov 2026 · Claude (Opus 5.5), supervisor. v0.3 applies the project owner's seven rulings of 8 Nov (§10, Q1–Q7; Q7 was ruled in chat the same day) and replaces the grid with the revised 25 × 12 grid from round GR (§2.1, §3). v0.3.1–v0.3.4 add the rule fixes from the two-coder test (§9 step 0) and the recall test (§9 step 1), and the Q7 ruling. v0.3.5 adds the 13 fixes found in pilot phases P1–P3, v0.3.6 the 7 found in P4, v0.3.7 three tie-break fixes from the third two-coder sample (RT3), v0.3.8 four rulings after RT4 and the consistency review (round LS), v0.3.9 three stage defaults after RT5, and v0.4.0 the rulings and fixes from round LS and HY1 (rule gaps G1–G8, 10 rulings, 30 fixes). See §12. Status: RULED. The 61 chains are coded; the health pilot (§9) started on 8 Nov 2026.*

**Why this exists.** Every case so far was found bottom-up, by scans that started from a blocker class or a lead (07, 08). There is no map that decomposes each industry along its full supply and value chain and asks, step by step, whether AI or an LLM agent could matter there at all. So there is no denominator per industry, no record of what was never looked at, and no way for a new agent to know where to dig next. The project owner raised this on 7 Nov 2026.

**How this spec was made.** Two independent designs from the same brief (`_parcels/logic_tree/design_brief.md`):
- design A: Gemini 3.8 Flash High, `_grok_returns/LT_FLASH.md`;
- design B: Claude Sonnet, `_grok_returns/LT_SONNET.md`.

Then:
- an adversarial review of both with a data-feasibility check on the web: Grok 4.7, `_grok_returns/LT_K1_answer.md`, 20 of 22 fetches succeeded;
- a landscape survey of existing frameworks and measures: Gemini 4 Argon, `_grok_returns/LT_ARGON.json`, 40 rows plus a debate map.

Claude spot-checked 2 of Grok's quotes and the 7 Argon quotes this spec relies on. All 9 were verbatim on the live page. The other 33 Argon rows are leads, under the Argon rule (04).

---

## 0. For a new agent: read this first

1. The project's question is in 05 §1. The tests that decide whether something counts are the three gates in 05 §4. This tree does not change them.
2. The tree has **two halves**. Read both before you expand anything.
   - **The grid** (§2–§5): industries → stages → activities → priced cost lines. It shows where cost sits, what blocks, and what has and has not been examined. **It is a coverage map, not the search.**
   - **The demand side** (§6): the parties who are *out* today (buyers, entrants, places), and the **trade records** that would serve them. **This is the search.** A trade record need not have an industry parent.
3. The single most important rule is in §5. **Write the whole blocker stack before you decide anything about AI.** A node AI cannot touch is often the one that binds. It is never closed for that reason.
4. Every number carries its numerator, denominator, date and kind (05 §5.13). Where you have no number, write `null` and a fill plan. Never substitute an industry average for the marginal buyer's order.
5. You may propose a chain or a trade record. You may not write a gate verdict. The supervisor does that, and the project owner adjudicates. A kill or deletion needs the project owner's dated ruling (05 §7.6).

---

## 1. What we learned building this (the evidence behind the design)

| Finding | Source | Consequence for the design |
|---|---|---|
| No published method combines an industry taxonomy, a process tree, task exposure and step-level cost share. The literature has two separate silos: industry → occupation → task → wage bill, and enterprise process frameworks with no exposure or public cost. | Argon gaps §1–3; Grok data table | We build the join ourselves. The bridges must be labelled as our construction, not as data. |
| Public input-output tables give purchased-input shares by industry: BEA 71 industries a year and 402 in benchmark years, Eurostat 64 NACE activities. They do not split an industry by stage or activity. | Grok, BEA and Eurostat pages (BEA quote verified by Claude) | Industry shares stop at L1. Below L1, cost comes from posted prices, fee schedules and cost studies. |
| No public source gives **the marginal buyer's whole order**. | Grok data table | That share is filled the way 08 already does it, from posted prices. It is the only share that can grade a chain. |
| O*NET has about 18,800 task statements, each tied to one occupation, with no price or time share. BLS OEWS staffing patterns weight occupations within an industry, but leave out the self-employed. | Grok; O*NET quote verified by Claude | Task lists are a checklist for L3 activities in incumbents. They cannot find a party who is out. |
| Exposure measures (Eloundou et al.; ILO WP96; Anthropic Economic Index; Microsoft "Working with AI") score whether AI could touch an incumbent's task. Their own authors say exposure is not deployment. ILO: the analysis "does not take into account the new jobs that will be created". | Grok; Argon | Exposure is a prior only. It never decides whether a node is expanded or closed. |
| Cost-effectiveness changes the picture. MIT FutureTech (Svanberg et al., 2024): "at today's costs U.S. businesses would choose not to automate most vision tasks that have 'AI Exposure'". | Argon row, verified by Claude | Exposure needs a third field: AI's price at sellable quality against the buyer's price (§4). |
| Baumol bottleneck (Aghion, Jones & Jones): "growth may be constrained not by what we are good at but rather by what is essential and yet hard to improve". | Argon row, verified by Claude | This is the economics behind our stack law (08). The binding node is the hard-to-improve one. |
| AI-powered growth "concentrates among larger firms and is associated with higher industry concentration" (Babina et al., JFE 2024). On freelance platforms, ChatGPT lets incumbent freelancers enter programming tasks (Liu et al.). | Argon rows, verified by Claude | The prior evidence on entry favours incumbents. Enablement by a new entrant is the contested claim, not the default. |
| Our own corpus is lopsided. On design A's coding, design (53) and support (34) hold 87 of 159 cases. On design B's coding, 59 of 324 industry × stage cells hold any case (18.2%) and 26 hold a held or emerging chain (8.0%). Sourcing, logistics and after-sale are nearly empty. | A and B coverage sections; denominators as stated | The pilot must show what is in the empty stages, or say why they are empty. |
| Both designs, as written, closed the node holding the binding blocker: A on infill housing, B on clinic billing. | Grok attack, §ATTACK A(b), B(b) | Descent rule in §5: stack first, and no closure on "no AI channel" or on cost share. |

---

## 2. The grid: levels

| Level | Unit | Count | Rests on | Share that can be filled here |
|---|---|---|---|---|
| L0 | Economy | 1 | — | — |
| L1 | **Industry system**: ISIC classes sharing one buyer-facing chain | 25 plus an out-of-scope bucket (§2.1) | defined on ISIC Rev.5 / NACE Rev.2.1; filled through ISIC Rev.4 / NACE Rev.2 tables | industry share of purchased inputs, from input-output tables (BEA, OECD ICIO, Eurostat FIGARO) |
| L2 | **Stage**: one of 12 fixed stages, by the job a line does in one order (§3) | 12 per L1, 300 cells; a stage can be `STAGE_ABSENT` | the life of one order, REACH to ASSURE (round GR, Opus design); SCOR and APQC as checks | usually null; a cost study where one exists |
| L3 | **Activity** within a stage of that industry, named by the work, not by the provider (§7 step 3) | up to 12 per cell, not counting protected lines; a tail goes in an "other" node under 10%, or is split; a protected line (§5) is never put in "other" | industry process frameworks where they exist (SCOR, eTOM, BIAN, ACORD, ISA-95, RIBA Plan of Work, OECD System of Health Accounts: its functions only at SPECIFY, MAKE, MOVE and DELIVER), ISIC 4-digit, O*NET tasks | wage bill × hours, cost studies, fee schedules |
| L4 | **Cost line**: the smallest item in a **marginal buyer's or entrant's whole order**, priced or not, where a blocker can be named (an unpriced line is tagged `unpriced`, §5 step 3) | 3–8 per expanded L3 | posted prices, statutory fees, unit-cost studies, the project's own records | **share of the marginal order** (the grading share) |
| — | **Blocker stack, chain, case**: records attached to an L4 node | — | 07, 08 | — |

### 2.1 The 25 industry systems (ruled by the project owner, 8 Nov 2026, Q2)

**Classification.** The grid is defined on ISIC Rev.5 (NACE Rev.2.1 in the EU). It is filled through tables still on ISIC Rev.4 / NACE Rev.2: EU supply-use and input-output transmissions move to NACE Rev.2.1 only "from September 2029" (Regulation (EU) 2023/137, Art. 2(2)(k), on Annex B of Regulation 549/2013). So each system carries both codes. The Rev.4 column is the fill route; where Rev.5 split or moved a class, the mapping is lossy and the node says so. Source and checks: `research/tree/GR_grouping_review_2026-11-08.md`.

| Code | System | ISIC Rev.5 | Filled through (Rev.4 / NACE Rev.2) |
|---|---|---|---|
| AGR | Agriculture, forestry, fishing | A 01–03 | A 01–03 |
| MIN | Mining and quarrying | B 05–09 | B 05–09 |
| FOOD | Food, beverages, tobacco | C 10–12 | C 10–12 |
| LITE | Light consumer goods | C 13–15, 18, 31–32 (excluding 3250) | C 13–15, 18, 31–32 |
| CHEM | Chemicals and pharmaceuticals | C 20–21 | C 20–21 |
| MATL | Process materials and fuels | C 16–17, 19, 23–24 | C 16–17, 19, 23–24 |
| PART | Made-to-order parts, moulding and repair of machinery | C 22, 25, 33 | C 22, 25, 33 |
| EQPT | Machinery, equipment, vehicles and devices | C 26 (semiconductor making goes to OUT), 27–30, 3250 | C 26 excluding 2610 semiconductor part, 27–30, 3250 |
| ENER | Energy supply | D 35 | D 35 |
| WATR | Water, waste and recycling | E 36–39 | E 36–39 |
| CONS | Construction | F 41–43 | F 41–43 |
| TRADE | Wholesale and retail, including 4790 retail intermediation and 4772 pharmacies | G 46–47 | G 45 (sale), 46–47 |
| TRAN | Transport, storage, post | H 49–53 | H 49–53 |
| HOSP | Accommodation and food service | I 55–56 | I 55–56 |
| MEDIA | Publishing, audiovisual, content distribution | J 58–60 | J 58–60 |
| ICT | Telecoms, IT and information services | K 61, 62, 6390 | J 61–62, 639 |
| FIN | Finance and insurance | L 64–66 | K 64–66 |
| REAL | Real estate (imputed owner-occupied rent is a denominator only, never a searchable market) | M 68 | L 68 |
| PROF | Professional, scientific, technical | N 69–75 | M 69–75 |
| ADMIN | Administrative and support | O 77–82 | N 77–82 |
| PUB | Public administration and defence | P 84 | O 84 |
| EDU | Education | Q 85 | P 85 |
| HLTH | Health and social care | R 86–88 | Q 86–88 |
| ARTS | Arts, sports, recreation | S 90–93 | R 90–93 |
| PERS | Personal and household services, repair of personal goods and motor vehicles, households as employers | T 94–96, U 97–98 | S 94–96, G 4520, T 97–98 |
| OUT | Out of scope as a subject: the AI build-out stack and extraterritorial bodies | K 6310; semiconductor making within C 2619; AI model developers (firm rule); V 99 | J 6311; C 2610, semiconductor part (NACE Rev.2 26.11); U 99 |

**Rules:**
- An ISIC Rev.5 class belongs to one system only. Imputed rent stays in REAL's size, not in its search.
- OUT is not searched. A case closes with `OUT_OF_SCOPE` only when its own subject product is in OUT, or its excluded party is a public body using AI on its own papers (§5 step 1). An OUT supplier line inside another case's order is allowed: a firm buying a custom chip for its own non-AI product is coded on that product (TB1c), and the chip is a line with `l1` OUT. An OUT line keeps its stage, is priced like any other line, and is never expanded or searched; neither §5 step 1 nor §7 step 1 closes it (round RC: I05's rank-1 shuttle line). The AI supply chain otherwise appears only as a `reverse` flag on input nodes (05 §3.8).
- **The ISIC class decides, not the system's name.** A coder writes the subject's 4-digit ISIC Rev.5 class (`isic5`) first; the system follows from the table above. Round TC: 5 of 12 system disagreements followed a label ("personal and household services", "made-to-order parts") rather than a class: D04, D11, D18, N06, N09.
- **A case's system** is the system of the output the excluded party wants to end up with (TB1, §3). For an infrastructure episode (canal, railway, grid, fibre), the subject is the enabled business; the network is a supplier line. This holds when the margin is the enabled business. Where the margin names the firm that builds or sells the network, TB1e decides (round LS, LS1-11).
- **Cross-industry services** (finance, carriage, retail, bookkeeping, certification, platforms, the state) are a case's system only when the excluded party wants that service itself. Everywhere else they are order lines, with their own system as `l1` and a default stage (§3). They are linked by `supplier_of` and `buyer_in`. **Shares are never added across a link.**
- **Purpose tag on every case.** Each case and E record carries:
  - `purpose`: the COICOP 2018 division of the household need the output finally serves, or the COFOG division when the final buyer is government, or `MULTI` for an intermediate input with no single final purpose (and for unnamed retail goods, G8 below);
  - `use`: household final, government final, fixed capital (GFCF), or intermediate.
  For an intermediate or GFCF output, `purpose` is a COICOP or COFOG division only when the output serves one final purpose (a part made only for medical devices is 06); otherwise `MULTI`. Round TC: 10 of 13 purpose disagreements were one coder tracing an intermediate to a final purpose and the other writing `MULTI`.
  Four defaults for purpose and use (rule gap G8; the project owner, 15 Nov 2026):
  - household heat (ENER 3530) is `HH_FINAL`, COICOP 04;
  - a medical device sold to a provider is `INTERMEDIATE`, with purpose COICOP 06;
  - a finished device with no buyer named is `MULTI`, use `GFCF`;
  - unnamed retail goods that households buy across several COICOP divisions, none named, are purpose `MULTI` with use `HH_FINAL`. This is the one case where `MULTI` is not an intermediate input.
  A health, housing or mobility view is a re-cut of the tree by purpose across systems, never a carve-out of classes into one system.
- The project's ten case groups (07/08 JSON `industry_group`) are retired as a level. "Regulated goods & compliance" is two stages (PERMIT, QUALIFY), not an industry (design B finding: 9 of its 11 rows sit at the approval stage).

---

## 3. The 12 stages (L2; ruled by the project owner, 8 Nov 2026, Q2)

The stages follow the life of one order. Every system has all 12 stage nodes, so every industry compares 12 columns against 12. A stage node is `STAGE_ABSENT` only where no protected line sits in it (§5 step 2). Each adjacent pair is split because different blocker classes bind on each side (round GR, Opus design).

| Code | Stage | The question it answers for this order | Blocker classes expected (08; folded classes with their host) |
|---|---|---|---|
| REACH | Reach | Can buyer and seller find each other at a cost the order carries? (listing, advertising, marketplace or channel fee; an outlet's catchment is DELIVER, G7) | 14; 8 (density, with folded 19) |
| ENGAGE | Engage | Will this buyer accept this seller and agree terms before any work? (sales call, the buyer's screen of the supplier, interview, quote or bid, contract) | 10; 11 (the screen); 1 via folded 15 (bid cost) |
| SPECIFY | Specify | What exactly is to be made or done? (survey, diagnosis, data interpretation, design, CAD file, engineering calculation, regulatory scoping) | 1 (the drawing half of the file); 4 (with folded 18) |
| PERMIT | Permit | May this operator, site or installation go ahead? (licence, planning or building permit, registration, statutory fee, grant condition, licensing of persons, interconnection application) | 7; 1 (the approval half of the file) |
| QUALIFY | Qualify | May this product, part or formula be sold? (sample, test, certificate, safety assessment, notified-body review, declaration of conformity) | 3; 11 when presumption of conformity attaches to a named maker |
| FINANCE | Finance | Can the order be paid for before it pays back? (credit, equity, working capital, quick-pay, grant or subsidy) | 6 (with part of folded 20) |
| SOURCE | Source | Can inputs be had in the needed shape, size and price? (materials, components, energy blocks, land or premises, rights, equipment) | 12; 16; 5 when the minimum is on an input (materials, components, a material lot); inputs the build-out makes dearer |
| MAKE | Make | Can it be made, or the service produced away from the user, at this batch size? (tooling, set-up, fabrication, building on site, content production, back office) | 5 (a minimum on making the subject's own product, in-house or by a contract maker); 2 via folded 17 (operator know-how) |
| MOVE | Move | Can it get from where it is made to where it is used? (freight, storage, cold chain, customs and duty, network transmission and connection) | 8 (route density); 7 (duties, border); 12 (network capacity) |
| DELIVER | Deliver | Can it be handed over and used at the point of use? (installation, site visit, staffed outlet, live service, last-metre labour, after-sale visit) | 2; 9; 8 (outlet catchment); 10 when the speech is the service |
| SETTLE | Settle | Can the order be paid, invoiced, booked, filed and claimed each period? | 13; 7 (tax statutes) |
| ASSURE | Assure | Who pays if it goes wrong, and can the right be enforced? (warranty, indemnity, insurance, escrow, venue, returns, enforcement) | 11 (recourse); 6 and folded 20 (enforcement) |

**Reading rules** (one stage set for goods, services, networks and public services, no variants):
- **MAKE or DELIVER.** MAKE is work that could happen away from the user. DELIVER is anything that must happen at the user's site or in the user's presence. Exception: building a structure whose site is the product is MAKE. Remote work takes the same test: asynchronous work done away from the user (a teleradiology read, a lab test) is MAKE; a synchronous remote session the user takes part in (a video consultation) is DELIVER (pilot P1c).
- **SPECIFY is a job, not a place.** Diagnosis, assessment and care or treatment planning are SPECIFY wherever they happen, in the user's presence or not. The examination time itself is DELIVER (pilot P1c).
- **Premises against accommodation.** The lease or purchase of premises is SOURCE (REAL). Boarding provided to the user as part of the service (a care home's room and meals, given with the care) is DELIVER in the subject's system (pilot P1c).
- **A cross-cutting service as the subject** uses its own chain. Lending: SPECIFY is the credit assessment, FINANCE the lender's own funding, MAKE the documentation and decision, ASSURE default and enforcement. Haulage: MAKE is the haul. Retail: MAKE is the outlet fit-out, DELIVER the staffed selling hours.
- **Public services:** FINANCE is the budget or grant, SETTLE the benefit or fee payment, ASSURE appeal and redress.
- **Networks:** MOVE is transmission and distribution, including the connection; DELIVER is metering and use at the premises.
- **Capital.** Capital that is tooling or plant for making the product → MAKE (class 5). The buyer's outlay, or a buyer of a business → FINANCE (class 6) (rule gap G6; the project owner, 14 Nov 2026).
- **Outlet catchment** (class 8) → DELIVER (rule gap G7; the project owner, 14 Nov 2026).

**Placement rule.**
1. Name the excluded party and the subject product. Entrant: what it would sell. Buyer: what it would end up with. Place: the product missing there.
2. Write the 4-digit ISIC Rev.5 class that produces the subject product (`isic5`). The case's system follows from the §2.1 table (TB1). Where the case names no product, `isic5` is null and the system is TRADE (TB1b). For a reseller, `isic5` is the reseller's own class and the goods class goes in `isic5_goods`.
3. List the order lines. Entrant: its costs for the first marginal unit or period. Buyer: everything it must buy to get the product into use. Place: list it as an Entrant, with the costs of a supplier who would sell the missing product there.
4. Each line's `l1` is the system of the industry that supplies it. The party's own labour takes the subject's system, even where the same work bought in has another home: a practice's own billing staff is HLTH, billing bought from a firm is PROF. The line records which in `supply: OWN|BOUGHT` (pilot P1a, K07). A statute or state charge takes PUB.
5. Each line's stage is the job the line does in the subject's chain, judged by the stage questions above, whoever supplies it.
6. The binding line is the line whose removal would admit the party. Where several lines must all be removed before the party is admitted, each is rank 1 (TB3, §5 step 3). Two exceptions, both in TB3: a stated order makes only the first-named line rank 1 (a comma list before 'then' is a joint tier, G2), unless the record says the lines bind together or prices them as one gap; and a gap pair is two rank-1 lines although moving either one would admit the party (round LS, LS1-01, LS1-02).

**Tie-breaks.**
- **TB1 (case system).** Classify by the output the excluded party wants to end up with, not by the firm that sells the bundle (own-generated rooftop power is ENER, not the installer's CONS). The same holds beyond electricity: a household's own heat → system ENER; storage, chargers and shops → EQPT (rule gap G1; the project owner, 14 Nov 2026). For an infrastructure episode, the subject is the enabled business and the network is a supplier line, when the margin is the enabled business; where the margin names the firm that builds or sells the network, TB1e decides (round LS, LS1-11). Four sub-rules, added after round TC:
  - **TB1a, parts.** A part specially designed for one kind of product is classed with that product, as ISIC does (railway parts 3020, bicycle parts 3092, motor-vehicle parts 2930). A general-purpose part is classed by process: plastics C 22, fabricated metal C 25. Casting of metals is C 243 (MATL).
  - **TB1b, resellers.** A party that resells goods made by others under their brand (importer, wholesaler, retailer, marketplace seller of others' goods), or whose case names no product at all, is TRADE. The goods' class is recorded as `isic5_goods`. A brand that designs its product and has it made under contract, and a seller whose own product is named, are coded on the product. A private party selling its own used item is not a reseller: code the item (D08, G03, S04-10).
  - **TB1c, buying an input to sell a product.** A party that buys an input in order to sell its own product is an entrant: code its product, and the input is an order line under the input's own system (OUT included).
  - **TB1d, the state.** The case's system is PUB when the excluded party is a public body, or wants the state service itself (a court, a registry). Otherwise the state is a supplier line (PUB) or a `rule` edge (round LS, LS1-10).
  - **TB1e, who the subject is.** The subject is the party the case's margin names. If the margin names an installer or seller, code what it sells (a firm that builds or sells a network included); the rooftop-power example above applies only when the margin is the household (round RT, J02-12). **Where a row names two parties** (an author and a publisher, a herder and a lender, a maker and a reseller), the subject is the party the margin names as kept out. If the margin names neither as kept out, the subject is the party that would sell the new product (round RT4; the project owner, 12 Nov 2026).
- **Not a case.** A row that names no excluded party and no product (a method row, a novelty attack on a class) is `NOT_A_CASE`. It is not coded and is counted separately in every denominator (round RT, X02-15). A row that names a party but no product is TRADE (TB1b), not `NOT_A_CASE`; a row that names a product but no party is coded on the product, with the party written as the E record of §5 step 3 (round LS, LS1-12, LS4-09). A method alone is `NOT_A_CASE`; a row that names a product is coded (rule gap G5; the project owner, 14 Nov 2026).
- **TB2 (a line that does two jobs).** A document an authority requires before an operator, site or person may go ahead → PERMIT; a document an authority requires before a product may be sold (a technical file, a certificate, a clinical evaluation) → QUALIFY; a document the producer needs anyway → SPECIFY. Licensing, registration or clinical privileging of a person or site → PERMIT; accreditation of a service offered for sale (ISO 15189 for a lab test) → QUALIFY (pilot P1a, D12; P1c). Speech or a screen before the contract → ENGAGE; speech that is the service → DELIVER. A statute sits at the line it creates or prices: a licence → PERMIT, a duty → MOVE, a tax return → SETTLE, a staffing floor → DELIVER. **Every statute is one `rule` record (§3, 'Statutes are edges'). A statute that charges a fee or requires a filing, test or registration also has its own line, linked to the record; otherwise it is only a `rule` edge on the line it prices, at that line's stage** (round TC, G06; round LS, LS1-09). A stack entry for such a statute points at the line it prices (round RC). **A statute that bans** a line while a condition holds is neither kind (MDR Art. 5(5)(c): a hospital may not make a device in-house while an equivalent device is on the market). It is a `rule` edge on the line it forbids, with `rule_bans: true`, and a stack entry for it points at that line. No price removes it; only a change to the statute or to the condition does (pilot P4, N04). A buyer's refusal before contract → ENGAGE; the cost of recourse after delivery → ASSURE. **A test or inspection** that licenses a person or a site → PERMIT; one the buyer or a rule requires on a product or a lot before acceptance → QUALIFY; the same step as part of the producer's own process, with no buyer or rule requiring it → MAKE (the project owner, 12 Nov 2026). **A bought input** (a subscription, a spare part) → SOURCE, unless a statute makes it a condition of going ahead (→ PERMIT) (round RT3). **Hired labour and a licence priced by tariff** take the stage of the job they do and the issuer: an authority's licence → PERMIT, a private right → SOURCE, hired labour → the stage of the work, a staffing floor → DELIVER (round LS, LS1-07). **A minimum** (class 5) follows what is bought, not who does the work: a minimum on making the subject's own product, in-house or by a contract maker, → MAKE; a minimum on an input that goes into the making → SOURCE. **A right or consent** obtained from a private holder (class 16), with the search for whom to ask, → SOURCE; a licence an authority grants → PERMIT. **Tax** registration and tax returns → SETTLE; an exemption or a threshold is a `rule` edge on the filing line it switches off, at SETTLE; a registration is PERMIT only where it is a condition of trading at all (a trade licence) (RT5; the project owner, 12 Nov 2026).
- **TB3 (lines bind jointly).** Record every one as rank 1. **Where the case record states an order** ('capital first, then the permit'), the first-named line is rank 1 and the summary stage, and the others are STACKED_BELOW. **A comma list before 'then'** is one joint tier, not an order: each line named in it is rank 1, not the first-named line only (rule gap G2; the project owner, 14 Nov 2026). Joint rank 1 otherwise applies only where the record says the lines bind together, or prices them as one gap. Where a single summary stage is needed for joint rank-1 lines, take the largest priced gap; if none is priced, the line the case record names first (round RT3). **A gap pair** is two lines that bind on the gap between them, so that moving either one would admit the party: what one line brings in against what another costs (K07: a panel of members at REACH against the physician year at DELIVER). Both are rank 1, each stack entry names the other in `gap_pair`, and the gap is priced as what closes it (members × fee against the year's cost) in `gap_price`. Its summary stage is the line with the larger priced amount; if neither is priced, the line the case record names first (the joint-line rule; round LS, LS1-03; pilot P4, K07, K13).
- **TB4 (the case record names no binding line).** Use the line where the cost fell, and flag the case as ambiguous (round LS, LS1-06). **On a row whose blocker has already been removed** (a context case: the cost fell and the party is in), the summary stage is the stage of the removed line, and the row is tagged `context`. The removed line is not rank 1. The next line that still binds, where the record names one, is rank 1; where it names none, the row has no rank-1 line. On a context row the summary stage may therefore lie outside the rank-1 stages. This is the coding-side form of the `admitted` rule (§5 step 3: the removed line is not `BINDING`, and a blocker that still stands is) (round RT3; the project owner, 12 Nov 2026). A context row is allowed where the row names no party; it is still coded and tagged `context` (rule gap G4; the project owner, 14 Nov 2026). **Missing uptake is an outcome, not a line.** Code the cause the row names (a consent, a price, a rule); if it names none, the cause is buyers not finding or not accepting the offer, and the stage is REACH (rule gap G3; the project owner, 14 Nov 2026), flagged ambiguous (RT5, C-2; the project owner, 12 Nov 2026).

**Default homes of cross-cutting services** (when they are a line, not the subject):

| Service | `l1` | Stage |
|---|---|---|
| Credit, grants | FIN, PUB | FINANCE |
| Insurance and guarantees | FIN | ASSURE |
| Payments | FIN | SETTLE |
| Carriage, storage, customs brokerage | TRAN | MOVE |
| Marketplace and retail channel fees | TRADE | REACH |
| Bookkeeping and tax filing | PROF | SETTLE |
| Testing and certification | PROF | QUALIFY |
| Advertising and social platforms | PROF (73) or MEDIA | REACH |
| The state: licences and permits / taxes / customs / courts / subsidies | PUB | PERMIT / SETTLE / MOVE / ASSURE / FINANCE |

**No double counting.** Each line appears once in the order, at one (system, stage) cell; a cost supplied by two systems is split into one line per supplier (round RC: K02's grid and water connection). A service's own chain is never expanded inside another case; if the binding line lies inside the service (K08: the bank's remedy), the case is re-run with the service as subject and the two are linked. A purchaser's price is split the way a supply-use table values it: basic price, trade margin, transport margin, taxes less subsidies, each its own line. Lines with no table row (the party's own hours, waiting time, a grant condition, a missing counterparty) are kept; the binding line is often one of them.

**Statutes are edges, not a stage.** A statute or standard is recorded once, as a `rule` record, and linked by a `rule` edge to every line whose price it sets (R4, L16). The old B4 stage held 1 of 153 cases.

**A platform, pool, servicer or certifier is not a stage.** If it is the business that would exist, it is a trade record (§6, layers 4–6 of the nine-layer map). If it already exists and serves the buyer, it is a line at the stage it serves.

---

## 4. Node fields

Every grid node carries the same record. The JSON schema is in §8.

- **Identity:** id, level, parent, industry, stage, name, taxonomy code, definition.
- **Two shares, never merged:**
  - `share.of_industry_cost`, filled from input-output tables, L1 only;
  - `share.of_marginal_order`, filled from posted prices.

  Each carries `value`, `kind`, `num` (numerator), `den` (denominator), `year` and `source`. A price taken from a source also carries `verified` (§9 step 7). There is no `confidence` field. Null is allowed only with a `fill_plan`. A missing marginal share is **not** replaced by the industry share.
- **Work nature:** weights across information or cognitive, physical, relational, trust or liability, capital or tooling, and statutory work, with the basis for them.
- **Three AI fields that are never averaged:**
  1. `exposure_prior`: theoretical, from Eloundou, ILO or Microsoft. Records the source and the occupation it came from.
  2. `observed_use`: e.g. the Anthropic Economic Index. Records the sample's limit.
  3. `sellable`: AI price at a quality the marginal buyer accepts, the buyer's current price, the cut observed, the cut needed, the distance, and the cost of human review included. **Only this field can support a chain.** The first two never close a node and never set the queue order.
- **Margin:** a pointer to the E record (§6.1), which owns who is out, the count, its basis and source. The node holds no count of its own. A `count_line`'s count lives on its stack entry (§9).
- **Blocker stack:** an ordered list, with rank 1 at the top. Each entry records:
  - the 08 class;
  - whether it is cognitive;
  - **the node where that blocker's cost sits**;
  - its cost per marginal unit;
  - what removed it elsewhere.

  `cognitive_on_top` is derived from the stack, never typed in.
- **Purpose:** COICOP 2018 or COFOG division, or `MULTI`; and use (household final, government final, GFCF, intermediate) (§2.1).
- **Tags:** route R0–R5; statute sets the price; predates the build-out; second book (sector tool, AI-system cover, AI performance of a human-authored work); reverse (the build-out makes this input dearer).
- **Status and closure:** status; for a closed node, the code, evidence, decider, date and a reopen trigger tied to a series or a statute, never a calendar lag (L11).
- **Links:** chains, blocker rows and cases (07, 08, 03, 01); `supplier_of`, `buyer_in`, `duplicate_of`; `rules` (the statutes and standards that set this line's price, §3); trade records; `killed_chains` (killed or failed chains whose path runs through this node, §5).
- **Denominators:** children defined, examined, closed by code, and unexamined.
- **Provenance:** agent, model, date, sources, and the fields marked UNCERTAIN.

---

## 5. The descent rule

Apply per node, breadth first. Finish a level across the pilot industry before descending. **In the pilot, descent below L3 runs only along E-record paths (§9); every other L3 node stays `QUEUED`.**

**Protected nodes, set before step 1 (round RC).** Every line on the path of an in-scope case's E record (§6.1), and every node a stack entry points at, is protected. A case closed at step 1 (its subject is in OUT, or it is a public body's own papers) gets no E record, so nothing of it is protected. E records of killed or failed chains stay on file and count. `protected` is derived, never typed in (§8). A protected node never takes a closure code, is never folded into an "other" node (§7 step 3), and the stage node above it is present. Protection comes first because steps 1 and 2 run before step 3 writes the stack: without it, a scope or presence rule can close a line before the stack names it. The recall test found such readings on 104 of 357 lines (§9 step 1).

**Step 1, scope.** Close only for `OUT_OF_SCOPE` or `DUPLICATE_OF`, and never a protected node. `OUT_OF_SCOPE` covers a node whose own subject is in the OUT bucket (§2.1: the AI build-out stack and extraterritorial bodies), and a case whose excluded party is a public body using AI on its own papers, unless a named private party becomes viable (05 §5.7). It never covers an OUT or PUB supplier line on an in-scope party's order (a chip, a model, a duty, a fee, a registration). Households are never out of scope: home care, where the household employs the carer, stays in.

**Step 2, presence.** At L2, a stage that does not exist in this industry is `STAGE_ABSENT`, with a reason. APQC's split between physical supply chain, service delivery and compliance is the check. A stage that holds a protected node is present, whatever the check says (round RC: PUB at MOVE for customs, HLTH at REACH for a patient panel).

**Step 3, write the stack before anything about AI.** For the margin this node serves, list every blocker the marginal party meets, in order, with the node where each one's cost sits. This includes the physical, statutory, capital and trust blockers, and the reliance screen (class 11). A blocker with no price still goes on the list, and it gets its own L4 node with `cost_per_unit: null` and the tag `unpriced`: L4 is the smallest item in the order, priced or not. **Rank order:** the case record (07, or the blocker row in 08) sets rank 1; the class file (`classes_08`) is a check, and any disagreement is written to `uncertain_fields` for the supervisor, never resolved by the agent; briefs name no other field for it (pilot P1a, K07). **An E record with no case record** (one found in a §6.3 source) takes a provisional rank 1 from the source's own stated reason ('too expensive', 'did not know of it', 'no one taking new patients'), recorded as `rank_basis: SOURCE_REASON`. The stack attack (§9 step 5) tests it, and the supervisor assigns the 08 class (pilot P3). Several blockers that bind together, cognitive or not (K12's visit, cooler and site; K02's cash and statute; C01's site file, water, cash and visit), are all rank 1 (TB3). A statute that is a `rule` edge, not a line, points at the line it prices, or at the line it forbids when `rule_bans` is true (TB2).

**A blocker already removed.** Where the case record says the party is already admitted, by a removed blocker or a cheap route (K03's tooling minimum, removed by additive making; a $5 human file), the stack keeps that blocker with `removed_elsewhere_by`. Its line is `OPEN` (`LEAF` at L4) with the `already_cheap` tag, not `BINDING`, and the E record is marked `admitted`. §9.1 counts these apart from binding stages.

**No excluded party named.** Where the record names only a held party (07 margin "-"), the E record is written for that party with `count: UNCOUNTED` (D15: fire-door makers held by resistance testing; I03: people without a prosthetist). A record that names no party and no product is `NOT_A_CASE` (§3).

**Step 4, classify the node by where it sits in that stack:**
- **It holds the rank-1 blocker:** status `BINDING`. It is never closed while that blocker stands, whatever AI can or cannot do. If AI cannot act on it, record `ai.channel: none`. The node then answers "what binds here", and it is also a reverse flag if the build-out makes it dearer.
- **It holds any blocker below a rank-1 blocker that has not been removed, on another node:** status `STACKED_BELOW`, naming that node. "Not removed" means the rank-1 blocker has no `removed_elsewhere_by`, so an `already_cheap` line is not `BINDING` (step 3; §6.1). This covers cognitive and non-cognitive lower blockers alike, and a reliance screen (class 11) that is only partly cognitive. The reopen trigger is a reading on the rank-1 class's series (08 priority classes).
- **Otherwise:** `OPEN` and queued for descent.
- **A path line (§6.1) holding no blocker** is `LEAF` when it is one cost item, and `OPEN` when it bundles several items, until it is split into its L4 lines (§9 step 5). A line holding a blocker takes the status above (pilot P1a).

**Tags, not statuses** (they never close a node): `already_cheap` (the line is already cheap for the marginal party: a diffusion sign, e.g. SolarAPP+ at $35; the tag follows the removal, and a price on file is optional, as in K03's additive making); `gate_flag` (the only AI channel sells advice, a decision, tuition, a warning or AI-authored content; the gate verdict stays with the chain, 05 §4); `second_book` (a sector tool, cover for AI systems themselves, or an AI performance of a human-authored work: kept and not delivered; 05 §4 governs).

**A node that any stack entry points at can never take a closure code.** This is what keeps the binding line visible (K05, K08, G01, I02 failed the recall walk under v0.1 because `ALREADY_CHEAP` closed them).

**One node, several margins.** Where a node serves more than one margin or buyer country (I02's three margins; G01's US against German and French buyers), it keeps one `margin_status` entry per E record, each with its own status. The node's own status is the most binding of them.

**Step 5, descend** an `OPEN`, `BINDING` or `STACKED_BELOW` node one level, until L4 (a stacked node's own lines are needed to price its stack entry).

**Closure codes (closed list):** `OUT_OF_SCOPE`, `DUPLICATE_OF`, `STAGE_ABSENT`. Each applies only to a node that is not protected.

**A kill is a chain status, not a closure (ruled by the project owner, 8 Nov 2026, Q7).** A killed or failed chain is not re-read (05 §6a): its chain record and its E record carry `status: KILLED` (or `FAILED`), with the gate and the evidence. Its E record stays on file, so the nodes on its path stay protected, carry the chain in `links.killed_chains`, and stay in every denominator. A node that served only killed chains is still a node: it is `OPEN`, `LEAF` or `STACKED_BELOW` like any other, and the queue order puts it after nodes that serve a live margin. The killed chain itself is not re-read: its path nodes are expanded only for other margins, and no fetch is spent on the killed chain's own lines (05 §6a).

**Non-closed states:** `OPEN`, `BINDING`, `STACKED_BELOW`, `LEAF`, `UNOBSERVABLE`, `QUEUED`, `UNEXAMINED`. `QUEUED` is a node that has been created and given a queue position. `UNEXAMINED` is a child defined in the taxonomy list that has no node yet.

**Not legal, by design:**
- **`NO_AI_CHANNEL` as a closure.** Both drafts used it, and it closed the binding node: the household out of infill housing, the clinic out on billing (Grok attack).
- **`BELOW_FLOOR`.** Cost share is a grade (05 §4, the RV_A overrule). Share sets the queue order; it never closes a node. The project owner ruled on 8 Nov 2026 (Q4): no park rule, at any level.

**Guarantees:**
1. Running out of budget never closes a node. An unreached node stays `QUEUED` or `UNEXAMINED`, and stays in every denominator.
2. Every closure needs a code, evidence and a reopen trigger.
3. A 5% yearly audit sample of closed nodes is re-tested by a different model family.

**Queue order:**
- `BINDING` and `STACKED_BELOW` nodes on margins with a counted party come first, then those on `UNCOUNTED` margins.
- Then `OPEN` nodes by marginal-order share.
- Then by industry share.
- Then `QUEUED` nodes, then `UNEXAMINED` children. This changes counts only, not coding.
- Nodes that serve only killed or failed chains come last.
- The exposure prior is never used to order the queue: it points at clerical work, where our register found the cognitive blocker on top almost nowhere (classes 1, 6, 13: 0 of 35 industry-instances, 08).

---

## 6. The demand side: excluded parties and trade records (the search)

Every public source that fills the grid describes incumbents: input-output tables, OEWS (which leaves out the self-employed), O*NET and APQC. The grid's L4 is defined on the marginal party's order (§2), but those sources hold no such order, so without an E record the node is never created. The E record is what puts the excluded party's order into the grid. **Grok's objection (LT_K2):** without a worked row from the §6.3 sources, this is a relabelling of the bottom-up method, and every E and T record it could build from these files is already a case on file. The test is in §10 Q1. Grok's test: a complete walk of the transport sector before fibre would have found no Netflix. So the object gets its own two records.

### 6.1 Excluded-party record (E)

One per margin and price regime: the buyer, entrant or place that is out today. **One E record per price regime**, meaning a country, or a payer scheme within one. Where the same party meets different prices or statutes in two legal orders, it gets a record in each (N01: the German check-up costs the patient nothing, a Dutch adult pays €28.51). A count shared between them is split, and the split is stated (pilot P4).

| Field | Content |
|---|---|
| `who` | the party at the margin, whether or not it is still out (`admitted` says which); e.g. "solo clinic under 250 patients in a place under 1,500 residents"; "seller under $1M adding one more country"; "household on an infill lot" |
| `count` | numerator, denominator, date, kind, source. Example: 25 lot splits completed of 6.1M eligible parcels (K02); 11,147 loans on 27.2M cards (K08). A source count that spans several price regimes is split between their records, with the basis of the split |
| `would_buy` | the non-AI thing (gate 3) |
| `path` | the ordered list of L4 cost lines, across stages and industries, that the party needs for its whole order, whether it can buy them or not: a line the party cannot buy at any price (a licence only a prosthetist can hold) is tagged `party_cannot_buy` (pilot P1a, I03). A line holding no blocker is `LEAF` when it is one item, `OPEN` when a bundle (until it is split, §5 step 4). This is where the grid and the demand side join. Every line on the path gets its own node, whether or not a taxonomy lists it, and is protected (§5). A line the party expects to be led into after its first purchase goes on the path tagged `contingent`, priced per instance (N01: a crown after a check-up that costs €0). Its expected cost needs the probability of being led into it; where no source gives one, that probability is null with a fill plan (pilot P4). `probability` and `expected_cost` sit on the stack entry; `share.of_marginal_order` holds the per-instance price, and `expected_cost` is kept apart from it |
| `stack` | the blocker stack along that path, with the rank-1 node |
| `source_type` | where the party was found (§6.3) |
| `admitted` | true when the case record says the party is already admitted, by a removed blocker or a cheap route (§5 step 3); no line on this margin is then `BINDING` unless the record names a blocker that still stands. Round RC: 12 of 61 chains (7 firm, 5 unsure, by Haiku's check). `admitted_basis` says why (pilot P1a, I08). An `admitted: true` record is a context or diffusion record (the capture book), not a chain candidate under gate 2 (05 §4) |
| `rank_basis` | `CASE_RECORD` (07 or 08 sets rank 1) or `SOURCE_REASON` (the §6.3 source's stated reason, provisional; §5 step 3) |
| `purpose`, `use` | the purpose and use tags of §2.1; the pilot admits records by `purpose` |
| `chain_status` | `live`, `KILLED` or `FAILED` (§5; with the gate and the evidence), `MECHANISM` (a mechanism row, no chain yet) or `NO_CHAIN` (round LS, LS1-25, LS1-26) |
| `regime` | the legal order the path's prices and statutes come from: a country, or a payer scheme within one (DE statutory health insurance; US, Florida). One record per regime (above; pilot P4) |

### 6.2 Trade record (T)

The thing that would exist: a business, market, intermediary, pool, certifier, place or institution. **It needs no ISIC parent.**

| Field | Content |
|---|---|
| `serves` | the E records it would admit |
| `customer_buys` | the non-AI product (gate 3) |
| `generated_from` | the shape (S1–S13, 05 §3.5), a blocker class that moved (08 extrapolation engine), an E record, or a historic analogue (01) |
| `depends_on` | the L4 nodes whose price must fall, and **the conjunction**: the second unlock and its trigger (05 §3.3) |
| `sellable_price` | AI's price at sellable quality against the cut needed, from §4 field 3 |
| `layers` | the nine-layer slots (05 §3.4), each marked filled, empty or unexamined. Layers 3, 4 and 9 (complements, intermediaries, second-order trades) are where the non-obvious beneficiaries sit |
| `ai_role` | the supervisor's reading of what AI does on the lines the trade moves: `NONE`, `FIRST` (AI removes the rank-1 line), `SECOND` (AI moves a lower line), `UNCERTAIN`; the basis goes in `ai_role_basis`, the two agents' claims in `ai_role_claims` (round LS, LS3) |
| `status` | `UNEXAMINED` → `PROPOSED` (agent) → chain record in 07 (supervisor) |

**Rule:** a stage may not be reported as having "no candidate" while an E record that runs through it is unexamined.

### 6.3 Where excluded parties are found (data that describes non-buyers and non-firms)

This is new for the project. The sources are proposals for the project owner (§10 Q1), not yet checked for fit:
- **Households who do not buy:** household budget and consumer expenditure surveys, by income band (Eurostat HBS, US CEX). Non-purchase of a service at a given income is the margin.
- **Firms that do not enter or stay small:** business demography (Eurostat business demography, US Census BDS). Births, deaths and size classes by industry; the missing small firm is the margin.
- **Firms refused or discouraged:** the ECB/EC SAFE survey (SME access to finance); trade-finance gap surveys (ADB, already in 03).
- **Work outside payroll statistics:** self-employment and own-account statistics (EU-LFS, US non-employer statistics). OEWS leaves these out by design.
- **Statutory take-up gaps:** a permitted right that is not used. Our own cases already use this: SB 9, SVAMITVA loans, EU orphan works, at 0.003–0.006% use.
- **Refusal and routing posted by suppliers:** quote floors, file requirements, minimum orders. Round MS: 19 of 40 suppliers post a refusal.

Every E record's `count` must name one of these, or say `UNCOUNTED`. An uncounted margin is a grade, not a deletion. 07 already holds several such chains.

---

## 7. The procedure for an agent expanding one node (one page)

```
EXPAND(node)
0. Read 05 §1 and §4, this file §0 and §5, and the node's parent chain. Do not change gates or rules.
1. Scope: subject in the OUT bucket (§2.1) / a public body on its own papers as the subject, with no named private party / duplicate
   → close with code + evidence. Stop. Never close a protected node: an OUT or PUB supplier line on an in-scope order stays.
   Households are never out of scope (§5 step 1).
2. If L1→L2: create the 12 stage nodes; mark each present or STAGE_ABSENT with a reason (APQC check); a stage holding a protected node is present (§5 step 2).
3. List children from the named taxonomy (process framework > ISIC 4-digit > O*NET tasks), ≤12, plus "other" <10%.
   Name the work, not the provider: one activity done by several provider types is one node, with the provider types
   (SHA HP codes) in `taxonomy.providers`; split it by provider only where its cost differs by provider, or along an
   E-record path where the party's provider type is known. SHA functions (HC) are a source only at SPECIFY, MAKE,
   MOVE and DELIVER; elsewhere taxonomy.scheme is ISIC4, O*NET or own.
   Add every protected line under this node as its own child, never in "other"; a null share is never "under 10%". The cap of 12 counts taxonomy children only; protected lines go on top, so a cell may hold more than 12.
4. For each child, for the margin(s) this branch serves (link or create an E record):
   a. write the full blocker stack along the party's path, with the node where each blocker's cost sits;
   b. fill shares: marginal order from a posted price (≤6 fetches per missing number), industry share
      only at L1; else null + fill_plan;
   c. fill the three AI fields separately; only `sellable` may be marked as evidence;
   d. set status per §5 step 4.
   In the pilot, run step 4 only for children on an E-record path; other L3 nodes stay QUEUED (§5).
   Finish the level across the pilot industry before descending (§5).
5. Never close on AI reach or on cost share. Never write a gate verdict. You may set a trade record to PROPOSED.
6. Emit JSON per §8; update the parent's denominators; append to the tree file.
7. Stop when: the node is L4; or 30 fetches are used on this node (record what is missing; a BINDING or STACKED_BELOW node keeps its status, tagged `unpriced`, with `fetches_spent` on its stack entry; any other node becomes UNOBSERVABLE);
   or a project rule would have to be broken to continue (report the conflict; do not resolve it).
```

---

## 8. Node schema (JSON, compact)

```json
{
  "id": "HLTH-SETTLE-03-02",
  "level": 4,
  "parent": "HLTH-SETTLE-03",
  "industry": "HLTH",
  "stage": "SETTLE",
  "name": "Payer enrolment and claims set-up for a new solo practice",
  "taxonomy": {"scheme": "OECD-SHA|ISIC5|ISIC4|O*NET|APQC|own", "code": null, "isic5": null, "isic5_goods": null, "isic4": null, "providers": []},
  "supply": "OWN|BOUGHT|null",
  "purpose": {"scheme": "COICOP2018|COFOG|MULTI", "division": "06", "use": "HH_FINAL|GOV_FINAL|GFCF|INTERMEDIATE"},
  "share": {
    "of_industry_cost": {"value": null, "num": null, "den": null, "year": null, "kind": null, "source": null, "fill_plan": "n/a below L1"},
    "of_marginal_order": {"value": null, "num": null, "den": null, "year": null, "kind": "CALC|POSTED|FEE_SCHEDULE|STATUTORY|STUDY", "source": null, "verified": "CONFIRMED|PARTLY|NUMBER_ONLY|RELAYED|null", "fill_plan": "..."}
  },
  "work_nature": {"cognitive": 0.0, "physical": 0.0, "relational": 0.0, "trust": 0.0, "capital": 0.0, "statutory": 0.0, "basis": "..."},
  "ai": {
    "exposure_prior": {"level": "NONE|PARTIAL|FULL|UNKNOWN", "source": null, "occupation": null},
    "observed_use": {"note": null, "source": null, "sample_limit": null},
    "sellable": {"ai_price": null, "buyer_price": null, "cut_observed": null, "cut_needed": null, "distance": null, "review_cost_included": false, "source": null},
    "channel": "general_llm|agent|sector_tool|none|unknown"
  },
  "margin": {"e_record": "E-HLTH-01", "rank_basis": "CASE_RECORD|SOURCE_REASON", "regime": null},
  "stack": [
    {"rank": 1, "class": 2, "cognitive": false, "cost_node": "HLTH-DELIVER-01-01", "cost_per_unit": null, "count": null, "gap_pair": null, "gap_price": null, "fetches_spent": 0, "probability": null, "expected_cost": null, "removed_elsewhere_by": null, "fill_plan": null, "source": null}
  ],
  "cognitive_on_top": false,
  "protected": false,
  "tags": {"route": "R0", "statute_sets_price": false, "predates": false, "second_book": "SECTOR_TOOL|AI_COVER|AI_PERFORMANCE|null", "reverse": false, "already_cheap": false, "gate_flag": null, "unpriced": false, "party_cannot_buy": false, "count_line": false, "contingent": false, "rule_bans": false, "ambiguous": false, "context": false},
  "margin_status": [{"e_record": null, "status": null, "stack": []}],
  "status": "OPEN|BINDING|STACKED_BELOW|LEAF|UNOBSERVABLE|QUEUED|UNEXAMINED|CLOSED",
  "closure": {"code": null, "evidence": null, "decider": null, "date": null, "reopen_trigger": null},
  "links": {"chains": [], "blocker_rows": [], "cases": [], "supplier_of": [], "buyer_in": [], "duplicate_of": null, "rules": [], "trades": [], "killed_chains": []},
  "denominators": {"children_defined": 0, "examined": 0, "closed_by_code": {}, "unexamined": 0},
  "provenance": {"agent": null, "model": null, "date": null, "uncertain_fields": []}
}
```

Validation rules: `cognitive_on_top` is false for an empty stack. Otherwise it is true if any rank-1 entry is cognitive and has cost_node == id, whatever the order of the entries. A `CLOSED` status requires a code from the closed list (`STAGE_ABSENT`, `OUT_OF_SCOPE` or `DUPLICATE_OF`, set in `closure.code` on a node with status `CLOSED`), plus evidence, decider, date and a reopen trigger (§4). A `BINDING` or `STACKED_BELOW` node, or any node a stack entry points at, cannot be `CLOSED`. The closure code must be one of the three in §5. `protected` is derived: true for every line on an in-scope E record's path and every node a stack entry points at (§5). A protected node cannot be `CLOSED`. A null share requires `fill_plan`. Where a node serves several margins, each `margin_status` entry carries its own stack, and the top-level `stack` is that of the most binding entry (round RC: K07 and K13 share the billing and physician-hour nodes). A stack entry with `gap_pair` is rank 1, names a rank-1 entry that names it back, and carries `gap_price` or a `fill_plan` (TB3). `gap_price` is an object holding both amounts and the net: `{add, cost, net}`, where `add` is what one line brings in, `cost` what the other costs, and `net` the difference. A `count_line` node carries `count` (numerator, denominator, date, source) on its stack entry in place of `cost_per_unit` (§9, done when). A node with `rule_bans` has a `links.rules` entry naming the statute and the condition (TB2). Every price taken from a source carries `verified` (§9 step 7).

---

## 9. The pilot: health and care by purpose, before anything else

**What the pilot covers (ruled by the project owner, 8 Nov 2026, Q3).** Every case and E record whose purpose tag is health (COICOP 2018 division 06, or COFOG 07), across systems. The HLTH system (R 86–88) is its core. Device, pharmaceutical and pharmacy lines stay in EQPT, PART, CHEM and TRADE, and come into the pilot by the tag. So all six health chains stay in: K07, K13, D12, D17, I03, I08. The tag adds two more: N04 (a hospital making its own osteotomy guide) and C02 (power for rural clinics; supervisor's purpose ruling, 8 Nov). The pilot set is 8 chains.

**Why health:**
- it already has six chains;
- on the old stages (design B's coding) 8 of 12 stages held no health case; this is re-measured on the new stages after step 1;
- the OECD System of Health Accounts gives a public functional and provider breakdown that may fill shares at L2 and L3. This was unverified: Grok could not fetch it, so the pilot checked it first. **Checked in P1b:** the SHA 2011 manual, the ICHA code lists and Eurostat `hlth_sha11_hchp` (function × provider) are fetchable; the functions are kinds of care, an L3 axis, so L2 shares stay null, and marginal-order shares come from practice cost studies and posted prices.

**Steps:**
0. **Two-coder test, then re-code the 61 chains (ruled, Q5).** Two coders from different model families (Gemini 3.8 Flash High and Grok 4.7), blind to each other, code all 61 chains of 07 (K01–K13, C01–C05, D01–D18, G01–G07, I01–I09, N01–N09) to the grid with one codebook (`_parcels/logic_tree/coding/`). Each row gets a system, the rank-1 binding stage(s), a summary stage (TB3), its order lines, a purpose, a use and an `ambiguous` flag (TB4).
   - **The test is measured on the 34 chains that round GR did not use as design cases.** The other 27 shaped the grid, so their agreement is reported separately and does not count.
   - **Pass, set before the run:** system agreement on at least 31 of 34 with Cohen's κ ≥ 0.80; summary-stage κ ≥ 0.60; the two coders' rank-1 stage sets share at least one stage on at least 29 of 34.
   - **Then** the supervisor adjudicates every disagreement on all 61 rows. Where a disagreement comes from a gap in a rule, the rule in §2.1 or §3 is amended and the change logged (§12). The adjudicated coding is the record the recall test uses.
   - **If the test fails,** the remaining 573 extracted rows are not re-coded until the amended codebook passes on a fresh sample of 30 of them. The sample excludes the 9 round-GR design rows among them, is drawn with a fixed seed, stratified by source file in proportion, and uses the same marks scaled to 30: system on at least 27 of 30 with κ ≥ 0.80; summary-stage κ ≥ 0.60; rank-1 sets sharing a stage on at least 26 of 30.
   - **Marks for any n, from RT5 on (the project owner, 12 Nov 2026):** the 34-row ratios rounded up: system on at least ⌈31n/34⌉ rows, rank-1 overlap on at least ⌈29n/34⌉ rows; the κ marks do not change. At n = 30 that is 28 and 26 (the RT to RT4 runs were scored on 27 and 26). A row leaves n only when both coders mark it `NOT_A_CASE`; a row one coder marks counts as a system disagreement. Two rows with no rank-1 line (context rows) count as sharing a stage.
   - **Result, round TC (8 Nov 2026): FAILED on the system.** On the 34 held-out chains: system 26 of 34, κ 0.72 (marks: 31, 0.80); summary stage 27 of 34, κ 0.74 (passes 0.60); rank-1 sets share a stage on 31 of 34 (passes 29); purpose 24 of 34 and use 28 of 34 (no mark). On the 27 design chains: system 23 of 27, κ 0.84; summary stage κ 0.83. Each coder flagged 23 of the 34 as ambiguous. The 12 system disagreements traced to four missing rules, now TB1a–TB1d, and the label rule in §2.1. Record: `research/tree/TC_two_coder_test_2026-11-08.md`.
   - **Result, re-test RT (8 Nov 2026, fresh sample of 30, seed 20261108): FAILED on the system count, passed the rest.** System 25 of 30 (mark 27), κ 0.80 (mark 0.80, met); summary stage 27 of 30, κ 0.88; rank-1 sets share a stage on 27 of 30 (mark 26); purpose 28 of 30; use 24 of 30; ISIC Rev.5 class 22 of 30 at 4 digits, 25 of 30 at 2 digits. Of the 5 system disagreements, 1 was not a case (X02-15) and 4 were TB1 subject questions, now TB1b (amended) and TB1e. **So the 573 rows are not re-coded yet.** The amended codebook must first pass a fresh sample of 30 (new seed, excluding the rows already used).
   - **Result, RT3 (11 Nov 2026, v0.3.6, seed 20261111): FAILED on stages.** Two rows were `NOT_A_CASE` for both coders. On 28: system 26, κ 0.92; summary-stage κ 0.54; rank-1 overlap 21. On 30: system 26, κ 0.86; stage κ 0.58; overlap 23. Fixes: v0.3.7.
   - **Result, RT4 (12 Nov 2026, v0.3.7, seed 20261112): FAILED on the system count by one row.** System 26 of 30 (mark 27), κ 0.85; summary-stage κ 0.84; rank-1 overlap 28 of 30. The prompts and the answer schema had not been updated for v0.3.7, and one sampled row (X01-C4) duplicated chain C04. The 4 system splits were subject choices (TB1e, amended). Fixes: v0.3.8; RT5 follows. Records: `research/tree/TC_two_coder_test_2026-11-08.md`, `research/tree/LS_logic_review_2026-11-12.md`.
   - **Result, RT5 (12 Nov 2026, v0.3.8, seed 20261113): PASSED.** One row (M5) was `NOT_A_CASE` for both coders, so n = 29 and the marks are 27 and 25. System 28 of 29, κ 0.96; summary stage 25 of 29, κ 0.84; rank-1 overlap 25 of 29, at the mark. The one context row (B01-A-R05) was marked by both. The 4 overlap misses: PS-13 (SETTLE/PERMIT), P03-9 (MAKE/SOURCE: class 5 has a home at both), J05-4 (subject: converter or owner), C-2 (REACH/SOURCE: class 16 has no default stage). **The 573 rows may now be re-coded** (after the pilot, Q5). Records: `_grok_returns/RT5_compare.json`, `RT5_disagreements.json`.
   - **The sample excludes** the 61 chains under any id: a 07 row whose note says it became a chain record (X01-C1 to X01-C5) is a chain (round LS, LS4-06).
   - The other 573 rows of `research/tree/` are re-coded after the pilot (Q5).
1. **Recall test.** Run §5 backwards on the cost lines of all 61 chains, as coded in step 0. Every line must survive as `BINDING`, `STACKED_BELOW`, `OPEN` or `LEAF`, with no illegal closure, and every rank-1 line on a margin not marked `admitted` must end `BINDING`. The test is run without the pilot's E-record cap: in the pilot, lines of chains outside health stay `QUEUED`, which is not a closure. If one does not, the rule is wrong, and is fixed before the pilot proceeds. Agent work: Sonnet, then a mechanical check by Haiku.
   - **Result, round RC (8 Nov 2026): see `research/tree/RC_recall_test_2026-11-08.md`.** Under the main reading 0 of 357 merged lines closed, and 59 of 61 chains kept every line with a node of its own. Two failed for want of a node: D15 (no excluded party, so no E record and no stack) and G07 (a line for a product the case does not name). Literal readings could close, fold or demote 104 of the 357 lines, on 57 of 61 chains, by the routes listed in §12 (v0.3.3); the fix is the protected-node rule in §5. Gemini 3.8 Flash High re-checked all 264 items against the draft, by route rather than line by line: 183 resolved, 80 left open by design (Q7 and case-record questions), 1 still open and since fixed (K02's two-supplier line). It found 5 new problems: 4 fixed, 1 answered in the record. Also found: the step-0 intersection default dropped a co-binder the 07 record names on 3 chains (C01, C05, D09; corrected), and on 12 of 61 chains the 07 binding blocker is the cheap route that already admits the party (now `admitted`, §6.1). Not re-walked under v0.3.3: the pilot's walk of the 8 health chains is the first use of the new rule.
2. **L1 → L2:** the 12 stages of HLTH, each present or absent, plus the cells of other systems that a health-purpose E record passes through.
3. **L3** for every present stage, from SHA functions and providers, ISIC 4-digit and O*NET.
4. **E records for health:** start from the existing margins of the 8 health chains (K07, K13, C02, D12, D17, I03, I08, N04), then source new ones from §6.3. Use SAFE and business demography for small practices, household surveys for unbought care, and statutory take-up gaps.
5. **L4 and stacks** only along E-record paths. Every other cell stays `QUEUED`.
6. **Trade records** from the shapes and from any class that moved.
7. **Roles:**
   - Gemini 3.8 Flash High reads the taxonomies and SHA files;
   - Grok finds posted prices and attacks each stack;
   - Claude supervises and checks every denominator. Sources are checked by script, then by hand: in P4 a hand check per node would have cost more context than the pricing (P4 snapshot of 9 Nov 2026: 118 lines and 107 quotes here, 119 lines in PLAN.md and the log, not reconciled; the current records v5 hold 124 lines). `research/pilot_health/inputs/check_quotes.py` fetches every cited URL and tests the quote and the number, with no model tokens; the supervisor re-checks every miss by a targeted search and hand-checks at least one source per E record, rank-1 prices first. Each price is marked `verified`: `CONFIRMED` (quote and number found), `PARTLY`, `NUMBER_ONLY`, or `RELAYED` (behind a bot wall, or a PDF with no text layer; kept, and counted apart) (pilot P4, #14);
   - Haiku validates the schema mechanically.
8. **Time it.** Record agent wall time, tool budget used, and the hours the project owner needs to read the closure sheet, the `BINDING` list and the trade records. A second industry opens only if the read fits inside one owner-day. That day is a separate one-off day that the project owner approves for each industry, never taken from the screen's owner-day (05 §7.5).

**Done when** health has:
- all 12 stages marked;
- every present stage expanded to L3;
- on every E record's path: each rank-1 and `STACKED_BELOW` line priced, or carrying the record of 30 fetches spent on it (it keeps its status under §7 step 7, tagged `unpriced`); each other line priced, `UNOBSERVABLE`, or `QUEUED` with a fill plan. The old wording, every path priced to L4 or `UNOBSERVABLE`, conflicted with §5 guarantee 1, because a line becomes `UNOBSERVABLE` only after 30 fetches on it (pilot P4, #16);
- **a count line is done with a count.** A rank-1 or `STACKED_BELOW` line that is a quantity the party needs, not an item anyone sells (a panel of members, a place on a doctor's list, providers within reach, people who know the offer exists), is tagged `count_line`. It is done when it carries that quantity as a count with its denominator, in place of a price. A count line that is one half of a gap pair is done by the gap's price, not by its count. A gap pair is done when its gap is priced (TB3). Without this, the 30-fetch rule spends fetches on lines no fetch can price. A line the party cannot buy but someone else can (I03's prosthetist licence, $805) is not a count line: it is priced (the project owner, 9 Nov 2026, #20);
- a coverage report with denominators (§9.1);
- the timing.

### 9.1 The coverage report every industry produces

- Stages present, out of 12. L3 activities defined, examined and unexamined.
- L4 lines priced, out of the lines on E-record paths; the priced ones by `verified` (confirmed, partly, number only, relayed); count lines apart, with their counts (§9, done when).
- Nodes by status, with each status's denominator.
- E records: counted versus `UNCOUNTED`, and by price regime (§6.1).
- Trade records by status.
- Margins marked `admitted` (§6.1), counted apart from the rank-1 column below.
- Existing cases attached, out of the cases coded to this industry.
- **Where the rank-1 blocker sits, by stage.** This is the answer to "where would AI even be relevant" at industry level: the stages where a cognitive blocker is rank 1 on a counted margin. A case with co-binding lines counts at each of their stages, so the column total can exceed the case count; both numbers are shown.

---

## 10. The project owner's rulings (8 Nov 2026)

Recorded on the rulings page (https://claude.ai/artifact/PAnzWYVyrTT8F9QBAxwA4g, db collection `rulings`, saved 11:59–13:06). Each ruling took the proposed option; no notes were added.

- **Q1. The two-halves design: accepted provisionally, with a test.** The grid is a coverage map; the search runs on excluded parties and trade records, sourced from data on non-buyers and non-firms (§6.3). Grok K2's objection stands as the test: the pilot must produce at least one E record from a §6.3 source, joined to a named margin, that is not already a case on file. If it cannot, the demand side merges into the grid as a field on L4. **Test result (pilot P3, 8 Nov 2026): passed, provisionally.** Three new E records from §6.3 sources, each joined to named L3 nodes, none a case on file: EU-SILC unmet need for a dental examination as too expensive (type A), the unused SGB XI §45b relief amount (type E), and Canadian adults with no provider because no one nearby takes new patients (type F). Caveats: rank 1 comes from the source's reason (§5 step 3); the counts are survey rates without headcounts; one is from 2018. So the demand side stays a separate record type; the stack attack (§9 step 5) can still undo a record. Record: `research/pilot_health/E_records_P3_v1.json`.
- **Q2. The grid: the revised 25 × 12 grid.** 25 systems on ISIC Rev.5, filled through Rev.4 / NACE Rev.2, plus the OUT bucket (§2.1); 12 stages by the job a line does in one order (§3); statutes as `rule` edges; a purpose tag on every case.
- **Q3. The pilot: health and care, by purpose** across systems (§9).
- **Q4. Cost share never closes a node.** It sorts the queue and grades the chain. No park rule (§5).
- **Q5. Re-coding: the 61 chains now, the other rows after the pilot.** Two coders on the 61 chains first (§9 step 0); the remaining 573 rows after the pilot.
- **Q6. Blocker classes: 1–14 canonical, 16 provisional** (rights clearance); 15 and 17–20 are subtypes of their host classes (08 round X).
- **Q7 (raised 8 Nov 2026 by the recall test; ruled by the project owner in chat the same day: drop it, as recommended). `KILLED_CHAIN`.** §9 step 1 says every line of a known chain must survive, but v0.3.2's §5 let `KILLED_CHAIN` close any line of a killed or failed chain that no stack entry pointed at: 63 recall conflicts on 18 of 61 chains. Under v0.3.3 a killed chain's E record stays on file, so its lines are protected and the code closes nothing a case coded. **Ruled (the recommended option):** drop `KILLED_CHAIN` as a node closure (§5). A kill becomes a status on the chain and its E record (not re-read, 05 §6a), and its path nodes carry a `links.killed_chains` entry and stay in every denominator. **Alternative:** keep the code and exempt killed chains' unstacked lines from §9 step 1.

## 11. What this spec does not yet know

- Whether the OECD System of Health Accounts can price health stages: fetched in P1b. It cannot price L2 (its functions are kinds of care); function × provider shares at L3 are possible as a prior outside the two shares, with no schema field yet (`of_industry_cost` stays L1-only); none is filled.
- Whether §6.3 sources can count excluded parties at the margin a chain names, rather than in broad bands: partly checked in P3. 10 counted candidates from 5 of the 6 source types, all survey rates or population bands, none a count at a chain's margin. SAFE has no health breakdown; US non-employer statistics need an API key.
- Hours and tool budget per industry: nothing has been measured. Grok K2's estimate for the health pilot as capped in v0.2: about 400 web fetches and 6–8 owner hours to read (high case about 1,200 fetches and more than a day, if descent is not capped to E-record paths). That read now has its own one-off owner-day per industry, approved by the project owner, and does not draw on the screen's (§9 step 8; round LS, LS2-16). Both designs' estimates were guesses, and Grok showed design B's do not survive its own expand-if-unknown rule.
- How a node's `path` is kept consistent when one E record crosses industries. Proposed: the E record owns the path, and the grid nodes hold back-links.
- Whether the v0.3.3 fixes close every route the recall test found: checked by route (Gemini, round RC), not by a re-walk of the 61 chains. The pilot's walk of the 8 health chains is the first real use of the protected-node rule.
- Whether two coders agree on the new grid at the system level: not yet. Four samples so far (TC, RT, RT3, RT4; §9 step 0): the system count failed on three and the stage marks on one. RT5, on v0.3.8, passed all four marks (overlap at the mark).
- Whether a final ISIC Rev.5 → Rev.4 correspondence table is published: both GR designers marked it UNCERTAIN. Until it is checked, the Rev.4 column of §2.1 is the supervisor's mapping, lossy where Rev.5 moved classes (45 → 46, 47 and 9531; 6311 → 6310; news agencies).
- How the top-level `stack` is picked when two `margin_status` entries are both `BINDING` (§8 validation, 'the most binding entry'): no tie rule yet (round LS, LS1-27). It has not arisen in the pilot.
- The OECD ICIO 2025 and FIGARO 2026 edition details, and Argon's Eurostat output shares (GR): not re-checked. Argon's Eurostat shares are leads, not used as shares until a person or a second auditor has opened the cited page (05 §8).

## 12. Change log

- **v0.2, 7 Nov 2026.** Grok's second review (`_grok_returns/LT_K2.json`, no web, clean) ran the descent rule on eight known chains: K02, K12 and D02 held; K05, K08, G01 and I02 lost their binding line. Fixes: `ALREADY_CHEAP` and `GATE_FLAG` became tags; a node a stack entry points at cannot be closed; unpriced blockers get an L4 node; the case record sets rank 1; co-binding blockers are all rank 1; per-margin status; the 30-fetch stop keeps a binding status; pilot descent below L3 only along E-record paths; scope follows 05 §5.7 and no longer closes households. Q1 now carries Grok's objection and a provisional test. Supervisor checked the status-enum and §6/§2 contradictions against v0.1 text before applying. Open, not fixed: K07 (the case labels billing as binding, 08 says the physician hour), left to the rank-order rule and the recall test; the trade record lacks 05 §6 fields (date, window, triggers) and must be completed before it enters 07.
- **8 Nov 2026 (round GR).** Grouping re-run by Argon and Opus (xhigh), independently. Both: MODIFY. Q2 rewritten; §2.1 flagged under review. Record: `research/tree/GR_grouping_review_2026-11-08.md`.
- **v0.3, 8 Nov 2026.** The project owner's six rulings applied (§10). §2.1 replaced: 27 systems on Rev.4 → 25 systems on ISIC Rev.5 with a Rev.4 fill column, an OUT bucket, purpose and use tags; the health carve-out removed. §3 replaced: P1–P8, B1–B4 → the 12 job stages REACH to ASSURE, with reading rules, placement rule, tie-breaks TB1–TB4 (TB1 extended to infrastructure episodes), default homes of cross-cutting services, and statutes as `rule` edges. §4 and §8 gain `purpose` and `links.rules`. §5 and §7: OUT bucket named; §7 step 1 no longer closes household employers (a v0.2 residue that contradicted §5 step 1). §9: the pilot is health by purpose; step 0 is the two-coder test with pass marks set before the run. The 27-system list and old stage table are kept in v0.2 only (`research/tree/spec_history/11_v0.2.md`; v0.1 at `11_v0.1.md` in the same folder).
- **v0.3.1, 8 Nov 2026 (round TC).** Two-coder test on the 61 chains (Gemini 3.8 Flash High; Grok 4.7 xhigh in three batches after a single 61-row call timed out at 40 min with no answer). Failed on the system mark (26 of 34, κ 0.72); passed both stage marks. Amendments from the disagreements: `isic5` written first and the class, not the label, decides (§2.1); OUT closes only a case whose own subject is in OUT, so a custom-chip buyer is coded on its product (both coders had put I04 and I05 in OUT); TB1a parts, TB1b resellers, TB1c inputs bought to sell a product, TB1d the state; a statute is a line only when it charges a fee or requires a filing, test or registration (TB2); purpose of an intermediate is `MULTI` unless it serves one final purpose. Re-test on a fresh 30-row sample before the 573 rows are re-coded (§9 step 0).
- **v0.3.2, 8 Nov 2026 (re-test RT).** Fresh 30-row sample: system 25 of 30, κ 0.80; stages κ 0.88. Failed the system count by 2. Amendments: TB1b narrowed (contract-made brands and named own products are coded on the product; a private seller of its own used item is not a reseller); TB1e, the subject is the party the margin names; `NOT_A_CASE` for rows with no party and no product. A third fresh sample must pass before the 573 rows are re-coded (after the pilot, Q5).
- **v0.3.3, 8 Nov 2026 (recall test RC, §9 step 1).** Four Sonnet walkers ran §5 backwards on the 357 lines of the 61 chains; a script and Haiku checked them; Gemini 3.8 Flash High re-checked the fixes. Main reading: 0 lines closed; 2 chains without a node for a line (D15, G07). Literal readings of v0.3.2 could close, fold or demote 104 lines on 57 chains, because steps 1–2 ran before the stack existed and the guard covered only stack lines. Fixes: **protected nodes** (every line on an in-scope E record's path and every stack cost line: no closure, no fold into "other", stage present; a derived field in §8); OUT_OF_SCOPE and the public-body clause apply to a case's subject, never to an OUT or PUB supplier line, and an OUT line keeps its stage (§2.1, §5 step 1, §7 step 1); a stage holding a protected node is present (§3, §5 step 2); protected lines are added as children and never folded, a null share is never under 10%, and L4 is priced or not (§2, §7 step 3); co-binders count cognitive or not, and placement rule 6 is aligned with TB3; a rule-edge statute's stack entry points at the line it prices (TB2, §5 step 3); an E record for a held party where none is excluded (D15, I03); `admitted` on the E record where 07 says the party is already admitted, with the cheap line OPEN and `already_cheap`, not BINDING (12 of 61 chains; §5 step 3, §6.1, §9.1); a cost supplied by two systems is split per supplier (K02); step 5 descends STACKED_BELOW; uncounted margins get a queue tier; one stack per `margin_status` entry (§8); §9 step 1 states the rank-1 requirement and that the pilot's cap is not part of the test; the pilot set is 8 health chains. Open: whether to drop `KILLED_CHAIN` (§10 Q7). Adjudication corrected for C01, C05, D09. Record: `research/tree/RC_recall_test_2026-11-08.md`. v0.3.2 kept at `research/tree/spec_history/11_v0.3.2.md`.
- **v0.3.4, 8 Nov 2026 (Q7 ruled).** The project owner ruled in chat: drop `KILLED_CHAIN`. The closed list is now three codes (§5, §8). A kill is a status on the chain and its E record; their path nodes stay protected, carry `links.killed_chains`, stay in every denominator, and come last in the queue when they serve no live margin. v0.3.3 kept at `research/tree/spec_history/11_v0.3.3.md`.
- **v0.3.5, 9 Nov 2026 (pilot P1–P3).** The 13 issues batched in `research/pilot_health/spec_issues.md`, applied as one amendment before P4. Path lines: one item is `LEAF`, a bundle `OPEN` until split (#1, §5 step 4, §6.1). TB2: an authority's document for an operator, site or person is PERMIT, a product's file is QUALIFY (#2); licensing or privileging of a person or site is PERMIT, accreditation of a service for sale is QUALIFY (#9). `who` names the party at the margin, `admitted` and `admitted_basis` say whether and why it is no longer out (#3). The path lists every line the party needs, with `party_cannot_buy` where it cannot buy one (#4). Rank disagreements go only in `uncertain_fields` (#5, no rule change). Own-staff work takes the subject's system, recorded as `supply` (#6). SPECIFY is a job, not a place (#7). A lease is SOURCE, boarding with the care is DELIVER (#8). Asynchronous remote work is MAKE, a synchronous remote session DELIVER (#10). An E record with no case record takes a provisional rank 1 from the source's reason, `rank_basis: SOURCE_REASON` (#11). L3 nodes are named by the work, with provider types in `taxonomy.providers`, split by provider only where cost differs or along an E path (#12; the proposed 'provider children' were not adopted, because L4 must stay the marginal order's cost lines). SHA functions only at SPECIFY, MAKE, MOVE and DELIVER (#13). Also recorded: the Q1 test result (§10) and the P1b SHA finding (§9, §11). Not re-applied yet to `L3_HLTH_v1.json` (#12, #13 re-cut due before the coverage report, P5). v0.3.4 kept at `research/tree/spec_history/11_v0.3.4.md`; script `research/tree/spec_amend_v035.py`.
- **v0.3.6, 9 Nov 2026 (pilot P4).** Issues #14–#19 in `research/pilot_health/spec_issues.md`, applied as proposed, plus #20, the project owner's amendment to #16. Sources are checked by script, then by hand, and every price carries `verified` (#14; §9 step 7, §8). A gap pair binds on the gap between two lines: both are rank 1 and the gap is priced (#15, TB3). Done when: each rank-1 and `STACKED_BELOW` line priced or carrying 30 fetches spent; each other line priced, `UNOBSERVABLE` or `QUEUED` with a fill plan (#16, §9). The proposal said '…or `UNOBSERVABLE`' for rank-1 lines too; it is read as '30 fetches spent, status kept', because §7 step 7 keeps a BINDING line's status after 30 fetches. A count line is done with a count (#20, §9); it covers quantities no one sells, so a priced line the party cannot buy (I03's licence) is not swept in. A statute that bans is a `rule` edge with `rule_bans` (#17, TB2). One E record per price regime, with a `regime` field and a stated split of a shared count (#18, §6.1). A follow-on line is tagged `contingent` and priced per instance (#19, §6.1). Schema: `kind` gains FEE_SCHEDULE and STATUTORY, which P4 already used; new fields `verified`, `regime`, `count`, `gap_pair`, `gap_price`, `fetches_spent`, and tags `count_line`, `contingent`, `rule_bans` (§8). Not re-applied yet to the P4 records (`research/pilot_health/E_records_P4_v1.json`): N01 and I03 to split by regime, the K07 and K13 gap pairs, N01's crown `contingent`, N04's ban, the count lines. v0.3.5 kept at `research/tree/spec_history/11_v0.3.5.md`; script `research/tree/spec_amend_v036.py`.
- **v0.3.7, 12 Nov 2026 (round RT3; the project owner approved 12 Nov).** RT3 passed the system mark (26 of 28, κ 0.92) and failed both stage marks (κ 0.54; rank-1 overlap 21 of 28). Three fixes: TB3, a stated order makes the first-named line rank 1 and the summary, the rest STACKED_BELOW; TB4, a row whose blocker is already removed takes the removed line's stage and the tag `context`; TB2, a required test or inspection is QUALIFY and the producer's own step MAKE, a bought input SOURCE unless a statute makes it a condition (PERMIT). Re-test on a fourth fresh sample (RT4) before the 573 rows are re-coded. v0.3.6 kept at `research/tree/spec_history/11_v0.3.6.md`; script `research/tree/spec_amend_v037.py`.
- **v0.3.8, 12 Nov 2026 (RT4 and round LS; the project owner's four rulings of 12 Nov).** TB4: on a context row the removed line carries the summary stage and the next standing line is rank 1. TB1e: where a row names two parties, the subject is the one kept out, else the seller of the new product. TB2: a test that licenses a person or site is PERMIT, a test on a product or lot QUALIFY, the producer's own step MAKE. §9 step 0: marks for any n are the 34-row ratios rounded up, and a row drops only when both coders mark it `NOT_A_CASE`; RT3 and RT4 results recorded; chain duplicates leave the sample. Contradictions removed: placement rule 6 against TB3; `NOT_A_CASE` in §3 against §5; `ai_channel` → `ai.channel`; `killed_chain` → `links.killed_chains` (§10); stale third-sample text (§9, §11). Fields added to §6.1 (`purpose`, `use`, `chain_status`) and §6.2 (`ai_role`). Not applied, still open from round LS: the other LS1 findings (35 unverified), the licence-fee placement (LS1-07), `already_cheap` without a price (LS1-38), the `cognitive` flag against PARTLY (LS2-19), and the stale text in 05 §8 and 06. The pilot records are not yet brought into line (LS3). v0.3.7 kept at `research/tree/spec_history/11_v0.3.7.md`; script `research/tree/spec_amend_v038.py`.
- **v0.3.9, 12 Nov 2026 (RT5 passed; the project owner's three defaults).** TB2: a class 5 minimum is MAKE when it is on making the subject's own product (in-house or by a contract maker) and SOURCE when it is on an input; a private right or consent (class 16) is SOURCE; tax registration and returns are SETTLE, a threshold or exemption is a `rule` edge on the filing line, and a registration is PERMIT only as a condition of trading. TB4: missing uptake is an outcome, not a line. The SOURCE and MAKE class cells in §3 are reworded to match. No further sample was run: the changes narrow choices RT5 passed with. The re-code of the 573 rows starts on this version (`research/tree/build_recode.py`). v0.3.8 kept at `research/tree/spec_history/11_v0.3.8.md`; script `research/tree/spec_amend_v039.py`.
- **v0.4.0, 15 Nov 2026 (round LS and HY1; G1–G7 defaults ruled by the project owner on 14 Nov; G8 and every other recommendation of the approval list approved on 15 Nov).** Rule gaps: G1 a household's own heat is ENER, storage, chargers and shops are EQPT (TB1); G2 a comma list before 'then' is one joint tier (TB3); G3 missing uptake with no cause named is REACH, flagged ambiguous (TB4); G4 a context row is allowed where the row names no party (TB4); G5 a method alone is `NOT_A_CASE`, a row that names a product is coded (§3); G6 capital that is tooling or plant for making the product is MAKE, the buyer's outlay or a buyer of a business is FINANCE, and 'capital' leaves the FINANCE class cell (LS1-34; reading rules); G7 outlet catchment (class 8) is DELIVER (reading rules); G8 purpose and use: unnamed retail goods are `MULTI` with `HH_FINAL`, household heat is `HH_FINAL` COICOP 04, a medical device sold to a provider is `INTERMEDIATE` COICOP 06, a finished device with no buyer named is `MULTI`/`GFCF` (§2.1). Rulings, each at its recommended option: 1 (LS1-03) a gap pair's summary stage follows the joint-line rule; 2 (LS1-06) with no binding line named, TB4 uses the line where the cost fell, and the `ambiguous` flag joins §9 step 0 and the §8 tags; 3 (LS1-07) hired labour and tariff licences leave SOURCE and take the stage of the job and the issuer (§3 SOURCE cell, TB2); 4 (LS1-10) TB1d: PUB also when the excluded party wants the state service itself; 5 (LS1-11) TB1e governs where the margin names the builder or seller of a network (§2.1, TB1, TB1e); 6 (LS1-15) a Place margin is listed as an Entrant (placement rule 3); 7 (LS1-37) protected lines go on top of the 12-child cap (§2, §7 step 3); 8 (LS1-38) `already_cheap` needs no price (§5 tags); 10 (LS2-16) a second industry gets its own one-off owner-day (§9 step 8). Ruling 9 (LS2-09) edits `10_Screen_Protocol.md` and is not in this amendment. Mechanical fixes: LS1-05 (§5 step 4); LS1-09 (TB2, §3 'Statutes are edges'); LS1-13 (placement rule 2); LS1-14 (§8 taxonomy); LS1-16 (§2.1); LS1-17 (§5 step 3); LS1-18 (§9); LS1-19 (§6.1); LS1-22 and LS1-23 (§7); LS1-24 (§6.1, §8); LS1-27 (§8, `cognitive_on_top` only); LS1-28 (§8); LS1-29 (§4); LS1-30 and LS2-20 (§5, §8); LS1-32 (§8); LS1-33 (§4, §8); LS1-35 (§2.1); LS1-36 and LS2-17 (§11); LS1-39 (§5); LS2-01 (§5); LS2-05 (§0); LS2-06 (§6.1); LS2-21 (§5). Edits to 05: LS2-08 (§4), LS2-11 (§7.5), LS2-12 and LS2-13 (§6a). LS2-14 and the five over-readings (LS2-02, -18, -22, -23, -24) need no change. Pilot records and the 573-row re-code are not touched by this amendment. v0.3.9 kept at `research/tree/spec_history/11_v0.3.9.md`; script `research/tree/spec_amend_v040.py`.
- **16 Nov 2026 (consistency pass, wording only).** Header now says seven rulings (Q1–Q7); the P4 line count in §9 step 7 is labelled as a snapshot. No rule changed.
