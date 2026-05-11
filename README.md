# propertyiq 🏠

> Investor-grade real estate deal analysis, powered by Claude AI.

Paste any property listing URL — Zillow, Realtor.com, Redfin, LoopNet, Crexi — and get a full underwriting report back in seconds. propertyiq scrapes the listing, pulls live rent comps, runs the numbers, and tells you plainly whether the deal pencils out.

Built as a [Claude Skill](https://www.anthropic.com/claude) for real estate investors evaluating single-family rentals and small multifamily acquisitions (1–20 units).

---

## Example Output

> **Note:** The example below was generated in May 2026 from an active listing at that time. The property may no longer be available. Numbers reflect market conditions, rent comps, and interest rates as of that date and should not be treated as a current analysis.

```
========================================================================
PROPERTY UNDERWRITING: 403 Leverett Ave, Staten Island, NY 10308
REPORT DATE: May 4, 2026
========================================================================

--- PROPERTY OVERVIEW ---
Type:                   Half Duplex (Single Unit — SFR analysis applies)
Year Built:             1976
Units:                  1
Unit Mix:               1x 3BD/2BA — 1,600 sqft
Utilities:              Tenant-paid
HOA:                    None
Days on Market:         5
Notable:                Brick/vinyl construction, finished basement,
                        above-ground pool, fully fenced yard, EV charging.
                        Listed as multi-family but only one rentable unit.

--- CORE ASSUMPTIONS ---
Purchase Price:         $750,000
Down Payment:           $187,500 (25%)
Loan Amount:            $562,500
Interest Rate:          7.50% (30yr investment property)
Amortization:           30 Years
Vacancy Rate:           5%
CapEx Reserve:          7% gross rent ($2,604/yr — elevated for 1976 build)
Maintenance/Repairs:    $100/mo ($1,200/yr)
Property Management:    10% of EGI ($3,534/yr)
Closing Cost Estimate:  $18,750 (2.5%)
Origination Points:     $0 (conventional)
Total Cash to Close:    $206,250

--- RENT ROLL ---
Unit            Type            Monthly Rent        Annual Rent
---------------------------------------------------------------
Unit 1          3BD/2BA         $3,100              $37,200
---------------------------------------------------------------
GROSS TOTAL                     $3,100              $37,200

--- RENT COMP ANALYSIS ---
Source 1: Zillow Rent Zestimate (same property)  → $3,094/mo
Source 2: Apartments.com (302 Maybury, 10308)    → $3,200/mo (3BR house)
Source 3: Zumper (Staten Island median, Apr 2026) → $3,200/mo (all types)
Median Market Rent:    $3,100/mo (conservative; half duplex vs. full house)
Listing Rent vs. Market: In-line

--- INCOME & EXPENSE CALCULATION ---
Gross Potential Income:             $37,200
Vacancy Adjustment (5%):          -($1,860)
-----------------------------------------------
EFFECTIVE GROSS INCOME (EGI):       $35,340

Property Taxes (2025 actual):     -($6,438)
Insurance:                        -($1,800)
Property Management (10%):        -($3,534)
CapEx Reserve (7% GPI):           -($2,604)
Maintenance/Repairs:              -($1,200)
-----------------------------------------------
TOTAL OPERATING EXPENSES:         -($15,576)
Operating Expense Ratio:            44.1%

NET OPERATING INCOME (NOI):         $19,764

--- DEBT SERVICE & CASH FLOW ---
Annual Debt Service (P&I):          $47,197
Monthly Debt Service:               $3,933
-----------------------------------------------
ANNUAL CASH FLOW:                  -($27,433)
MONTHLY CASH FLOW:                 -($2,286)

STATUS: DEEPLY NEGATIVE CASH FLOW

--- KEY PERFORMANCE METRICS ---
Cap Rate:                           2.64%
Cash-on-Cash Return (Down Pmt):    -14.63%
Cash-on-Cash Return (All-In):      -13.30%  (incl. closing costs)
Debt Service Coverage Ratio:        0.42x   [lender min: 1.20x — FAILS]
Loan-to-Value (LTV):                75.0%
Gross Rent Multiplier (GRM):        20.2x
Price Per Unit:                     $750,000
1% Rule:                            0.41%   [FAILS — needs $7,500/mo to pass]
Break-Even Rent Per Unit:           $5,231/mo
Current Rent vs. Break-Even:        -$2,131/mo BELOW break-even

--- MARKET BENCHMARKS (Staten Island / NYC Metro) ---
Typical Cap Rate (Staten Island SFR): 4.0–6.0%  → Deal is FAR BELOW at 2.64%
                                      (Outer-borough NYC: between Tier 1 and Tier 2)
Typical GRM:                          14–20x     → Deal is at HIGH END at 20.2x
Target CoC (investor standard):       8–12%      → Deal is deeply below at -14.6%
DSCR Lender Minimum:                  1.20x      → Deal FAILS at 0.42x

--- SAFETY INDEX: 10308 (Great Kills, Staten Island) ---
Overall Safety Grade:       B  (CrimeGrade.org)
Violent Crime Rate:         1.8 per 1,000 residents  (national avg: ~4/1,000)
Property Crime Rate:        8.2 per 1,000 residents  (national avg: ~19/1,000)
Safer than:                 72% of U.S. cities
Crime Trend (3yr):          Stable
Key Finding:                Great Kills is one of Staten Island's safer neighborhoods
                            with crime well below national averages. Low property crime
                            reduces vacancy risk and supports tenant demand — a genuine
                            positive for this deal despite the unfavorable financials.
Source(s):                  CrimeGrade.org, NeighborhoodScout

--- BREAKEVEN & UPSIDE SCENARIOS ---
* Current Status: $2,131/mo BELOW break-even ($5,231 needed vs. $3,100 market)
* At $3,125/unit (+$25): NOI ~$20,048 | Cash Flow ~-$27,149/yr
* Rent Growth (+5%): Rent ~$3,255/unit | Cash Flow ~-$25,666/yr (still deeply negative)
* Value at 5.5% Cap (NYC lower bound): ~$359,000 — $391,000 BELOW asking price
* Value at 6.5% Cap (SI midpoint):     ~$304,000 — $446,000 BELOW asking price

--- RISK FLAGS ---
1. PRICE SEVERELY DISCONNECTED FROM INCOME: NOI of $19,764 supports a value of
   ~$304–$359k at market cap rates. Seller is asking $750,000 — more than double
   the income-based valuation. This is priced for an owner-occupant, not an investor.
2. 1% RULE FAILS BADLY: At $3,100/mo rent, the 1% ratio is 0.41% — less than half
   the minimum threshold. Break-even rent of $5,231/mo is completely unachievable.
3. VINTAGE CONSTRUCTION: 1976 build (49 years old) — CapEx risk is elevated.
   Roof, HVAC, plumbing, electrical all approaching or past typical replacement windows.
4. SINGLE UNIT CONCENTRATION: 100% income from one tenant. Any vacancy = 100% income loss.
5. MULTI-FAMILY CLASSIFICATION MISLEADING: Listed as "multi-family" on Zillow, but this
   is a half duplex — one side of a semi-attached home. There is no second income unit.
   Investors searching for 2-unit income properties should note this distinction clearly.
6. PRICE HISTORY: Last sold in April 2012 for $365,000. Current ask of $750,000 is a
   105% increase in 14 years — well ahead of rental income growth. Yield compression
   makes this uninvestable at asking price.

--- BOTTOM LINE ---
At $750,000, this property fails every investor metric by a wide margin. The income-based
valuation sits between $304,000–$359,000 — the asking price is more than double what the
rental income justifies. Break-even requires $5,231/mo in rent; the market supports $3,100.
No conventional DSCR or investment lender will finance this on rental income alone.

This is a classic owner-occupant-priced home in a high-cost NYC borough. The "multi-family"
label is misleading — there is no second unit generating income. The 1976 construction adds
CapEx risk that further erodes already-thin margins.

If this neighborhood or property type appeals to you, the investment case only works at a
dramatically lower entry price (~$300–$375k), which is not realistic given current market
comps. The only viable buyer here is an owner-occupant who values the location, schools,
and lifestyle — not an investor seeking income.

As a rental investment: DO NOT PROCEED at this price.
========================================================================
DATA CONFIDENCE: HIGH (price, tax, unit count, HOA all confirmed from
  Zillow public record; rent based on 3 independent sources within 5% of each other).
========================================================================
```

---

## What It Analyzes

| Report Section | What You Get |
|---|---|
| Property Overview | Type, vintage, unit mix, utilities structure, HOA, days on market |
| Core Assumptions | Financing terms confirmed before running — all overridable |
| Rent Roll | Per-unit breakdown with annual totals |
| Rent Comp Analysis | 2–3 live market sources, median comp, flags if >15% off market |
| Income & Expenses | Full waterfall: GPI → vacancy → EGI → OpEx → NOI |
| Debt Service & Cash Flow | Monthly P&I, annual cash flow, break-even status |
| Key Metrics | Cap rate, CoC (2 versions), DSCR, LTV, GRM, 1% rule, price/unit — with ✅/❌ benchmarks |
| Market Benchmarks | Deal vs. local cap rates, DSCR minimums, CoC targets |
| Safety Index | Crime grade, violent & property crime rates vs. national avg, trend, investor impact |
| Upside Scenarios | Rent growth scenarios, implied value at market cap rate |
| Risk Flags | 3–6 property-specific risks auto-generated from the data |
| Bottom Line | Plain-English verdict on feasibility and investment thesis |
| **Comparison Report** *(multi-property)* | Side-by-side metrics table, pass/fail scorecard, 🏆 winner per metric, ranked recommendation |

---

## Installation

propertyiq is a Claude Skill — it runs inside Claude.ai on Pro, Team, or Enterprise plans.

**Step 1:** Clone or download this repo

```bash
git clone https://github.com/yourusername/propertyiq.git
```

**Step 2:** In [Claude.ai](https://claude.ai), go to **Settings → Skills**

**Step 3:** Upload the `propertyiq/` folder or the packaged `.skill` file

**Step 4:** Start a new conversation and paste any listing URL

> That's it. No API keys, no configuration, no code to run.

---

## Usage

Paste 1, 2, or 3 listing URLs — propertyiq handles both single analysis and side-by-side comparison:

```
# Single property
/propertyiq https://www.zillow.com/homedetails/...

# Compare two properties
/propertyiq https://www.zillow.com/... https://www.realtor.com/...

# Compare three properties
/propertyiq https://www.zillow.com/... https://www.redfin.com/... https://www.loopnet.com/...

# Natural language also works
Analyze this deal — 4-unit building in Columbus OH, asking $525k [URL]
Is this a good investment? [URL1] [URL2]
```

propertyiq will scrape all listings, pull comps, then show you the proposed assumptions before running. You can override any default before it runs.

**Output files:**
- Single property → one `.md` report (e.g. `propertyiq-123-main-st-cleveland.md`)
- Multi-property → one `.md` per property + `propertyiq-comparison.md` with side-by-side metrics, pass/fail summary, ranking, and plain-English recommendation

---

## Scope

propertyiq covers **small residential investment properties**:

| Property Type | Covered |
|---|---|
| Single-Family Rental (SFR) | ✅ |
| Duplex / Triplex / Quadplex (2–4 units) | ✅ |
| Small Multifamily (5–20 units) | ✅ |
| Large Multifamily (21+ units) | ❌ |
| Short-Term Rentals (Airbnb/VRBO) | ❌ |
| Mobile Home Parks | ❌ |
| Student Housing | ❌ |
| Commercial / Mixed-Use | ❌ |

Out-of-scope property types require fundamentally different underwriting models — different income structures, loan products, and metrics. Future modules may extend propertyiq to cover these categories.

---

## Conservative Defaults by Property Type

propertyiq uses industry-standard conservative inputs — not broker projections.

| Assumption | SFR | 2–4 Unit | 5–20 Unit |
|---|---|---|---|
| Down Payment | 25% | 25% | 25–30% |
| Amortization | 30 yr | 25 yr | 25 yr |
| Vacancy | 5% | 7% | 8% |
| CapEx Reserve | 5–8% gross rent | $100–150/unit/mo | $75–100/unit/mo |
| Maintenance | $75–125/mo | $50–75/unit/mo | $40–60/unit/mo |
| Management Fee | 10% EGI | 8–10% EGI | 8% EGI |
| Interest Rate | Live market rate (searched) | Live market rate | Live commercial rate |

All defaults are shown before running and can be changed.

---

## File Structure

```
propertyiq/
├── README.md                          # You are here
├── SKILL.md                           # Core skill instructions for Claude
├── LICENSE
├── CONTRIBUTING.md
└── references/
    ├── defaults-by-property-type.md   # Full assumptions table with notes
    ├── cap-rate-benchmarks.md         # Cap rate ranges by US metro tier
    └── insurance-benchmarks.md        # Regional landlord insurance estimates

# Output files generated per run:
propertyiq-[address].md                # Individual property report
propertyiq-comparison.md               # Side-by-side comparison (multi-property only)
```

---

## Limitations

- **Site scraping**: Zillow and Redfin occasionally block automated fetches. If a URL fails, propertyiq falls back to a web search on the address automatically.
- **Rent estimates**: When comps are thin, the report flags it and recommends a manual Rentometer check.
- **Short-term rentals**: Models long-term buy-and-hold rentals only. STR/Airbnb potential is flagged but not underwritten.
- **Property scope**: Designed for residential 1–20 units. Large commercial, hotel, or industrial properties are out of scope.
- **Not financial advice**: propertyiq is a screening tool. Always verify inputs with actual lender quotes, insurance bids, and local market data before making an offer.

---

## Contributing

Contributions are welcome. See [CONTRIBUTING.md](CONTRIBUTING.md) for how to get started.

Ideas for improvement:
- STR/Airbnb income modeling
- 5-year cash flow projection table
- Multi-deal comparison mode
- Additional market benchmark data for international markets

---

## License

MIT — free to use, modify, and distribute. See [LICENSE](LICENSE) for details.

---

## Disclaimer

propertyiq is an AI-powered screening tool for informational purposes only. It does not constitute financial, legal, or investment advice. Always conduct full due diligence and consult qualified professionals before making any real estate investment decision.
