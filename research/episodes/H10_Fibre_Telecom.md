# H10 — The telecom and fibre boom and bust (1996–2002)

> **Provenance.** Grok (Grok 4.7 256K Extra High) fenced read + web.
> Wall 871s · tokens in/out/cached 185,688/48,016/375,296
> · searches 13 · fetches 22/23 ok.
> **Fence:** blocked 0 · breaches 0 · unexpected tools 0 · stage changes 0
> · URLs cited but not fetched: 0.
> **Status: GROK RETURN — leads, not findings.** Only the items listed under *Verified by Claude* below were checked
> against the source by Claude; everything else is relayed unverified. Typing (THIRD CLAIM / DIFFUSION) is Grok's
> and is reviewed in the cross-episode map.

## Verified by Claude (spot checks, quote found verbatim in the fetched source unless stated)

- ✅ Light Reading, 19 Jul 2001, *Fiber Utilization Figures Challenged*: "carriers are only using about 2.7 percent of their total lit fiber capacity" — Merrill Lynch analyst Michael Ching; a **macro-US average utilisation of lit capacity**, which Ching compares with a ~15% 1980s norm; CEOs attacked it as mixing dark with lit fibre; TeleChoice found 14 of 22 sampled city-pair routes at ≥70% of supply. **So the figure is neither "97% dark" (synthesis) nor a "misquoted single-city datapoint" (market-plumbing Concept Map §7). The Concept Map's conclusion — do not use it as a dark-fibre statistic — stands; its description of the figure is wrong.**
- ✅ Same article: "at least two thirds of the cost of a network deployment is in turning the raw fiber into usable bandwidth" (B4 substrate vs overlay — the lighting electronics, not the glass, were most of the cost).
- ✅ Cogent SEC filing (Apr 2002): "100 Mbps Internet connectivity for $1,000 per month" (= $10/Mbps-month on the bankrupt PSINet backbone; B2 Cogent).
- ⚠ **Open conflict with the Concept Map:** Grok types Cloudflare as DIFFUSION on bitrate arithmetic alone (no Cloudflare source fetched); the Concept Map calls Cloudflare "the only well-chosen name". Unresolved — needs Cloudflare's own cost/pricing evidence.
- ⚠ **New vs the Concept Map:** Grok types Indian ITES/call centres (not software exports) as THIRD CLAIM on international bandwidth (Dossani & Kenney) — the Concept Map's internet chain lists only video/CDN. Unverified.
- Unverified: DrPeering transit series (DrPeering itself calls it "very rough"), Global Crossing/FLAG/WilTel transfer fractions, Internet2/FiberCo route-miles.

---

## Grok return (verbatim)

I'll start from the draft excerpt in `H10_material.md`, then check its facts and map the downstream businesses against primary and scholarly sources.The draft is about the 1996–2002 fiber glut and what was built on the cheap capacity afterward. I’ll check the mileage, write-downs, dark-fiber claims, and price path against the best economic-history sources.The boom left a glut of long-haul glass and a collapse in wholesale capacity prices. Most of that residue was more of the same product — city-to-city bandwidth for carriers — and the predictable result was consolidation among the builders. A smaller set of businesses, selling to viewers, foreign back offices, universities, and advertisers, could exist only after the metered price fell far below what the builders had underwritten.

Assumption: the infrastructure is the long-haul fiber and IP-capacity build of about 1996–2002. The metered input is wholesale IP transit in dollars per Mbps per month, with wholesale city-pair leases (dollars per year for an OC-3, 155 Mbps) as the product the builders actually sold.

PART A

FACT: A1
VERDICT: PARTLY SUPPORTED
CORRECTION: “Millions of miles” is a strand-mile claim, not a route-mile claim. US national long-haul networks reported 104,444 route miles in 1996 and 396,125 route miles in 2001; owned route miles were 100,943 in 1996 and 204,463 in 2001, about 52 percent of the 2001 total. The rest were IRU swaps and leases. Strand-miles are many times route miles. A June 2001 press account said about 39 million miles had been laid in the US and about $90 billion spent in four years.
SOURCE: http://jwhitehorn.web.wesleyan.edu/Research/excessive.pdf
QUOTE: "measures of “fiber miles” or “strand miles” are usually many times larger than route miles."

FACT: A2
VERDICT: SUPPORTED
CORRECTION: The wipeout was on the order of $1–2 trillion, depending on date and whether equipment makers and wireless are included. A House memorandum put the broad telecom complex at a March 2000 peak of $2.7 trillion and a loss of $1.7 trillion over the next year. By September 2002, about $2 trillion of telecom equity capitalization was gone. WorldCom filed on 21 July 2002 listing $103.8 billion of assets and $41 billion of debt; its equity fell from about $150 billion in January 2000 to under $150 million by 1 July 2002. Global Crossing filed on 28 January 2002 listing assets of $22.44 billion and debts of $12.39 billion, after reportedly spending $13.7 billion to build the network. Williams Communications reportedly spent about $6 billion and faced about $5.16 billion of debt.
SOURCE: https://financialservices.house.gov/media/pdf/032102wm.pdf
QUOTE: "reached a peak in March 2000, with a combined market value of $2.7 trillion."

FACT: A3
VERDICT: PARTLY SUPPORTED
CORRECTION: The “2.7 percent” figure was not a single-city lit-share. Merrill Lynch’s Michael Ching estimated that carriers were using about 2.7 percent of total lit-fiber capacity, as an average across the US network, and he said the calculation included only lit fiber. A May 2002 account of the same research said Merrill had estimated that 35 percent of carrier fiber had been lit, and later put average utilization at 10.7 percent for 2002 including protection bandwidth, against a historical norm near 15 percent. TeleChoice, sampling 22 routes among 12 cities, found demand on 14 routes at or above 70 percent of supply. A separate Level 3 anecdote — 2 of 96 fibers lit in the first conduit — is a single-conduit fact and is not the 2.7 percent figure.
SOURCE: https://www.lightreading.com/cable-technology/fiber-utilization-figures-challenged
QUOTE: "carriers are only using about 2.7 percent of their total lit fiber capacity."

FACT: A4
VERDICT: PARTLY SUPPORTED
CORRECTION: Wholesale prices fell very far and, by early 2002, to around short-run cost. They were not practically free in 2002. DrPeering’s anecdotal US transit series runs from $1,200 per Mbps-month in 1998 to $200 in 2002, $25 in 2007, and $0.63 in 2015. TeleGeography reported city-to-city prices in the US and Europe falling about 70 percent a year for three years: a New York–Los Angeles OC-3 (155 Mbps) fell from $1.8 million per year to under $150,000 per year by the first quarter of 2002. By the third quarter of 2002 the median New York–Los Angeles 155 Mbps monthly lease was $17,720, so the freefall paused.
SOURCE: https://www.lightreading.com/business-management/telegeography-issues-bandwidth-report
QUOTE: "In the first quarter of 2002, the same lease could be had for less than $150,000."

FACT: A5
VERDICT: PARTLY SUPPORTED
CORRECTION: The engineering life cited for newly laid fiber was 25 or 30 years, with an economic overlay often planned at 10 or 15 years. Glass from the build was still being bought and lit in 2003–2005. A large share was a poor economic fit for the next speed generation: the Telecommunications Industry Association said much of the fiber already in the ground did not efficiently handle the speeds then wanted, so lighting old glass could cost more than overlaying newer fiber.
SOURCE: https://www.lightwaveonline.com/business/earnings-statements/article/16648148/is-too-much-fiber-not-enough
QUOTE: "the engineering spec may be 25 or 30 years, but you may want it to last 10 years or 15 years before you overlay."

FACT: A6
VERDICT: WRONG
CORRECTION: The bubble was fed by a false belief that cable could not be laid fast enough. US backbone traffic did roughly double every three or four months in 1995–96, then reverted to about 100 percent a year. From year-end 1997 to year-end 2001, long-distance fiber miles grew about 5 times, DWDM capacity about 100 times, and cumulative fiber capacity about 500 times, against demand growth of about 4 times. The glut did not remove the last-mile and provisioning constraints. By 2002 about 80 percent of US households could get cable-modem or DSL broadband and about 10 percent subscribed.
SOURCE: https://www-users.cse.umn.edu/~odlyzko/talks/isscc-telecom-crash.pdf
QUOTE: "Cumulative fiber capacity growth of around 500x • Actual demand growth: around 4x"

PART B

QUESTION: B1
ANSWER: What was built was long-haul fiber scope: rights-of-way, conduit, huts, and cable, plus movable lasers and DWDM terminals that “lit” strands. In the US national segment, reported route miles went from 104,444 in 1996 to 396,125 in 2001, while owned route miles went from 100,943 to 204,463. Global Crossing alone claimed a network of about 100,000 miles and reportedly spent $13.7 billion. Press accounts put US fiber at about 39 million miles and about $90 billion over four years; that mileage is not route miles. The metered input is wholesale IP transit in dollars per Mbps per month, and the builders’ own product was a city-pair lease or a multi-year IRU. A workable P* is the late-1990s sale price of that product: GTE, Frontier, and WorldCom bought about half the fibers on Qwest’s network for about $3.6 billion, enough to cover about 90 percent of construction cost, and dark fiber was quoted as high as $5,000 per mile in 1997. The realized path was $1,200 per mile for dark fiber by 2001; a New York–Los Angeles OC-3 from $1.8 million per year around 2000 to under $150,000 per year in the first quarter of 2002; and US transit from $1,200 per Mbps-month in 1998 to $675 in 2000, $200 in 2002, and $0.63 in 2015. Idle capacity was real on many new routes and in average utilization (about 2.7 percent of lit capacity in the Merrill average; about 35 percent of carrier fiber estimated lit), and it was not a 97 percent dark national plant. On 14 of 22 major routes sampled in 2001, demand was already at or above 70 percent of supply.
SOURCE: http://jwhitehorn.web.wesleyan.edu/Research/excessive.pdf
QUOTE: "more than half of total route miles added during the period 1990–2001 were based on non-sunk forms of investment."
UNCERTAIN: No prospectus page fetched this session states a single required price per Mbps-month. The Qwest IRU proceeds and the 1997–2000 lease levels are the best recovered P*. A carrier 10-K with IRU price decks would settle the exact hurdle.

QUESTION: B2
ANSWER: Ranked by later economic weight. Leads are confirmed, rejected, or reclassified inside the blocks. The same-market residue — more wholesale bandwidth for carriers — predicts the consolidation in B3 and B7, not these industries.

BENEFICIARY: YouTube, ad-supported consumer video
TYPE: THIRD CLAIM
DATES: Founded February 2005; by 9 October 2006, more than 100 million video views a day and 65,000 new videos a day; Google agreed that day to buy it for $1.65 billion in stock.
CHEAP INPUT: US IP transit, $1,200 per Mbps-month in 1998 versus $75 in 2005 and $50 in 2006 (DrPeering). A free, high-volume viewing service is not viable at the 1998 unit price.
HOW USED: Strangers uploaded and streamed video to a global audience. The customers were viewers and, after the acquisition, advertisers, not carriers buying IRUs.
MECHANISM: INPUT-COST
SCARCE COMPLEMENT: The audience and the upload habit. Google’s purchase price shows the complement had durable value; the cheap bit itself did not.
LAG: About 3 years from the 2002 bankruptcy wave to founding, about 4 years to the acquisition.
FORESEEN?: Builders expected pay-per-view and internet traffic to fill pipes. They did not describe an ad-supported free viewing platform whose supplier would be the public.
SOURCE: https://googlepress.blogspot.com/2006/10/google-to-acquire-youtube-for-165_09.html
QUOTE: "YouTube currently delivers more than 100 million video views every day"
UNCERTAIN: YouTube’s bandwidth bill as a share of cost was not on the press release. A cost-of-revenue breakdown would settle how large the input was in 2006.

BENEFICIARY: Indian IT-enabled services and call centers (GE and Dell captives, Convergys, Wipro’s Spectramind, Infosys’s Progeon, TCS’s BPO arm)
TYPE: THIRD CLAIM
DATES: Telecom liberalization from 1999; ITES takeoff around 2000. NASSCOM: ITES employment grew at a compound annual rate of 52.6 percent from fiscal 2000 to fiscal 2005, from 254,000 workers in fiscal 2004 to 348,000 in fiscal 2005; ITES export revenue from $3.6 billion to $5.2 billion in that year. Dell’s India call center opened June 2001 and reached nearly 10,000 people in Bangalore by June 2005.
CHEAP INPUT: International circuits and bandwidth. Dossani and Kenney write that the 1990s cable glut accelerated the long decline in the cost of transmitting bits, and that India’s 1999 deregulation raised bandwidth and cut prices. No India-specific dollars-per-Mbps series was on the page.
HOW USED: Real-time voice and digitized back-office work for US and UK firms were performed in India. The buyer was a foreign operating company, not a carrier shopping for an IRU.
MECHANISM: NEW-LOCATION
SCARCE COMPLEMENT: English-speaking graduates and process managers. Wages were rising about 10 percent a year in their interviews, so the labor rent was real but not fixed. Once bandwidth was cheap, the saving they measured was labor: at least 40 percent, and in one case up to 80 percent.
LAG: About 1 to 3 years from the 1999–2001 price break to large-scale hiring.
FORESEEN?: Not by the long-haul prospectuses, whose customers were carriers and large corporations buying capacity. GE and American Express had started earlier; the mass of captives arrived after deregulation and the glut.
SOURCE: https://kenney.faculty.ucdavis.edu/wp-content/uploads/sites/332/2018/03/Relocation-of-Service-Providers-to-Developing-Nations_-The-Case-of-India.pdf
QUOTE: "telecommunications carriers installed a glut of new international fiber optic cable capacity, accelerating price declines."

BENEFICIARY: Netflix instant viewing
TYPE: THIRD CLAIM
DATES: Netflix incorporated August 1997; website April 1998; IPO May 2002. Instant viewing introduced January 2007, with more than 1,000 titles, rolled out over about six months. At 31 December 2006 the firm had more than 6.3 million subscribers and more than 70,000 DVD titles. Plans started at $4.99 a month.
CHEAP INPUT: Transit at $25 per Mbps-month in 2007, against $1,200 in 1998 and $200 in 2002. The DVD-by-mail business did not use that input.
HOW USED: Selected films were streamed to subscriber PCs. The customer was a household, not a carrier.
MECHANISM: DISTRIBUTION-REACH
SCARCE COMPLEMENT: About 1.7 billion subscriber ratings, studio licenses, and the subscriber list. The 2006 10-K still treats those, not the pipe, as the assets that transfer into digital delivery. Content owners and later last-mile ISPs also took rent.
LAG: About 5 years from the 2002 crash to the January 2007 launch. Streaming did not become the main product in this filing.
FORESEEN?: The 10-K says digital delivery “will surpass DVD” only “at some point,” and that DVD would dominate the near term. Carriers had imagined pay-per-view filling their own networks.
SOURCE: https://www.sec.gov/Archives/edgar/data/1065280/000119312507042689/d10k.htm
QUOTE: "we introduced a new feature in January 2007 that allows subscribers to instantly watch movies and television series on their personal computers."
UNCERTAIN: The 10-K does not split bandwidth out of cost. Postage is the delivery cost it quantifies. The claim that a heavy-viewing subscription fails at 1998 transit prices is inferred from DrPeering’s series: a continuous 1 Mbps costs $1,200 a month at the 1998 price and $25 at the 2007 price, so two hours a day at 1 Mbps is on the order of $100 a month versus about $2. A Netflix delivery-cost footnote would settle the 2007 share.

BENEFICIARY: Google’s private dark-fiber network, used for search, data-center replication, and video haul
TYPE: THIRD CLAIM
DATES: Dark-fiber buying was being explained publicly by October 2006, alongside the YouTube deal. Google itself was founded in 1998.
CHEAP INPUT: Dark fiber, quoted at up to $5,000 per mile in 1997 and $1,200 per mile in 2001, plus transit that had fallen to $50 per Mbps-month by 2006. Google bought strands so it would not have to buy long-haul transport.
HOW USED: To tie server farms together, replicate the search index, and reach carriers’ peering points. The paying customers were advertisers and users.
MECHANISM: INPUT-COST
SCARCE COMPLEMENT: The index, the ad auction, and the data centers. The fiber was an input Google could buy; the advertisement business is what stayed scarce. Search queries themselves are a small number of bits and would have worked at a higher transit price; the third-claim piece is bulk replication and video, not the query.
LAG: About 4 years from the crash to the 2006 disclosure.
FORESEEN?: No. Sacca’s point was that outsiders misread a private network as Google becoming a carrier.
SOURCE: https://www.lightreading.com/optical-networking/google-dark-fiber-story-not-so-dark
QUOTE: "we use it to interconnect our data centers (for example, to replicate our search index to all of our computing sites)"

BENEFICIARY: US research and education optical networks (FiberCo, National LambdaRail, state and regional optical networks, SURA)
TYPE: THIRD CLAIM
DATES: Internet2’s FiberCo took an initial allocation of more than 2,500 route-miles of Level 3 dark fiber in early 2003, with further draws on the same terms through spring 2006. By early 2005 those assignments, including NLR and Internet2, exceeded 5,600 route-miles. The research community had acquired more than 27,000 intercity route-miles. SURA received 8,000 route-miles from AT&T.
CHEAP INPUT: Already-laid intercity dark fiber, released by carrier bankruptcies and abandoned wholesale plans. The article gives no dollar price for the academic buys.
HOW USED: Universities lit the fiber themselves for multi-gigabit science — high-energy physics, radiology, atmospheric data, high-definition video — instead of leasing carrier circuits.
MECHANISM: NEW-ORGANISATION
SCARCE COMPLEMENT: Campus demand and the skill to light and run the glass. The article says the advantage was ownership, and that the chance to buy the fiber would not last. Gains went to research users, not to a brand rent.
LAG: About 1 year from the 2002 bankruptcies to the 2003 Level 3 purchase.
FORESEEN?: No. The article says dark fiber had been “the exclusive province of the telecommunications carriers,” and that high-end education and financial customers could buy it only after the downturn.
SOURCE: https://er.educause.edu/articles/2005/5/dark-fiber-shining-a-new-light
QUOTE: "Spurred in part by opportunities emerging from the recent downturn in the telecommunications sector"

BENEFICIARY: Businesses buying unmetered fast access from distressed operators, Cogent’s customers
TYPE: THIRD CLAIM
DATES: Cogent closed the PSINet US asset purchase on 2 April 2002 and was already selling 100 Mbps for $1,000 a month, which is $10 per Mbps-month, unmetered, against DrPeering’s $200 per Mbps-month metered benchmark that year.
CHEAP INPUT: That $10 per Mbps-month retail offer, made possible because Cogent had bought a bankrupt backbone for about $10 million ($7 million plus $3 million for diligence).
HOW USED: Multi-tenant businesses and smaller providers took 100 Mbps or 1,000 Mbps connections as a flat monthly cost. Cogent itself is a second-claim operator, not the downstream firm.
MECHANISM: INPUT-COST
SCARCE COMPLEMENT: For the customer, whatever business sat on the pipe. The cheap port did not by itself create a scarce asset; many of these firms would have existed on slower links. The new piece was affordable 100 Mbps.
LAG: Zero. The offer and the bankruptcy purchase are the same moment.
FORESEEN?: The builders’ plans assumed rising, not bankruptcy-floor, prices. TeleGeography’s Stephan Beckert said 2002 prices were driven by short-run cost and fear of bankruptcy court.
SOURCE: https://www.sec.gov/Archives/edgar/data/1158324/000091205702013642/0000912057-02-013642.txt
QUOTE: "100 Mbps Internet connectivity for $1,000 per month."

BENEFICIARY: Indian software services (TCS, Infosys, Wipro, and the export industry)
TYPE: DIFFUSION BENEFICIARY
DATES: TCS was established in 1968 and was exporting programmers in the 1970s–80s. Software and software-services exports reached $12 billion in fiscal 2005. Employment in that segment grew at a compound annual rate of 23.6 percent from fiscal 2000 to fiscal 2005, slower than ITES.
CHEAP INPUT: International bandwidth fell, but Dossani and Kenney say software production “does not demand extremely sophisticated communications.” The decisive input was engineer wages, not Mbps.
HOW USED: Code, maintenance, and IT services were delivered from India to foreign clients. This would have grown at pre-crash circuit prices.
MECHANISM: NEW-LOCATION
SCARCE COMPLEMENT: Trained programmers and client relationships. Those kept the value; bandwidth did not.
LAG: The industry predates the glut by more than a decade. The 2000s acceleration is not evidence that the write-down was required.
FORESEEN?: The export model was already visible in the 1980s, before this boom.
SOURCE: https://kenney.faculty.ucdavis.edu/wp-content/uploads/sites/332/2018/03/Relocation-of-Service-Providers-to-Developing-Nations_-The-Case-of-India.pdf
QUOTE: "Software production was easily movable, because it can be directly done on a computer and does not demand extremely sophisticated communications capability"

BENEFICIARY: Wholesale IP voice and the international-calling business that bought it
TYPE: THIRD CLAIM
DATES: On the restructured Global Crossing network, VoIP volume was on track for 17 billion minutes in 2003, a 15-fold increase since 2001. Retail VoIP was already visible as a threat to circuit-switched carriers in 2002.
CHEAP INPUT: IP capacity on written-down networks. A voice stream is roughly a hundredth to a tenth of a megabit per second, so even the 1998 transit price of $1,200 per Mbps-month implies a sub-cent wholesale minute if the pipe is full. The collapse mattered more for carriers’ termination costs and for call-center trunks than for a PC-to-PC call.
HOW USED: Carriers and resellers moved international minutes onto IP and sold them below accounting-rate telephony. Global Crossing is the operator; the third claim is the reseller and the call-center buyer.
MECHANISM: INPUT-COST
SCARCE COMPLEMENT: Numbering, local termination, and customer relationships. Those stayed scarce. The minute itself was driven toward cost.
LAG: About 1 year. The volume surge is measured from 2001 to 2003.
FORESEEN?: Flat-rate internet telephony was already discussed in 2002. The scale of the 15-fold jump on a bankrupt global network was not in the builders’ demand cases, which had assumed traffic they could not carry.
SOURCE: https://www.sec.gov/Archives/edgar/data/1061322/000090951803000964/mv12-10ex99_1.txt
QUOTE: "it is on track to transmit 17 billion minutes of Voice over Internet Protocol (VoIP) traffic in 2003, for a 15-fold increase in VoIP volume since 2001"
UNCERTAIN: The sub-cent-per-minute arithmetic is inferred from DrPeering’s 1998 price and a 16–64 kbps codec. A tariff card would settle it.

BENEFICIARY: Skype and consumer PC calling
TYPE: DIFFUSION BENEFICIARY
DATES: The lead’s 2003 date was not re-verified on a page fetched this session. Consumer internet voice was already operating by 2002.
CHEAP INPUT: IP transit. Because a call uses so little of a megabit, the model clears at the 1998 price of $1,200 per Mbps-month as well as at the 2003 price of $120. It does not require the price to fall below the builders’ P*.
HOW USED: Individuals substituted an internet session for a retail international call. The binding complements were a broadband last mile and client software.
MECHANISM: INFORMATION/COORDINATION
SCARCE COMPLEMENT: The user network. Bandwidth was not the scarce piece.
LAG: Not applicable as a glut-dependent takeoff. Household broadband subscription, about 10 percent in 2002, was the gate.
FORESEEN?: Starr, in September 2002, already treated voice-over-IP as a threat that could offer a flat-rate service and any area code.
SOURCE: https://www.princeton.edu/~starr/articles/articles02/Starr-TelecomImplosion-9-02.htm
QUOTE: "It is already possible for anyone with a broadband connection to obtain unlimited, flat-rate telephone service"

BENEFICIARY: Akamai
TYPE: DIFFUSION BENEFICIARY
DATES: The lead’s 1998 founding was not re-verified on a fetched page. The firm is a pre-crash business.
CHEAP INPUT: None required. Its original product economized on congested, expensive delivery. Odlyzko’s result is that from 1997 onward capacity outran traffic, which undercuts a scarcity thesis.
HOW USED: Caching and edge delivery for websites. Survival through the bust is not evidence that the bust created the firm.
MECHANISM: OTHER (a scarcity-era complement: it sold relief from expensive, congested bandwidth)
SCARCE COMPLEMENT: Edge servers and customer contracts. As transit ceased to be scarce, that cost-saving rent thinned; latency and reliability could remain valuable.
LAG: Founded before the crash, so the lag is negative.
FORESEEN?: It was itself a contemporary bet on scarcity, the opposite of the third-claim bet.
SOURCE: https://www-users.cse.umn.edu/~odlyzko/talks/igi.pdf
QUOTE: "Fiber glut does not solve the other obstructions (access and provisioning)"
UNCERTAIN: An Akamai S-1 would settle the 1998 date and the original pricing thesis. They were not fetched.

BENEFICIARY: Online gameplay, podcasting, music streaming, Cloudflare, and remote work
TYPE: DIFFUSION BENEFICIARY
DATES: Not re-verified firm by firm. The lead dates are Skype’s neighbors: podcasts and games around the mid-2000s, Cloudflare 2009, mass video meetings much later.
CHEAP INPUT: By 2009 transit was $9 per Mbps-month and by 2015 $0.63, down from $1,200 in 1998. Game state, speech, and a podcast are small files. A music stream near 0.16 Mbps costs little even at late-1990s transit prices. Live gameplay is latency-bound, not price-bound.
HOW USED: They rode a network that already existed. They did not require the write-down below P*. Application hosting and early SaaS belong in this group: bandwidth is a small line item next to labor and software.
MECHANISM: DISTRIBUTION-REACH
SCARCE COMPLEMENT: Rights (music), social graphs, and software. Those held the value.
LAG: Long, and timed to last-mile broadband, codecs, and handsets more than to the 2001–02 balance-sheet collapse.
FORESEEN?: “Web 2.0” and mobile apps in the draft are mostly this diffusion. Mobile apps were gated by radios and devices, which this fiber plant did not make cheap.
SOURCE: https://drpeering.net/HTML_IPP/chapters/ch02-Internet-Transit/ch02.1-Internet-Transit-Prices
QUOTE: "these data have always generated heated debate in the peering coordinator community."
UNCERTAIN: Firm-level cost shares for Spotify, Zoom, Cloudflare, and game publishers were not fetched. The classification rests on bitrate versus the DrPeering price path.

QUESTION: B3
ANSWER: Control moved by Chapter 11 write-downs and distressed sales, not by nationalization. Old Global Crossing shareholders were cancelled. Debt and preferred stock fell from about $11 billion at the end of 2001 to $200 million at emergence on 9 December 2003. Singapore Technologies Telemedia paid $250 million for 61.5 percent of the new equity; creditors took the other 38.5 percent and $200 million in cash. Against a reported build cost of $13.7 billion, $250 million is about 1.8 percent for majority control, and the implied equity value of about $406 million is about 3 percent. Creditor recovery in cash plus equity at that price is a few cents on the dollar of the $12.39 billion claim. Reliance Gateway, after a rejected Chapter 11 bid of $110–134 million in August 2002, paid $207 million cash in October 2003 for 100 percent of FLAG. Level 3 agreed on 31 October 2005 to buy WilTel for $370 million cash plus 115 million Level 3 shares, without assuming WilTel’s debt; Williams had reportedly spent about $6 billion building that network. Cogent bought PSINet’s US operations from the bankruptcy estate for about $10 million on 2 April 2002. IRU holders also simply handed capacity back: Hogendorn records 360networks returning IRUs to Level 3 in 2005. The same owners who kept solvent networks, notably Level 3 and AT&T, took the economic write-down in equity value and then sold or donated dark fiber.
SOURCE: https://www.sec.gov/Archives/edgar/data/1061322/000090951803000964/mv12-10ex99_1.txt
QUOTE: "substantially reduced from approximately $11 billion at the end of 2001, including $1 billion of Asia Global Crossing debt, to $200 million of debt post-emergence."
UNCERTAIN: The $13.7 billion Global Crossing build cost and the $6 billion Williams build cost are “reportedly” figures in the House memorandum, not audited capex in the emergence filing. An as-spent capex rollforward would fix the fractions.

QUESTION: B4
ANSWER: The long-lived substrate was rights-of-way, conduit, huts, and the cable in them. The short-lived, and often more expensive, piece was the electronics that lit the fiber. Carrier executives told Light Reading that at least two-thirds of the cost of turning a route into usable bandwidth was that lighting. A 2001 account said routers cost many times the fiber, and that a dark strand had fallen from as much as $5,000 a mile in 1997 to $1,200. What the later users actually bought was the glass and the conduit: FiberCo’s Level 3 route-miles in 2003, more than 27,000 research route-miles by 2005, Google’s data-center fiber by 2006. Much early glass was a weak host for the next generation of speeds, so the surviving asset was the right-of-way and the spare strands, relit with newer terminals, not the original DWDM shelves. Of the headline route-miles, more than half of the 1990–2001 additions were non-sunk IRUs rather than new trenches.
SOURCE: https://www.zdnet.com/home-and-office/networking/the-path-to-the-u-s-fiber-cable-glut/
QUOTE: "could pick it up for $1,200 a mile, down from as much as $5,000 in 1997, according to Qwest."

QUESTION: B5
ANSWER: The direct losers were the builders’ shareholders and bondholders, and the equipment vendors who had financed the build. Nortel, in the same June 2001 account, was predicting a $19.2 billion quarterly loss; Corning and Lucent were named in the same damage. WorldCom’s long-distance franchise was caught between a capacity glut and customers substituting email, instant messaging, and wireless; local lines fell by 9 million, 4.7 percent, in the year Starr describes, the first such drop since the Depression. High international calling rates lost volume to IP voice: Global Crossing’s own VoIP minutes rose fifteen-fold from 2001 to 2003. US routine service work lost to Indian ITES; Dossani and Kenney note that state strategies built on domestic call centers were exposed. The wholesale lease business itself lost the price it had underwritten: TeleGeography described prices at or below cost, enforced by the threat of bankruptcy. Application firms for whom a bit was already cheap, and the DVD rental business in 2006, were not yet displaced.
SOURCE: https://www.princeton.edu/~starr/articles/articles02/Starr-TelecomImplosion-9-02.htm
QUOTE: "the total number of local phone lines dropped by 9 million, or 4.7 percent, the first decline registered since the Great Depression."

QUESTION: B6
ANSWER: DrPeering’s anecdotal US transit price, dollars per Mbps per month, minimum commit, middle of a small sample: 1998, $1,200; 1999, $800; 2000, $675; 2001, $400; 2002, $200; 2003, $120; 2004, $90; 2005, $75; 2006, $50; 2007, $25; 2008, $12; 2009, $9; 2010, $5; 2011, $3.25; 2012, $2.34; 2013, $1.57; 2014, $0.94; 2015, $0.63. Norton says there is no single market price and that the series is a rough center, not a tariff. City-pair leases, from TeleGeography via the trade press: about 70 percent annual declines for three years into early 2002; New York–Los Angeles OC-3 (155 Mbps) from $1.8 million per year to under $150,000 per year by the first quarter of 2002. Third-quarter 2002 median monthly prices for 155 Mbps, 12-month term, install excluded: New York–London $6,025; New York–Frankfurt $8,300; New York–Los Angeles $17,720; Amsterdam–London $4,200. Several of those routes had stopped falling, or had risen, between June and September 2002. A current TeleGeography wavelength database was not accessible as a historical table.
SOURCE: https://drpeering.net/HTML_IPP/chapters/ch02-Internet-Transit/ch02.1-Internet-Transit-Prices
QUOTE: "I would not recommend taking these numbers as anything but very rough indications"

QUESTION: B7
ANSWER: ST Telemedia, December 2003: $250 million for 61.5 percent of Global Crossing, about 1.8 percent of the reported $13.7 billion build, with debt cut from about $11 billion to $200 million. Reliance, October 2003: $207 million cash for FLAG after Chapter 11; a 2002 bid of $110–134 million had been turned down. Original FLAG construction cost was not in the proxy fetched here. Level 3, agreement of 31 October 2005: WilTel for $370 million cash plus 115 million shares, debt left behind, against a reported Williams build of about $6 billion. Cogent, 2 April 2002: PSINet’s US customer base, backbone, and equipment for about $10 million. Academic buyers, 2003–2005: thousands of Level 3 and AT&T route-miles, including an 8,000-mile AT&T donation to SURA. Google, by 2006, was buying dark fiber for data centers rather than a carrier. No fetched page identifies a new US national long-haul network completed between 2002 and 2015. Hogendorn notes that Aerie was proposed and never built. The documented pattern through 2006 is purchase, donation, and relighting of fiber already in the ground. Zayo’s later rollup was not on a page fetched this session.
SOURCE: https://www.sec.gov/Archives/edgar/data/1102752/000104746903036333/a2122154zprer14a.htm
QUOTE: "Reliance Gateway will pay an aggregate $207m in cash for outstanding common shares and options"
UNCERTAIN: A route-mile census for 2002–2015 would be required to say flatly that no new national network was built. Spread Networks’ later New York–Chicago path was not in these sources.

QUESTION: B8
ANSWER: Bandwidth was decisive where consumption is continuous and the product is priced in a few dollars per user per month. At $1,200 per Mbps-month (1998), one continuous megabit costs $1,200 a month; at $25 (2007), $25; at $0.63 (2015), 63 cents. Two hours a day of a 1 Mbps picture is on the order of $100 a month at the 1998 price and about $2 at the 2007 price, before peering. That is YouTube’s free viewing and, later, a Netflix-style subscription. It is also an international voice trunk into an Indian call center, which had to be cheap and reliable before the labor arbitrage of 40 percent or more could be collected; after that threshold, labor dominated the cost stack and telecom was no longer what managers complained about. Google’s inter-data-center replication is the same class of bulk input, which is why it bought dark fiber rather than pay transport. Bandwidth was a small line item for Indian software exports, for search queries, for early application hosting and SaaS, for DVD-by-mail (postage was Netflix’s named delivery cost in the 2006 10-K), for podcasts, for music at roughly 0.16 Mbps, and for ordinary game state. Skype-style calling sits in the small-line-item group even at 1998 transit prices. Akamai’s early product was a way to avoid buying the expensive input, so the price collapse weakened that thesis.
SOURCE: https://drpeering.net/HTML_IPP/chapters/ch02-Internet-Transit/ch02.1-Internet-Transit-Prices
QUOTE: "The point is that the trend is unmistakable, and no one would disagree—because transit prices have dropped every year."
UNCERTAIN: The hours-per-day conversion assumes a filled pipe and a 1 Mbps encode. It is not a firm’s ledger.

PART C

1. The mileage panic mixed three different stocks. Reported national route miles in 2001 were 396,125, and only about 204,463 were owned; the majority of the boom’s added “miles” were IRUs. Strand-miles are a further multiple. Average use of lit capacity near 2.7 percent was then retold as “almost all the fiber is dark,” while the same Merrill work was later described as finding 35 percent of carrier fiber lit. A Level 3 conduit with 2 of 96 fibers lit was a startup fact, not the national statistic.
SOURCE: http://jwhitehorn.web.wesleyan.edu/Research/excessive.pdf
QUOTE: "The loss-producing level of competition that prevailed circa 2001 was due more to the willingness of firms to sell IRUs than to actual over-investment"

2. The buyers who noticed first were laboratories, not studios. Within about a year of the bankruptcies, Internet2’s FiberCo was taking Level 3 dark fiber for universities, and by 2005 the research community held more than 27,000 intercity route-miles, including an 8,000-mile AT&T donation. Their customers were physicists and hospitals. EDUCAUSE also names the financial sector as the other group that could suddenly buy the raw material. That use was non-obvious because the builders had raised money to sell lit wholesale service, and because a dark strand was useless without electronics that still cost more than the glass.
SOURCE: https://er.educause.edu/articles/2005/5/dark-fiber-shining-a-new-light
QUOTE: "for the first time, high-end customers, such as those within the higher education and financial sectors, could obtain this vital raw material"

3. India is two industries. Software exports were old, and the work did not need rich communications; fiscal 2005 software exports of $12 billion are mostly a labor story. The glut-dependent industry was ITES: voice and digitized paper, which NASSCOM shows growing about twice as fast as software employment after the 1999 opening and the international cable glut. Collapsing them into “Indian IT” hides the third claim inside a diffusion story.
SOURCE: https://kenney.faculty.ucdavis.edu/wp-content/uploads/sites/332/2018/03/Relocation-of-Service-Providers-to-Developing-Nations_-The-Case-of-India.pdf
QUOTE: "The most significant policy reform for the ITES sector was the reform and deregulation of the communications infrastructure"

4. The dot-com bust was not waiting on the plow. Too much money went into rural long-haul and too little into the last mile. Odlyzko showed that tripling a transatlantic pipe did not make traffic grow faster than about 100 percent a year. Starr’s 2002 figures — broadband available to about 80 percent of households, taken by about 10 percent — and Netflix’s own February 2007 filing, which still expected DVD to dominate the near term, put the streaming lag on codecs, rights, and household access. The draft’s line that the bubble was constrained by the speed of laying cable reverses the sequence.
SOURCE: https://www.zdnet.com/home-and-office/networking/the-path-to-the-u-s-fiber-cable-glut/
QUOTE: "Too many companies focused on the easy part of building a network: the long-distance loops that cut mostly through rural areas."

5. Cheap glass did not make a private network cheap, and several famous “internet” businesses did not need the write-down. Lighting equipment was the larger cost, which is why a $1,200-a-mile strand still left most firms on leased ports, while Google and the universities, who could buy terminals, took the option. Consumer VoIP, software exports, podcasts, and ordinary web applications clear at 1998 transit prices. The uses that fail at P* and work after the fall are bulk video, inter-data-center replication, and real-time offshore voice. Akamai, built to save scarce bandwidth, is the counter-example inside the draft’s own lead list: it is a child of congestion, and the glut was the environment it had to outlive.
SOURCE: https://www.lightreading.com/cable-technology/fiber-utilization-figures-challenged
QUOTE: "at least two thirds of the cost of a network deployment is in turning the raw fiber into usable bandwidth"

SOURCES FETCHED:
https://www-users.cse.umn.edu/~odlyzko/doc/internet.growth.myth.pdf
https://www-users.cse.umn.edu/~odlyzko/talks/isscc-telecom-crash.pdf
https://www.lightwaveonline.com/business/earnings-statements/article/16648148/is-too-much-fiber-not-enough
https://www.princeton.edu/~starr/articles/articles02/Starr-TelecomImplosion-9-02.htm
https://drpeering.net/HTML_IPP/chapters/ch02-Internet-Transit/ch02.1-Internet-Transit-Prices
https://www.lightreading.com/cable-technology/fiber-utilization-figures-challenged
https://www.lightreading.com/business-management/telegeography-issues-bandwidth-report
https://www.lightwaveonline.com/business/market-research/article/16653636/long-haul-bandwidth-prices-stabilising-on-key-routes
http://jwhitehorn.web.wesleyan.edu/Research/excessive.pdf
https://www.sec.gov/Archives/edgar/data/1061322/000090951803000964/mv12-10ex99_1.txt
https://www.everycrsreport.com/reports/RS21253.html
https://kenney.faculty.ucdavis.edu/wp-content/uploads/sites/332/2018/03/Relocation-of-Service-Providers-to-Developing-Nations_-The-Case-of-India.pdf
https://er.educause.edu/articles/2005/5/dark-fiber-shining-a-new-light
https://www.zdnet.com/home-and-office/networking/the-path-to-the-u-s-fiber-cable-glut/
https://www-users.cse.umn.edu/~odlyzko/talks/igi.pdf
https://financialservices.house.gov/media/pdf/032102wm.pdf
https://www.sec.gov/Archives/edgar/data/1065280/000119312507042689/d10k.htm
https://www.sec.gov/Archives/edgar/data/794323/000110465905051575/a05-19295_1ex99d1.htm
https://www.sec.gov/Archives/edgar/data/1158324/000091205702013642/0000912057-02-013642.txt
https://www.sec.gov/Archives/edgar/data/1102752/000104746903036333/a2122154zprer14a.htm
https://www.lightreading.com/optical-networking/google-dark-fiber-story-not-so-dark
https://googlepress.blogspot.com/2006/10/google-to-acquire-youtube-for-165_09.html
