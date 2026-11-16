# H09 — Electricity: the Insull holding-company frenzy and cheap-power industries

> **Provenance.** Grok (Grok 4.7 256K Extra High) fenced read + web.
> Wall 972s · tokens in/out/cached 265,461/65,620/1,152,640
> · searches 18 · fetches 17/19 ok.
> **Fence:** blocked 0 · breaches 0 · unexpected tools 0 · stage changes 0
> · URLs cited but not fetched: 0.
> **Status: GROK RETURN — leads, not findings.** Only the items listed under *Verified by Claude* below were checked
> against the source by Claude; everything else is relayed unverified. Typing (THIRD CLAIM / DIFFUSION) is Grok's
> and is reviewed in the cross-episode map.

## Verified by Claude (spot checks, quote found verbatim in the fetched source unless stated)

- ✅ Gould, *Output and Productivity in the Electric and Gas Utilities* (NBER c4272): "the horsepower of electric motors owned by manufacturing plants and driven by purchased energy constituted 65 percent of total electric motor horsepower" (B2 — purchased power was the builders' own intended market → diffusion).
- ✅ BPA history (OSTI 1132823; sentence split by a sidebar in the PDF layout): "June 8, 1938 – The Federal Power Commission approves BPA's initial power rates of $17.50 kilowatt-year (equivalent to 2 mills per kilowatt-hour)"; and "Dec. 20, 1939 – BPA signs its first power sales contract with an industrial firm – Aluminum Company of America" (B7 — cheap power by public rate, not write-down).
- ◐ *Niagara Mohawk Power Corp. v. FPC*, 209 F.2d 814 (D.C. Cir. 21 Jan 1954): Justia and CourtListener both block automated reads (Cloudflare / API token), so the full sentence was **not** read. CourtListener's full-text search for the exact phrase "one and one-third mills" + Alcoa returns this opinion and only this one — the phrase is in the cited case; the $8.00/mhp and "discriminatorily low" wording remains **unverified**.
- Not checked: HSUS Db234/Db218 price and generation rows (Grok's QUOTE fields are table rows, not sentences); David (1990) quotes.
- Consistent with market-plumbing Concept Map §7: Insull = a securities write-down above solvent operating companies; L3 unit drive predates the crash. **New datum for the framework: average revenue per kWh *rose* 1929→1932 (2.57¢ → 2.85¢ all services; industrial 1.38¢ → 1.53¢) — the metered input never fell below P\*, so no third claim could form on the crash.**

---

## Grok return (verbatim)

I'll start from the draft excerpt and the definitions in `H09_material.md`, then check the numbered facts and map the downstream beneficiaries against primary and historical sources.The receivership dates and the price series are in view. Next I’ll pin the capital structure, how much physical plant was actually built, and whether the crash changed the price of a kilowatt-hour.The 1920s episode was a write-down of holding-company securities sitting on top of operating utilities that stayed solvent and kept charging regulated rates. The kilowatt-hour did not become cheap because those securities failed. Most of the industries usually listed as “downstream of Insull” were diffusion beneficiaries of electrification the utilities had been recruiting since the 1900s, or they sat on purpose-built hydro priced in mills, not on stranded Insull steam plant.

Assumption: “the boom” is the late-1920s holding-company pyramid in the draft (Middle West, Insull Utility Investments, Corporation Securities), not the whole history of electrification since 1882. Prices below are average revenue per kilowatt-hour sold (revenue divided by sales), not a single posted tariff.

Part A

FACT: A1
VERDICT: PARTLY SUPPORTED
CORRECTION: All three failed in 1932, but they were not one receivership. Middle West Utilities: creditor’s bill filed 14 April 1932; equity receivers (Samuel Insull, Edward N. Hurley, Charles A. McCulloch) appointed 15 April 1932. Insull Utility Investments, Inc.: equity receiver Calvin Fentress appointed 16 April 1932; adjudicated bankrupt 22 September 1932; trustee appointed 9 March 1933. Corporation Securities Company of Chicago was in the same April 1932 cluster — the court treated its receivership application as inseparable from the other two — but the opinions fetched do not state a separate calendar day for its receiver.
SOURCE: https://law.justia.com/cases/federal/appellate-courts/F2/74/779/1477242/
QUOTE: "on the next day, Samuel Insull, Edward N. Hurley, and Charles A. McCulloch, at the suggestion and by agreement of the parties, were appointed by the court as such receivers."
UNCERTAIN: the exact day a receiver was appointed for Corporation Securities. A docket entry or the 16–18 April 1932 Chicago newspapers would settle it.

FACT: A2
VERDICT: SUPPORTED
CORRECTION: The leverage that broke was at the top of the pyramid, not a debt-to-plant ratio on the dynamos. On 16 April 1932 Insull Utility Investments had $60,000,000 of unsecured Series B debentures, $6,000,000 of Series A debentures, and $42,085,020 of secured bank debt, against about $1,500,000 of unliened assets. The court called it hopelessly insolvent. Stock on top of that debt (60,000 prior preferred, 40,000 first preferred, 450,000 second preferred, and 3,636,622 common, all without par) was wiped out in substance. Middle West’s common was later found worthless. The Public Utility Holding Company Act of 1935 describes the device Congress was striking at: control “through disproportionately small investment,” and securities issued on “fictitious or unsound asset values.” No fetched source gives a single empire-wide ratio such as “one percent controlled the plant.”
SOURCE: https://www.cetient.com/case/in-re-insull-utility-investments-inc-2264956
QUOTE: "On April 16, 1932, when the receivers were appointed, it had outstanding unsecured debentures of Series B, aggregating $60,000,000"

FACT: A3
VERDICT: PARTLY SUPPORTED
CORRECTION: Operating companies built and kept the grid; the 1928–32 top layer mostly stacked securities on it. Edison’s Pearl Street station opened in 1882. Census kilowatt-hours generated rose about tenfold from 1902 to 1917, before Insull Utility Investments existed. Middle West, a holding company and not itself a public-service corporation, did control real systems: more than eighty-five utilities in over 5,000 communities. When it failed, Commonwealth Edison, Peoples Gas, and Public Service Company of Northern Illinois were solvent and paying dividends. Judge Evans called the 1929 investment trust “nothing but a glorified gambling institution.” The Federal Trade Commission inquiry, begun in 1928 and run for seven years in 96 volumes, documented securities issued on inflated asset values, affiliate overcharges, and financial structures that state regulators could not see. The 1935 Act then required those write-ups to be stripped out of the property base used to judge investors’ claims. The frenzy financed both some real acquisition and integration and a large volume of write-ups and circular securities. It did not, by itself, “build the physical foundation of the modern power grid.”
SOURCE: https://www.ftc.gov/enforcement/competition-matters/2014/11/ftc-milestones-making-case-reform-public-utility-holding-company-laws
QUOTE: "issuing securities based on inflated asset values, overcharging for services provided by affiliates to the regulated utility, and unsound or unnecessary financial structures"

Part B

QUESTION: B1
ANSWER: What was built was central-station generation plus distribution and, increasingly, interconnection, owned by operating utilities. Edison’s Pearl Street steam station (New York, 1882) is the commercial start. Census generation by central stations was 2,507 million kilowatt-hours in 1902 and 25,438 million kilowatt-hours in 1917, about a tenfold rise. Electric-utility net generation (Historical Statistics series Db218, million kilowatt-hours, United States) was 39,405 in 1920, 75,418 in 1927, 92,180 in 1929, 79,393 in 1932, and 141,837 in 1940. By 1937, sales to ultimate consumers were about 100,798 million kilowatt-hours. Large commercial (wholesale) service was 52,879 million kilowatt-hours, 52.5 percent of sales and 27.9 percent of revenue, at 1.14 cents per kilowatt-hour. Domestic nonfarm service was 16,815 million kilowatt-hours, 16.7 percent of sales and 33.5 percent of revenue, at 4.32 cents per kilowatt-hour. Street railways and electrified steam railroads took 6,446 million kilowatt-hours at 0.88 cents per kilowatt-hour.
Metered input: average revenue per kilowatt-hour sold, by class of service, in cents per kilowatt-hour. That is the unit whose path can be measured. It is not one price. In 1917, census average revenue was about 5.54 cents per kilowatt-hour sold for lighting, 1.22 cents for stationary-motor power, and 0.77 cents for rail.
P*: not recoverable as a single cents-per-kilowatt-hour figure from a fetched Insull prospectus. Two different hurdles show up. Operating companies sold kilowatt-hours at regulated rates and, in the Chicago core, kept paying dividends through the crash. The top companies’ hurdle was debt service on pledged shares: Insull Utility Investments failed in April 1932 because it could not pay interest on $66 million of debentures, with only about $1.5 million of assets left unpledged. A later statutory benchmark, not a 1920s prospectus, is the Niagara licensee’s Federal Power Act standard: half of surplus above an annual return of 6 percent on net investment went to amortization reserves. That is a return on investment, not a kilowatt-hour price.
Idle plant: utility net generation in 1932 was 79,393 million kilowatt-hours, 12,787 million kilowatt-hours and 13.9 percent below the 1929 peak of 92,180 million. On the Edison Electric Institute sample, large-commercial sales fell from 42,971 million kilowatt-hours in 1929 to 30,964 million in 1932 (down 27.9 percent), while the average revenue on that class rose from 1.375 to 1.532 cents per kilowatt-hour. Domestic sales on the same sample rose, from 9,526 million kilowatt-hours in 1929 to 11,494 million in 1932. The idle margin was unused industrial capability in a depression, not a scrapped grid.
SOURCE: http://hsus.cambridge.org/HSUSWeb/toc/treeTablePathIdDb218-227.html
QUOTE: "1929 | 92,180" and, same table, "1932 | 79,393" (million kilowatt-hours, utility net generation)
UNCERTAIN: the share of nameplate kilowatts standing idle. A national installed-kilowatt series for 1929 and 1932 (Census of Electrical Industries or Federal Power Commission) would settle it. Gould’s prime-mover horsepower line in the fetched NBER chapter is too damaged by transcription to use.

QUESTION: B2
ANSWER: Ranked by economic significance. The first three are one phenomenon: more kilowatt-hours in the markets central stations were already built to serve. That predicts consolidation of generation into utilities, which is what happened, rather than a new industry created by a 1932 price collapse. At least three entries are easy to miss: electrified steam railroads, irrigation as the original farm load, and process heat in paper, chemicals, and petroleum.

BENEFICIARY: U.S. manufacturing on electric unit drive (motors on individual machines; single-story layouts)
TYPE: DIFFUSION BENEFICIARY
DATES: Electric motors under 5 percent of factory mechanical drive in 1899; about 55 percent of manufacturing power equipment by 1919; 82.3 percent by 1929; 89.8 percent by 1939 (Gould, Table 14). Productivity effect shows in 1919–29, before the crash.
CHEAP INPUT: Purchased central-station energy, priced for industry near 1.2 to 1.5 cents per kilowatt-hour in the late 1920s (1.38 cents industrial average revenue in 1929; 1.22 cents for power sales in 1917). David dates the industrial takeoff to real rate declines after 1914–17, not to 1932.
HOW USED: Group drive and then unit drive replaced line shafts. Factories were rebuilt lighter and often on one floor, with separate motors so one department could stop without stopping the mill. About half of a 5 percentage-point acceleration in manufacturing total-factor-productivity growth, 1919–29 versus 1909–19, lines up with the rise in secondary motor capacity.
MECHANISM: NEW-ORGANISATION
SCARCE COMPLEMENT: Know-how of factory layout and machine placement. The measured gains showed up as productivity, so a large share went to buyers of manufactured goods, not to a durable monopoly rent.
LAG: About four decades from the first central station (1881–82) to the early-1920s productivity effect. Relative to the 1932 crash the lag is negative: the payoff was already in the statistics.
FORESEEN?: Engineers saw unit drive early. The 1912 census already listed motors for printing, woodworking, pumps, and machine tools. Wide redesign was slow because old shafted plants were still serviceable.
SOURCE: https://gwern.net/doc/economics/automation/1990-david.pdf
QUOTE: "factory electrification did not reach full fruition in its technical development nor have an impact on productivity growth in manufacturing before the early 1920s."

BENEFICIARY: Industrial buyers of central-station power as a class (chemicals and paints, electrical equipment, rubber, iron and steel, textiles, leather, and other motor loads)
TYPE: DIFFUSION BENEFICIARY
DATES: Power’s share of central-station revenue rose from about 12 percent in 1902 to 34.5 percent in 1917. In 1937 large commercial sales were more than half of all kilowatt-hours. Takeoff of purchased power is 1902–1929, not post-1932.
CHEAP INPUT: Wholesale power, about 1.1 to 1.8 cents per kilowatt-hour (1.80 cents in the 1922 Gould classification for power; 1.14 cents for large commercial in 1937). Utilities posted these rates to fill daytime and off-peak load. They were inside the operating company’s plan for earning its allowed return on the average kilowatt-hour, not a price below that plan.
HOW USED: Firms shut isolated generators and bought energy. In 1939, motors driven by purchased energy were 65 percent of manufacturing electric-motor horsepower; in 1899 self-generated energy still drove more than three-fifths. This is the same market the stations were built for. The residue is more kilowatt-hours for power buyers, and consolidation of generation, not a new downstream industry.
MECHANISM: INPUT-COST
SCARCE COMPLEMENT: The utility franchise and the industrial customer’s process know-how. Once purchased power was reliable, the isolated plant lost its rationale; the durable scarcity sat with the franchised distributor.
LAG: From Pearl Street (1882) to power as a third of revenue (1917) is about 35 years. No lag after 1932: industrial kilowatt-hours fell in the depression.
FORESEEN?: Yes. The 1907 census said central stations were creating daytime motor load on purpose, including concessions for customers who would shift hours.
SOURCE: https://www.nber.org/system/files/chapters/c4272/c4272.pdf
QUOTE: "the horsepower of electric motors owned by manufacturing plants and driven by purchased energy constituted 65 percent of total electric motor horsepower"

BENEFICIARY: Household mechanical refrigeration, led by General Electric’s Monitor Top; the wider appliance load (irons, cooking, washing) is the same customer
TYPE: DIFFUSION BENEFICIARY
DATES: Monitor Top line manufactured 1927–1936 and was a large seller in the late 1920s and early 1930s. Household refrigerator ownership: 10 percent of households in 1930, 56 percent in 1940. Use per residential customer: 339 kilowatt-hours in 1920, 502 in 1929, 601 in 1932, 952 in 1940.
CHEAP INPUT: Residential average revenue per kilowatt-hour, 7.45 cents in 1920, 6.33 cents in 1929, 5.60 cents in 1932, 3.84 cents in 1940. The refrigerator boom was underway at the 1927–29 price, about 6.3 to 6.8 cents, before any holding-company write-down. Part of the later fall in average revenue is customers moving into lower blocks as they used more kilowatt-hours, which is the appliance effect itself.
HOW USED: Households replaced iceboxes. The refrigerator is a complement to the domestic meter: the utility’s customer and the appliance maker’s customer are the same household. Frigidaire, Maytag, and Hoover belong to this complex; this session did not retrieve separate company histories for them.
MECHANISM: COMPLEMENTARY-PRODUCT
SCARCE COMPLEMENT: Brand, cabinet design, and dealer or utility installment plans. Ownership jumping from 10 percent to 56 percent of households in ten years means much of the gain went to households. Utility merchandise departments also captured the customer relationship.
LAG: Urban nonfarm electrical service was already 47.4 percent of dwellings in 1920 and 84.8 percent in 1930. The appliance takeoff is the late 1920s, during the build-out, not after 1932. Domestic kilowatt-hours kept rising in 1929–32 while industrial sales fell.
FORESEEN?: Yes. The 1907 census already treated irons, toasters, and small refrigerating apparatus as load-builders, and some companies tried Tuesday ironing circuits.
SOURCE: https://www.thehenryford.org/collections/explore/artifact/165213
QUOTE: "In 1930, 10% of households had them -- by 1940, 56% did."

BENEFICIARY: Aluminum smelting on purpose-built cheap hydro (Alcoa at Niagara from 1895; Alcoa on TVA power from 1935; Alcoa as Bonneville’s first industrial customer, contract 20 December 1939)
TYPE: THIRD CLAIM relative to ordinary investor-owned industrial rates; the intended customer of the hydro projects themselves. Not a claimant on written-down Insull securities.
DATES: Niagara contracts from 1895, raised by 1922 to 52,000 mechanical horsepower, term to 1 May 1967. TVA purchases from 1935; wartime dams (Fontana, Cherokee, Douglas) built for aluminum. Bonneville Project Act 20 August 1937; rate approved 8 June 1938; Alcoa contract 20 December 1939; war expansion 1941–42.
CHEAP INPUT: Niagara mechanical power at $8.00 per mechanical horsepower-year, equal to $11.50 per kilowatt-year, about 1.33 mills per kilowatt-hour, against 3 mills per kilowatt-hour paid by that company’s other electric customers. Bonneville wholesale rate $17.50 per kilowatt-year, equal to 2 mills per kilowatt-hour, unchanged for 27 years. The 1940 U.S. industrial average revenue was 1.06 cents (10.6 mills) per kilowatt-hour. Smelting was viable at roughly one-eighth to one-fifth of that industrial average. No fetched TVA tariff schedule states Alcoa’s Tennessee mills-per-kilowatt-hour.
HOW USED: Continuous electrolysis in potlines sited at the falls or the federal bus. The Columbia and Tennessee plants were recruited by public power agencies. They did not buy distressed Middle West turbines.
MECHANISM: INPUT-COST
SCARCE COMPLEMENT: The power contract and the smelter site. At Niagara the cheap right had private value: in 1949 the power company paid Alcoa $1,500,000 to cancel it, then earned about $1,059,000 a year from other customers against $416,000 a year from Alcoa. That rent was durable until the utility bought it back.
LAG: Niagara aluminum predates the 1920s pyramid by a generation. Bonneville aluminum is about 7 years after 1932, timed to federal dams, not to the Insull receivership.
FORESEEN?: Yes for the projects that served it. Niagara contracts begin in 1895 with the reduction plant on a leased site. Bonneville’s first industrial contract was Alcoa, by design. TVA launched Cherokee and Douglas largely for wartime aluminum.
SOURCE: https://law.justia.com/cases/federal/appellate-courts/F2/209/814/362226/
QUOTE: "Alcoa paid for the mechanical power at the annual rate of $8.00 per mhp, which is the equivalent of $11.50 per kilowatt per year, or about one and one-third mills per kilowatt hour."

BENEFICIARY: Process-heat and continuous-process industries (paper, petroleum refining, chemicals) using electricity for heat and instruments, not only for shafts
TYPE: DIFFUSION BENEFICIARY
DATES: Bound up with the 1920s manufacturing-productivity acceleration. David treats them as part of the 1919–29 total-factor-productivity jump, alongside unit drive.
CHEAP INPUT: The same industrial kilowatt-hour, around 1 to 1.5 cents in the 1920s and 1930s. These plants also often kept their own generation where they needed steam, so purchased power was only part of the energy system.
HOW USED: Electric instruments and relays for automatic control, and electricity as process heat, let refineries, paper mills, and chemical works run longer and more continuously. This is easy to miss because it is not “motors instead of belts.”
MECHANISM: NEW-ORGANISATION
SCARCE COMPLEMENT: Process patents and plant-specific operating skill. Productivity accounting picked up the capital saving; the text does not show a durable monopoly created by the cheap kilowatt-hour alone.
LAG: Same as unit drive: payoff in the 1920s, about forty years after the dynamo’s commercial start, and before the holding-company crash.
FORESEEN?: Electrical engineers foresaw flexible electric drive. David’s point is that the process-control and shift-work package was worked out industry by industry, not as a surprise after 1932.
SOURCE: https://gwern.net/doc/economics/automation/1990-david.pdf
QUOTE: "electrification was a key complementary element in the foregoing innovations because pulp- and paper-making, chemical production, and petroleum refining"

BENEFICIARY: Farms reached by central stations and, after 1936, by rural electric cooperatives
TYPE: DIFFUSION BENEFICIARY for early irrigation and commercial farm power; the post-1935 acceleration is INSTITUTIONAL (federal loans to cooperatives), not a purchase of idle Insull plant
DATES: Farm dwellings with service: 1.6 percent in 1920, 10.4 percent in 1930, 12.6 percent in 1935, 32.6 percent in 1940, 77.7 percent in 1950. Rural Electrification Act 20 May 1936, low-cost loans to nonprofit cooperatives. Executive Order 7037 is the usual 11 May 1935 start of the agency; that order was not on a page successfully fetched this session.
CHEAP INPUT: Not a collapse in the urban cent per kilowatt-hour. Farm average revenue was high because the lines were long: Gould’s farm price moves from about 2.1 cents per kilowatt-hour in 1927 to 2.66 cents in 1937 as domestic farm use, rather than cheap irrigation power, became a larger share. Private utilities would not build those lines at their required return. The scarce cheap input was federal credit, not a written-down urban kilowatt-hour.
HOW USED: Early western projects pumped irrigation water. Later loads were household and farmstead motors (and, on Gould’s evidence, a rising domestic share). The cooperatives built new rural lines.
MECHANISM: INSTITUTIONAL
SCARCE COMPLEMENT: The cooperative franchise and access to federal loans. The statute’s aim was the farm household’s gain, not a durable private rent.
LAG: Slow rise until the mid-1930s (10.4 percent of farms in 1930, 12.6 percent in 1935), then a jump to 32.6 percent by 1940, about four to five years after the Act. That lag follows legislation, not the 1932 receiverships.
FORESEEN?: Irrigation power was listed in the 1912 census. Universal farm domestic service was a political project of the 1930s precisely because private builders had declined it.
SOURCE: https://www.nps.gov/home/learn/historyculture/ruralelect.htm
QUOTE: "This law allowed the federal government to make low-cost loans to farmers who had banded together to create non-profit cooperatives"

BENEFICIARY: Commercial air conditioning in stores, theaters, hotels, and other commercial buildings
TYPE: DIFFUSION BENEFICIARY
DATES: Gould, writing in 1946 from census and trade data through the early 1940s, treats air conditioning as a recent commercial load that was starting to fill seasonal valleys. Carrier’s 1902 machine and 1920s theater installations were not on a page fetched this session, so those dates are not used as findings.
CHEAP INPUT: Commercial average revenue, about 4.35 cents per kilowatt-hour in 1926 and 3.03 cents in 1940 (Historical Statistics, commercial class). Air conditioning was being added while commercial rates were still several cents, not at a post-crash distress price.
HOW USED: Cooling public rooms flattened seasonal demand and improved the utility’s load factor. It is a complement to the commercial meter. The later Sun Belt migration is a longer geographical effect; it is not documented in the pages fetched here.
MECHANISM: COMPLEMENTARY-PRODUCT
SCARCE COMPLEMENT: Equipment makers’ designs and the building owner’s location. By 1941 it was still a load-balancing use, not yet a mass household industry in these sources.
LAG: Roughly a decade after the 1920s commercial grids were dense, and still incomplete in 1941. Not timed to 1932.
FORESEEN?: Utilities had chased off-peak load since the 1900s. Gould presents air conditioning as a new way to do that job, visible to the trade by 1941.
SOURCE: https://www.nber.org/system/files/chapters/c4272/c4272.pdf
QUOTE: "air-conditioning has begun to balance seasonal demands in the electric consumption of stores, theaters, hotels,"

BENEFICIARY: Electrified divisions of steam railroads
TYPE: DIFFUSION BENEFICIARY
DATES: Kilowatt-hours for electrified steam railroads more than quadrupled from 1927 to the early 1940s, while street-railway purchases fell. Gould’s index for this class, 1927 = 100, is 555.6 by 1942 on the Edison Electric Institute splice.
CHEAP INPUT: Rail traction was the cheapest large class: about 0.77 cents per kilowatt-hour in 1917 and 0.88 cents in 1932, still under 1 cent in 1942 (0.809 cents on Gould’s 1942 rail average).
HOW USED: Locomotives on electrified divisions took firm wholesale power. This grew through the depression and the war. It is easy to miss because the streetcar story, which is a decline, dominates popular accounts.
MECHANISM: INPUT-COST
SCARCE COMPLEMENT: The railroad’s right-of-way and terminal traffic. Electrification followed dense corridors; the cheap kilowatt-hour did not create the railroad.
LAG: A 1920s–1940s build on grids already interconnected. Growth continues after 1932 because traffic and engineering projects continued, not because holding-company stocks were cancelled.
FORESEEN?: Central stations had courted traction load since the 1900s. The shift from streetcars toward main-line electrification was visible in the census by 1927–37.
SOURCE: https://www.nber.org/system/files/chapters/c4272/c4272.pdf
QUOTE: "rapid gains in the use of electric power by electrified divisions of steam railroads, which has more than quadrupled since 1927"

BENEFICIARY: Electric street railways, streetcar suburbs, and trolley-park amusement load
TYPE: UNCLEAR only if “beneficiary of electrification” is the question; as a beneficiary of the post-1929 residue, the lead is rejected
DATES: Traction was an early central-station customer (revenue share about 3.4 percent in 1902, 4.9 percent in 1917). Street and interurban purchases then fell from 6,256 million kilowatt-hours in 1927 to 4,395 million in 1932 and 4,256 million in 1942.
CHEAP INPUT: They already had the cheapest public rate, under 1 cent per kilowatt-hour. A further fall in that rate did not save them.
HOW USED: They were a load the utilities and holding companies owned or supplied, including inside Middle West’s “railway or bus” subsidiaries. Traffic declined for many years. Suburbs and end-of-line parks were traction companies’ own weekend-load strategy from the early century, and they faded with the cars. Automobiles and buses took the passengers. Cheap kilowatt-hours were not the cause.
MECHANISM: OTHER (an early intended load that then shrank; not a third claim)
SCARCE COMPLEMENT: Franchise streets. That scarcity lost value as riders left. Holding-company owners were stuck with the decline.
LAG: Peak is before or around 1920; the 1930s are the decline. Lag after the crash is not a takeoff.
FORESEEN?: The original traction load was foreseen and sought. The collapse was the surprise, and it was a transport surprise.
SOURCE: https://www.nber.org/system/files/chapters/c4272/c4272.pdf
QUOTE: "the falling off in the consumption of power purchased by street and inter-urban railway companies, whose traffic has been declining for many years"

BENEFICIARY: Electric elevators and the skyscraper
TYPE: DIFFUSION BENEFICIARY of the early central station, rejected as a creature of the 1920s holding-company boom
DATES: Listed by the 1912 census as a standard motor use, fifteen years before Insull Utility Investments (1928).
CHEAP INPUT: Daytime commercial power at retail rates of several cents per kilowatt-hour. Elevators were valuable to the station because they filled the daytime valley. They did not need a price below the builder’s required average return; they were part of earning it.
HOW USED: Motors with simple speed control moved cars. The customer was the building owner, already the utility’s commercial customer.
MECHANISM: COMPLEMENTARY-PRODUCT
SCARCE COMPLEMENT: The urban land parcel and the elevator patent position (Otis is the usual name; not documented on a page fetched here). Height was limited by structure and zoning as much as by the kilowatt-hour.
LAG: In place before the 1920s frenzy. No post-1932 takeoff in these sources.
FORESEEN?: Yes. The 1912 census named elevators explicitly.
SOURCE: https://www.nber.org/system/files/chapters/c4272/c4272.pdf
QUOTE: "for running elevators, where electrical devices for securing control in speed and direction of movement"

BENEFICIARY: Frozen-food packers (Birdseye) and the supermarket (King Kullen, 1930)
TYPE: UNCLEAR
DATES: Not established from a page fetched this session. Mechanical refrigeration as a motor load is in the 1907 census, which is much earlier than 1930.
CHEAP INPUT: Unknown for these firms from fetched pages. Household and commercial refrigeration ran at the ordinary domestic and commercial rates above, which were falling for technical and block-rate reasons.
HOW USED: A cold chain needs reliable refrigeration. That does not show that the business required the holding-company write-down, or that the supermarket’s binding input was electricity rather than the automobile and self-service. Treat as unconfirmed, not as a third claim.
MECHANISM: OTHER (cold chain; not shown to be price-collapse dependent)
SCARCE COMPLEMENT: Unknown here. Brand and retail sites are the likely candidates if the lead is real.
LAG: Unknown relative to 1932.
FORESEEN?: Small electric refrigerating apparatus was already a census example in 1907. The retail frozen-food format is not documented in the pages fetched.
SOURCE: https://www.nber.org/system/files/chapters/c4272/c4272.pdf
QUOTE: "the introduction of electric motors in refrigeration, in the operation of New York City's high pressure water system"

BENEFICIARY: Clinton Engineer Works / Oak Ridge gaseous diffusion (K-25), as a TVA customer
TYPE: UNCLEAR as a market third claim. It is a state project on new federal hydro, secret from TVA’s own chairman. It is not a private firm living on written-down Insull kilowatt-hours.
DATES: Site chosen 1942; K-25 construction began June 1943, completed early 1945, cost about $500 million, about 12,000 construction workers. Alcoa was already TVA’s large prewar customer from 1935.
CHEAP INPUT: TVA power in very large blocks. No fetched page states the cents per kilowatt-hour Oak Ridge paid. A 2014 decommissioning paper says that at full operation K-25 used one-seventh of the nation’s electrical power. Utility net generation in 1945 was 222,486 million kilowatt-hours, so one-seventh is about 31,800 million kilowatt-hours, on the order of 3,600 megawatts if run all year. That sits badly next to the rest of the wartime record and should not be used as a fact.
HOW USED: The gaseous-diffusion cascade separated uranium-235. The site was chosen because TVA power and non-flooding cooling water from below Norris Dam were already there.
MECHANISM: INPUT-COST
SCARCE COMPLEMENT: Federal priority, secrecy, and the process design. There was no private brand to capitalize the cheap power.
LAG: About a decade after TVA’s 1933 start; three years after U.S. entry into the war. Unrelated to the 1932 receiverships.
FORESEEN?: The war load was planned. The use was not: TVA’s account says the chairman did not know what the power was for until August 1945.
SOURCE: https://www.tva.com/about-tva/our-history/powering-world-war-ii
QUOTE: "using millions of kilowatts of TVA energy for something not even the Chairman of TVA knew about"
UNCERTAIN: K-25’s share of national generation. A Manhattan District power log, or the Federal Power Commission’s wartime industrial series, would settle the “one-seventh” sentence.

QUESTION: B3
ANSWER: Control changed by receivership and reorganization of the holding companies, then by the 1935 Act’s breakup rules, not by a sale of power plants at a fraction of construction cost. Middle West went into equity receivership on 15 April 1932; that receivership was superseded by a section 77B reorganization, with a trustee appointed in 1934. Its common stock was worthless. The Chicago operating companies (Commonwealth Edison, Peoples Gas, Public Service Company of Northern Illinois) stayed solvent and kept paying dividends. Insull Utility Investments’ receiver was appointed 16 April 1932; the firm was adjudicated bankrupt on 22 September 1932. Its assets were mostly pledged utility securities. Secured banks held the collateral; unsecured debenture holders ($66 million) had about $1.5 million of free assets and a possible fight over whether the pledge was allowed. The court did not find a liquidating dividend in cents per dollar of physical plant, because the physical plant was not the bankrupt’s free asset. Under the 1935 Act the SEC then stripped write-ups out of the base used to allocate votes and pushed systems toward a single integrated geography. Buyers at distressed prices, where they appear, bought securities and claims, not turbines by the kilowatt.
SOURCE: https://law.justia.com/cases/federal/appellate-courts/F2/74/779/1477242/
QUOTE: "It is disclosed by the record that the common stock is worthless and will probably remain so"
UNCERTAIN: the cents on the dollar ultimately paid to Insull Utility Investments debenture holders, and the dollar write-down of operating-company rate base. Bankruptcy dividend orders and the original-cost restatements under Accounts 100.5 and 107 would settle those fractions.

QUESTION: B4
ANSWER: No fetched source splits 1920s utility capital expenditure into a percentage for long-lived civil works versus short-lived machinery. What the record does show is that the durable piece beneficiaries actually used was the operating franchise, the distribution network, and regional interconnection, still in the hands of solvent operating companies. Generating equipment was not a frozen 1929 stock: Gould finds the larger part of the rise in output per unit of fuel in 1912–32, which means boilers and turbines were being replaced by more efficient ones while the depression cut sales. By 1939, 89.8 percent of manufacturing power equipment was electric and 65 percent of manufacturing motor horsepower ran on purchased energy, so the 1940s industrial and appliance load sat on a living grid, not on a bankrupt’s surplus dynamos. Hydro civil works (Niagara, and later TVA and Columbia dams) are the truly long-lived substrate, and they belong to those projects, not to the Insull securities.
SOURCE: https://www.nber.org/system/files/chapters/c4272/c4272.pdf
QUOTE: "The greater part of the productivity increase occurred in 1912—32."
UNCERTAIN: the accounting share of 1920s gross additions that was structures, rights-of-way, and copper, versus turbines, boilers, and meters. A Federal Power Commission or census breakdown of electric plant in service by account would settle it.

QUESTION: B5
ANSWER: The incumbents displaced by central-station electricity were other ways of making light, cold, and mechanical drive, not the customers of a post-1932 distress price.
Isolated factory power plants lost the contest inside the factory. In 1899 self-generated energy drove more than three-fifths of manufacturing electric-motor horsepower; in 1939 purchased energy drove 65 percent.
The household icebox lost to the electric refrigerator: ownership of mechanical refrigerators went from 10 percent of households in 1930 to 56 percent in 1940.
Illuminating gas and other non-electric light lost the lighting load the stations were born to take. In 1902, lighting was 84.6 percent of central-station electric revenue. Dwellings with electric service rose from 8.0 percent in 1907 to 34.7 percent in 1920, 68.2 percent in 1930, and 78.7 percent in 1940. David notes that early electric light was aimed squarely at illuminating gas on cost, with brightness and fire safety as the unmeasured edge.
Street and interurban railways lost passengers, and their purchased kilowatt-hours fell from 6,256 million in 1927 to 4,256 million in 1942. The displacer was the automobile and the bus. They were electricity customers, not victims of cheap electricity, and they sat inside the holding-company systems as a declining load.
SOURCE: https://www.nber.org/system/files/chapters/c4272/c4272.pdf
QUOTE: "In 1902 more than four-fifths of the electric service revenue of all central electric stations came from the sale of current for domestic and street lighting."

QUESTION: B6
ANSWER: Average revenue per kilowatt-hour, United States electric utilities, cents per kilowatt-hour (Historical Statistics Db234 residential is Db235, industrial is Db237; denominator is kilowatt-hours sold in that class).
Residential: 16.20 in 1902, 10.50 in 1907, 9.10 in 1912, 7.52 in 1917, 7.45 in 1920, 7.00 in 1926, 6.33 in 1929, 6.03 in 1930, 5.60 in 1932, 5.01 in 1935, 3.84 in 1940.
Industrial: 1.49 in 1926, 1.38 in 1929, 1.41 in 1930, 1.53 in 1932, 1.30 in 1935, 1.06 in 1940. The industrial series in this table starts in 1926.
All services: 2.70 in 1907, 2.10 in 1917, 2.57 in 1929, 2.66 in 1930, 2.75 in 1931, 2.85 in 1932, 2.46 in 1935, 2.06 in 1940.
The Insull collapse did not lower the price anyone paid in 1932. The all-services average rose from 2.57 cents in 1929 to 2.85 cents in 1932 because the cheap industrial class shrank. The industrial average itself rose, from 1.38 to 1.53 cents. Residential revenue kept falling on a path that had already run from 16.20 cents in 1902 to 6.33 cents in 1929, and it was 5.60 cents in 1932. The 1935 Act restructured holding companies and attacked write-ups and affiliate fees. It was not a statute that cut the cents per kilowatt-hour, and the annual series shows no break in 1935: residential went from 5.01 cents in 1935 to 3.84 in 1940 as use per residential customer rose from 677 to 952 kilowatt-hours, which pulls average revenue down a declining-block schedule even if the posted blocks do not move.
SOURCE: http://hsus.cambridge.org/HSUSWeb/toc/treeTablePathIdDb234-241.html
QUOTE: "1932 | 2.85 | 5.60 | 3.93 | 1.53" (all services, residential, commercial, industrial, cents per kilowatt-hour)

QUESTION: B7
ANSWER: These are cheap-power industries of their own infrastructures. They are not the residue of the Insull write-down.
Niagara, from 1895: Alcoa (successor of the Pittsburgh Reduction Company) paid $8.00 per mechanical horsepower-year, $11.50 per kilowatt-year, about 1.33 mills per kilowatt-hour, for up to 52,000 mechanical horsepower, while the power company’s other electric customers paid 3 mills per kilowatt-hour. The company later called the Alcoa rate discriminatorily low and in 1949 paid $1,500,000 to escape it. That is the fetched viability price: on the order of 1.3 mills per kilowatt-hour, against an alternative sale at 3 mills. Hooker Electrochemical, Carborundum, and Union Carbide clustered at the same falls for the same reason; no contract price for those three was on a page fetched this session.
Norsk Hydro, founded 2 December 1905 for Birkeland-Eyde nitrogen fixation, is the same kind of story only if it is told as owned hydro (Svelgfoss, then Vemork at Rjukan), so the “price” is the company’s own cost of falls, not a utility tariff below someone else’s P*. No kilowatt-hour price was retrieved from a non-Wikipedia page this session.
Bonneville: Federal Power Commission approval on 8 June 1938 of $17.50 per kilowatt-year, stated as 2 mills per kilowatt-hour, postage-stamp, no increase for 27 years. First industrial contract: Aluminum Company of America, 20 December 1939, locating in the Pacific Northwest. Grand Coulee was tied into that federal system (Bonneville–Grand Coulee line energized 23 March 1941). Viability price for that aluminum: 2 mills per kilowatt-hour wholesale, against a 1940 U.S. industrial retail average of 1.06 cents (10.6 mills) per kilowatt-hour.
TVA and aluminum: Alcoa’s plant south of Knoxville, then the largest in the world, began buying TVA power in 1935 after having generated much of its own. Fontana was given to TVA in 1941; Cherokee and Douglas were crash-built for wartime aluminum. No mills-per-kilowatt-hour figure for those contracts was fetched.
TVA and Oak Ridge: the Clinton Engineer Works (1942) was sited for TVA power and for cooling water below Norris Dam. K-25 (construction from June 1943, operation early 1945) “consumed enormous amounts of electric power.” The price per kilowatt-hour was not on the pages fetched. The claim that K-25 used one-seventh of national electric power is in a 2014 demolition paper and is not reconciled with 1945 utility generation of 222,486 million kilowatt-hours.
SOURCE: https://www.osti.gov/servlets/purl/1132823
QUOTE: "The Federal Power Commission approves BPA’s initial power rates of $17.50 kilowatt-year (equivalent to 2 mills per kilowatt-hour)."
UNCERTAIN: contract prices for Hooker, Carborundum, Union Carbide, Norsk Hydro, TVA-Alcoa, and Oak Ridge. The company contracts or TVA and Norsk Hydro annual reports would settle them.

QUESTION: B8
ANSWER: David’s 1990 paper says the dynamo’s productive use waited on factory reorganization, not on the arrival of cheap current alone. In 1899 electric motors were under 5 percent of U.S. factory mechanical drive, and only about 3 percent of residences had electric light. Reaching 50 percent diffusion took about another twenty years. Group drive (one motor per line shaft) persisted from the mid-1890s to the eve of the 1920s and left the old belts in place, so capital-output ratios could rise and total-factor productivity did not. Unit drive, one motor per machine, then allowed lighter single-story buildings, materials handling, and partial shutdowns. That package “did not reach full fruition … before the early 1920s,” four decades after the first central station. About half of the 5 percentage-point acceleration in manufacturing total-factor-productivity growth in 1919–29, compared with 1909–19, is associated with the growth of secondary motor capacity. A further slice came from continuous-process plants (petroleum, paper, chemicals) using electric instruments and process heat. The lag that matters is from the 1880s technology to a 1920s reorganization. It is not a lag from the 1932 write-down to a new industry. The factories that captured it did so while holding-company stocks were still rising.
SOURCE: https://gwern.net/doc/economics/automation/1990-david.pdf
QUOTE: "approximately half of the 5 percentage point acceleration recorded in the aggregate TFP growth rate of the U.S. manufacturing sector during 1919-29"

Part C

1. The metered price moved the wrong way at the moment of the crash. All-services average revenue rose from 2.57 cents per kilowatt-hour in 1929 to 2.85 cents in 1932, and the industrial average rose from 1.38 to 1.53 cents, because the cheap class of sales collapsed. A third claim needs the unit price to fall through the builders’ required price. Here the security holders were wiped out while the operating companies kept a regulated rate base and, in Chicago, kept paying dividends. Contemporaries staring at Insull’s ruin naturally thought “the utilities failed.” The firms that sold the kilowatt-hours had not.
SOURCE: http://hsus.cambridge.org/HSUSWeb/toc/treeTablePathIdDb234-241.html
QUOTE: "1929 | 2.57 | 6.33 | 4.00 | 1.38" and the 1932 row "2.85 | 5.60 | 3.93 | 1.53"

2. The uses that look downstream were the utilities’ own sales program. By 1907–12, census reports already named industrial motors, elevators, small refrigeration, irrigation pumps, irons, and toasters as ways to escape an evening-only lighting load. Appliance makers and elevator firms were complements the first claimants were cultivating, at rates designed so that the average kilowatt-hour still covered the franchise. They are diffusion beneficiaries. They are not firms whose model worked only after P* was abandoned.
SOURCE: https://www.nber.org/system/files/chapters/c4272/c4272.pdf
QUOTE: "Central stations became increasingly interested in encouraging other off-peak uses for electricity."

3. The big productivity gain arrived before the bubble burst, and it was an architectural gain. Unit drive paid when new single-story plants were built in the 1920s capital boom. David ties roughly half of the manufacturing total-factor-productivity acceleration of 1919–29 to secondary motors. A historian who starts the clock at Insull’s 1932 failure will miss the payoff and will mis-date the lag. The lag is from the 1880s dynamo to 1920s building practice.
SOURCE: https://gwern.net/doc/economics/automation/1990-david.pdf
QUOTE: "This was four decades after the first central power station opened for business."

4. The industries that truly required power at a few mills per kilowatt-hour did not live on the Insull residue. Alcoa’s Niagara power, from 1895, cost about 1.33 mills per kilowatt-hour against 3 mills for other customers of the same company, and the utility eventually paid $1,500,000 to cancel a contract it called discriminatorily low. Bonneville’s 1938 rate was 2 mills per kilowatt-hour, and Alcoa was the first industrial signer, in 1939. Those are intended customers of hydro built for them, or a federal sponsor setting a cost-based rate below investor-owned industrial retail prices (1.06 cents per kilowatt-hour industrial average in 1940). The non-obvious mechanism is a discriminatory long contract, or a public rate, not a receivership.
SOURCE: https://law.justia.com/cases/federal/appellate-courts/F2/209/814/362226/
QUOTE: "He also admitted that Alcoa's rate of $8.00 per mhp was discriminatorily low."

5. Two familiar “electricity” stories run backward, and one famous wartime statistic does not survive the generation series. Street railways are remembered as the industry electricity created; their purchased energy was already in long decline by 1932 (6,256 million kilowatt-hours in 1927 to 4,256 million in 1942), and the holding companies were carrying a shrinking traction load. Electrified steam-railroad demand, the quieter series, more than quadrupled after 1927. Separately, a 2014 account of K-25 says the plant used one-seventh of U.S. electric power. One-seventh of 1945 utility net generation (222,486 million kilowatt-hours) is about 31,800 million kilowatt-hours. That claim should not be repeated until a wartime power log supports it. Oak Ridge was a secret federal load on TVA, which is a real fact; “one-seventh of the nation” is the part most accounts do not check.
SOURCE: https://archivedproceedings.econference.io/wmsym/2014/papers/14141.pdf
QUOTE: "Under full operation, K-25 used one-seventh of the nation’s electrical power."

SOURCES FETCHED:
https://law.justia.com/cases/federal/appellate-courts/F2/74/779/1477242/
https://www.cetient.com/case/in-re-insull-utility-investments-inc-2264956
https://www.ftc.gov/enforcement/competition-matters/2014/11/ftc-milestones-making-case-reform-public-utility-holding-company-laws
https://repository.law.umich.edu/cgi/viewcontent.cgi?article=7742&context=mlr
http://hsus.cambridge.org/HSUSWeb/toc/treeTablePathIdDb234-241.html
http://hsus.cambridge.org/HSUSWeb/toc/treeTablePathIdDb218-227.html
https://www.nber.org/system/files/chapters/c4272/c4272.pdf
https://gwern.net/doc/economics/automation/1990-david.pdf
https://law.justia.com/cases/federal/appellate-courts/F2/209/814/362226/
https://www.osti.gov/servlets/purl/1132823
https://www.thehenryford.org/collections/explore/artifact/165213
https://www.tva.com/about-tva/our-history/powering-world-war-ii
https://www.energy.gov/management/k-25-gaseous-diffusion-process-building
https://archivedproceedings.econference.io/wmsym/2014/papers/14141.pdf
https://www.nps.gov/home/learn/historyculture/ruralelect.htm
