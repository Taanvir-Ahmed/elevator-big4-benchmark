# Elevator Big 4 Benchmark (FY2025)

**KONE vs Otis, Schindler and TK Elevator, plus a pro forma view of a combined KONE + TKE**

An Excel model and a 6-slide deck built from the four companies' public FY2025 reports.

## Question
How does KONE compare with its three largest peers on size, business mix and profitability, and what would a combined KONE + TK Elevator look like if the announced deal closes?

## Key findings
| | KONE | Otis | Schindler | TK Elevator |
|---|---|---|---|---|
| Sales (EUR bn) | 11.2 | 12.8 | 11.7 | 9.2 |
| Adjusted EBIT margin | 12.2% | 16.9% | 13.3% | 14.8% |
| Service + modernization share of sales | 64% | 65% | not disclosed | 65% |

1. **Scale:** a combined KONE + TKE would have about EUR 20.4bn in sales, 1.6 times Otis.
2. **Mix:** about two-thirds of sales come from service and modernization, the industry's most profitable business.
3. **Profitability:** KONE has the lowest adjusted EBIT margin of the four. The gap to Otis is worth about EUR 530m a year at KONE's sales.
4. **Deal:** if the full EUR 700m of announced synergies is delivered, the combined margin would reach about 16.8%, level with Otis.

## What's in the repository
| File | Contents |
|---|---|
| `elevator_benchmark_2025.xlsx` | The model: README, Inputs, Raw_Data, Benchmark, ProForma, Checks, Dashboard |
| `elevator_benchmark_deck.pdf` | 6-slide presentation of the findings |

## How the model works
1. **Raw_Data:** 43 reported figures in their original currency, one row each, with the source.
2. **Inputs:** exchange rates (ECB 2025 averages) and a synergy-scenario dropdown (Low / Base / Full).
3. **Benchmark:** converts every figure to EUR with `SUMIFS` lookups and calculates margins, mix, productivity and ranks.
4. **ProForma:** adds KONE and TKE together and shows the combined margin for 0–100% synergy realisation.
5. **Checks:** 10 automated tests, e.g. business lines add up to total sales and the combined sales match the announced EUR 20.5bn. Result: ALL OK.
6. **Dashboard:** charts linked to the model.

Skills used: Excel (SUMIFS, INDEX/MATCH, data validation, Excel tables, charts), financial analysis, PowerPoint storytelling.

## Limitations
- Fiscal years differ: TKE's year ends in September 2025; the others in December 2025.
- "Adjusted EBIT" is each company's own definition. TKE's likely excludes acquisition-related amortisation, so its margin is not strictly like-for-like.
- Otis's Service segment includes modernization; Schindler does not publish revenue by business line.
- The pro forma is a simple sum. It ignores antitrust divestments, integration costs and financing.

*Illustrative analysis based on public company reports. Not investment advice.*

## Sources
- KONE: [Financial Statement Bulletin 2025](https://www.kone.com/global/en/newsroom/releases/2026/financial-statement-bulletin-of-kone-corporation-for-januarydecember-2025-2026-02-06.html), Annual Review 2025
- Otis: [Q4 and full-year 2025 results](https://otisinvestors.com/news/news-details/2026/OTIS-REPORTS-FOURTH-QUARTER-AND-FULL-YEAR-2025-RESULTS/default.aspx)
- Schindler: [Annual Report 2025](https://reports.schindler.com/en/2025/report/group-review/statement-of-the-board-of-directors)
- TK Elevator: [FY2024/25 results](https://www.tkelevator.com/global-en/newsroom/press-releases/tk-elevator-reports-strong-business-momentum-and-record-fy-2024-2025-financial-results-growth-in-service-and-modernization-drove-adjusted-ebitda-up-12-to-a-new-high-of-%E2%82%AC1-6bn-191424.html)
- Deal: [Reuters coverage, 29 Apr 2026](https://www.hl.co.uk/news/kone-to-buy-rival-tk-elevator-in-344-billion-cash-and-stock-deal)
- Exchange rates: [Bank of Finland, 2025 averages](https://www.suomenpankki.fi/en/statistics/interest-rates-and-exchange-rates/exchange-rates/average-annual-exchange-rates-for-the-year-2025/)

---
Author: Tanvir Ahmed · [LinkedIn](https://www.linkedin.com/in/tanvir-ahmed-cu/) · October 2026
