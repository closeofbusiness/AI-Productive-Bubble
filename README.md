# Productive Bubbles and the AI Infrastructure Boom

Infrastructure booms overbuild, and the cheap capacity they leave behind has repeatedly founded businesses nobody planned for. Fibre laid in the dot-com boom later carried Netflix and YouTube. This repository asks which businesses the AI build-out could make possible, where the customer buys something other than AI, and turns the answer into dated forecasts that will be scored.

**Status:** research in progress. Draft forecasts lock on 31 January 2027; the first scoring is in October 2027.

## Findings so far

- **History supports the idea, with limits.** In 10 of 13 classic bubbles, from the 1470s printing glut to the 2002 fibre bust, at least one business grew because leftover capacity became cheap. These businesses are usually small and specific. When only the shares crash and a solvent owner keeps the assets, nothing reaches new users: electricity prices rose after the 1929 Insull crash.
- **The classic route is not open for AI yet.** There has been no bust, so no AI capacity has been written down and sold cheap. What AI makes cheap is general capability: the price of a fixed level of model performance falls about 13 times a year. The physical inputs the build-out uses (memory chips, transformers, electricians) are getting more expensive for everyone else.
- **Cheap AI rarely removes the blocker.** Of 61 candidate business chains, 35 pass the project's gates and 26 fail. In the first 13, every business that already pays was made possible by something other than AI: printing, locks, statutes, supply chains, or dropping insurance billing. Where it could be measured, AI's saving covered 2–9% of the gap that keeps people out.
- **Blockers come in stacks.** Machine interpreting costs about $2 an hour against a $37.50 threshold, so the price has crossed. Quality on a business call now binds, and then whether the buyer will trust it.
- **Count what people buy, not what gets made.** AI-generated music reached 44% of daily uploads at one streaming service and about 1–3% of streams.

## How it works

Each candidate is a **chain**: a cost falls; at some price a new business can pay; suppliers and services form around it; someone holds the scarce piece and keeps the value. A chain is admitted only if three gates hold:

1. The product is not AI.
2. It could not pay at the old cost, judged at the margin: someone who is out of the market today gets in.
3. The customer is not buying AI.

For each chain the project records the **blocker**, meaning the cost or constraint that keeps the marginal buyer or entrant out, with a price and a source. It then writes dated forecasts, each with a probability and a reference forecast to be scored against.

## Repository contents

| File | What it is |
|---|---|
| `01_Historic_and_Logic_Map.md` | 17 historic episodes, the rules drawn from them, and 20 corrections to commonly repeated stories |
| `03_AI_Enablement_Map.md` | Where AI lowers a general-purpose cost, and which businesses that might enable |
| `04_Argon_Trust_Assessment.md` | An audit of Gemini Deep Research as a source finder |
| `05_Mission_Statement.md` | The question, the gates and the scoring rules; governs where documents conflict |
| `06_Mission_Logic_Map.md` | The admission logic as a flow and a decision table |
| `07_Chain_Register.md` | The 61 candidate chains and their verdicts |
| `08_Blocker_Register.md` | Blocker classes, priced blockers, and what removed blockers elsewhere |
| `09_Forecast_Sheet.md` | 160 draft forecasts with probabilities and reference forecasts |
| `10_Screen_Protocol.md` | The two-monthly screen that re-reads blocker prices from March 2027 |
| `11_Logic_Tree_Spec.md` | An industry-by-stage grid used to check that the search misses nothing, with a health care pilot |
| `research/episodes/` | One source file per historic episode, with the evidence behind each row of the map |

## Method and checks

AI models do most of the reading, searching and drafting. Claude supervises, Grok builds and attacks chains and finds sources with read-only web access, and Gemini reads long documents and codes cases independently. A person rules on every verdict.

Every model output is a lead until the cited page has been fetched and the quoted sentence found on it. Of 578 evidence items in the enablement round, 567 were verbatim and none were invented. Two model families code each case blind; the coding rules passed on the fifth test round, when the two models agreed on the industry for 28 of 29 cases.

## Limits

- The documents cite working files (model returns, dispatch parcels, earlier spec versions) that are not in this repository.

- The method screens candidates out. It cannot pick winners.
- No forecast is locked yet, and every chain verdict is a proposal until it is ruled on.
- Many figures come from vendors' own pages or filings and are labelled as such.
- The detailed industry test covers health care only so far.

## Licence

Copyright © 2026 the Productive Bubbles project. Text, tables and figures are licensed under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/). Short quotations from cited sources remain under their original terms. See `LICENSE`.
