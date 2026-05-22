# BABA Company Financial Data Pack

Generated: 2026-05-23 01:28:19 Asia/Shanghai  
Issuer: Alibaba Group Holding Limited | Ticker: BABA | CIK: 0001577552 | Fiscal year-end: March 31 | Reporting currency: RMB/CNY. Tables are CNY millions unless noted.

## Coverage And Sources

已加载: policy.yaml, catalog-index.md, cheatsheet.md, statement-schema.yaml, contracts/company-financial-data-pack.yaml

- Company profile type: foreign private issuer / ADR; annual source is Form 20-F, interim source is 6-K earnings release.
- Primary structured data: OpenBB `sec` endpoints, SEC companyfacts JSON, SEC 20-F rendered statement R-files.
- Price data: OpenBB `cboe` quote and historical price.
- Latest annual filing: [FY2026 20-F](https://www.sec.gov/Archives/edgar/data/1577552/000119312526231755/baba-20260331.htm); latest official earnings release: [FY2026 Q4/annual 6-K Ex.99.1](https://www.sec.gov/Archives/edgar/data/1577552/000110465926060224/tm2614494d1_ex99-1.htm).
- Recent interim releases: [FY2026 Q3 6-K](https://www.sec.gov/Archives/edgar/data/1577552/000110465926032060/tm269353d1_ex99-1.htm), [FY2026 Q2 6-K](https://www.sec.gov/Archives/edgar/data/1577552/000110465925115949/tm2532163d1_ex99-1.htm), [FY2026 Q1 6-K](https://www.sec.gov/Archives/edgar/data/1577552/000110465925085638/tm2524743d1_ex99-1.htm), [FY2025 Q4 6-K](https://www.sec.gov/Archives/edgar/data/1577552/000110465925049400/tm2515233d1_ex99-1.htm).
- SEC filing trail: latest 20-F filed 2026-05-20 for FY ended 2026-03-31; latest annual/Q4 6-K Exhibit 99.1 filed 2026-05-13.

## Financial Snapshot

- FY2026 revenue was RMB1,023.7bn, +3% reported YoY; the issuer states like-for-like revenue excluding disposed Sun Art and Intime would have grown 11%.
- FY2026 operating income fell 64% to RMB50.2bn as adjusted EBITA fell 56% to RMB76.4bn; management attributed the decline mainly to investments in quick commerce, user experience and technology businesses.
- FY2026 net income attributable to parent was RMB103.6bn; diluted EPS was RMB5.50 per ordinary share, or RMB44.00 per ADS.
- FY2026 operating cash flow was RMB76.2bn; issuer-defined free cash flow was a RMB46.6bn outflow, mainly due to quick commerce investment and cloud infrastructure expenditure. Canonical CFO plus R8 PP&E/land-use capex was a RMB49.9bn outflow.
- As of 2026-03-31, cash and other liquid investments were RMB520.8bn per the Q4 release; total liabilities were RMB783.3bn and shareholders' equity was RMB1,060.9bn.
- CBOE quote via OpenBB: BABA last price $130.230 as of 2026-05-22 13:11:44; implied market cap about $302,466mm using 18.580bn ordinary shares / 8 ADS ratio.

## Four Statements And Notes

### 3.1 Income Statement — Annual (FY-4..LFY)

| standard_line_item | FY2022 | FY2023 | FY2024 | FY2025 | FY2026 | xbrl_tag_or_formula | mapping_status | source |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| Revenue | 853,062 | 868,687 | 941,168 | 996,347 | 1,023,670 | Revenues | reported | SEC companyfacts / 20-F |
| Cost of Revenue | 539,450 | 549,695 | 586,323 | 598,285 | 616,136 | CostOfRevenue | reported | SEC companyfacts / 20-F |
| Gross Profit | 313,612 | 318,992 | 354,845 | 398,062 | 407,534 | Revenues - CostOfRevenue | derived | SEC companyfacts / 20-F |
| Research and Development / Product Development | 55,465 | 56,744 | 52,256 | 57,151 | 66,533 | ResearchAndDevelopmentExpense | reported | SEC companyfacts / 20-F |
| SG&A | 151,721 | 145,679 | 157,126 | 188,260 | 278,105 | SellingAndMarketingExpense + GeneralAndAdministrativeExpense | derived | SEC companyfacts / 20-F |
| Operating Income | 69,638 | 100,351 | 113,350 | 140,905 | 50,150 | OperatingIncomeLoss | reported | SEC companyfacts / 20-F |
| Interest Expense | 4,909 | 5,918 | 7,947 | 9,596 | 9,793 | InterestExpense | reported | SEC companyfacts / 20-F |
| Pretax Income | 59,550 | 89,185 | 101,596 | 155,455 | 129,387 | IncomeLossFromContinuingOperationsBeforeIncomeTaxes... | reported | SEC companyfacts / 20-F |
| Tax Expense | 26,815 | 15,549 | 22,529 | 35,445 | 30,045 | IncomeTaxExpenseBenefit | reported | SEC companyfacts / 20-F |
| Net Income Attributable to Parent | 62,249 | 72,783 | 80,009 | 130,109 | 103,592 | NetIncomeLoss | reported | SEC companyfacts / 20-F |
| Diluted EPS (CNY/share) | 2.8 | 3.4 | 3.9 | 6.7 | 5.5 | EarningsPerShareDiluted | reported | SEC companyfacts / 20-F |
| Diluted Shares (million ordinary shares) | 21,787 | 21,114 | 20,359 | 19,318 | 19,235 | WeightedAverageNumberOfDilutedSharesOutstanding | reported | SEC companyfacts / 20-F |

### 3.2 Income Statement — Last 5 Standalone Quarters

| standard_line_item | FY25 Q4 | FY26 Q1 | FY26 Q2 | FY26 Q3 | FY26 Q4 | xbrl_tag_or_formula | mapping_status | source |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| Revenue | 236,454 | 247,652 | 247,795 | 284,843 | 243,380 | 6-K table row: Revenue | reported | 6-K Ex.99.1 |
| Cost of Revenue | -145,626 | -136,429 | -150,781 | -169,534 | -159,392 | 6-K table row: Cost of revenue | reported | 6-K Ex.99.1 |
| Gross Profit | 90,828 | 111,223 | 97,014 | 115,309 | 83,988 | Revenue + Cost of revenue (cost row uses filing-sign negative) | derived | 6-K Ex.99.1 |
| Product Development | -14,934 | -15,001 | -17,095 | -15,480 | -18,957 | 6-K table row: Product development expenses | reported | 6-K Ex.99.1 |
| SG&A | -46,510 | -60,576 | -73,876 | -80,289 | -63,364 | Sales and marketing + G&A | derived | 6-K Ex.99.1 |
| Operating Income | 28,465 | 34,988 | 5,365 | 10,645 | -848 | 6-K table row: Income from operations | reported | 6-K Ex.99.1 |
| Pretax Income | 18,473 | 50,234 | 23,921 | 23,875 | 31,357 | 6-K table row: Income before income tax... | reported | 6-K Ex.99.1 |
| Tax Expense | -6,854 | -8,865 | -5,550 | -8,460 | -7,170 | 6-K table row: Income tax expenses | reported | 6-K Ex.99.1 |
| Net Income | 11,973 | 42,382 | 20,612 | 15,631 | 23,502 | 6-K table row: Net income | reported | 6-K Ex.99.1 |
| Diluted EPS (CNY/share) | 0.7 | 2.2 | 1.1 | 0.7 | 1.3 | 6-K table row: diluted EPS | reported | 6-K Ex.99.1 |
| Diluted Shares (million ordinary shares) | 19,153 | 19,142 | 19,168 | 19,310 | 19,319 | 6-K table row: diluted share denominator | reported | 6-K Ex.99.1 |

### 3.3 Balance Sheet — Annual

| standard_line_item | FY2022 | FY2023 | FY2024 | FY2025 | FY2026 | xbrl_tag_or_formula | mapping_status | source |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| Cash and Equivalents | 189,898 | 193,086 | 248,125 | 145,487 | 131,530 | CashAndCashEquivalentsAtCarryingValue | reported | SEC companyfacts / 20-F |
| Short-term Investments | n/a | n/a | n/a | 228,826 | 155,310 | ShortTermInvestments | reported | SEC companyfacts / 20-F |
| Accounts Receivable | 32,813 | 32,134 | 30,686 | 31,172 | 36,020 | AccountsReceivableNetCurrent | reported | SEC companyfacts / 20-F |
| Inventory | data_unavailable_after_sec_check | data_unavailable_after_sec_check | data_unavailable_after_sec_check | data_unavailable_after_sec_check | data_unavailable_after_sec_check | InventoryNet | data_unavailable_after_sec_check | SEC companyfacts tag absent; balance sheet groups it in other current assets |
| Current Assets | 638,535 | 697,966 | 752,864 | 674,049 | 610,769 | AssetsCurrent | reported | SEC companyfacts / 20-F |
| PP&E, Net | 171,806 | 176,031 | 185,161 | 203,348 | 282,699 | PropertyPlantAndEquipmentNet | reported | SEC companyfacts / 20-F |
| Goodwill and Intangibles | 328,812 | 315,004 | 286,629 | 276,412 | 264,361 | Goodwill + FiniteLivedIntangibleAssetsNet | derived | SEC companyfacts / 20-F |
| Total Assets | 1,695,553 | 1,753,044 | 1,764,829 | 1,804,227 | 1,909,570 | Assets | reported | SEC companyfacts / 20-F |
| Accounts Payable + Accrued Liabilities | 271,460 | 275,950 | 297,883 | 332,537 | 359,893 | AccountsPayableAndAccruedLiabilitiesCurrent | reported | SEC companyfacts / 20-F |
| Current Liabilities | 383,784 | 385,351 | 421,507 | 435,346 | 476,398 | LiabilitiesCurrent | reported | SEC companyfacts / 20-F |
| Debt (bank borrowings + notes) | 141,344 | 156,554 | 154,524 | 230,703 | 259,996 | 20-F R5 current bank + non-current bank + senior notes + convertible/exchangeable | reported/derived | SEC rendered 20-F balance sheet R5 fallback |
| Total Liabilities | 613,360 | 630,123 | 652,230 | 714,121 | 783,300 | Liabilities | reported | SEC companyfacts / 20-F |
| Shareholders' Equity | 948,479 | 989,657 | 986,544 | 1,009,858 | 1,060,886 | StockholdersEquity | reported | SEC companyfacts / 20-F |
| Common Stock and APIC | 410,506 | 416,880 | 397,999 | 381,379 | 385,086 | AdditionalPaidInCapital | reported | SEC companyfacts / 20-F |
| Retained Earnings | 563,557 | 599,028 | 597,897 | 645,478 | 708,382 | RetainedEarningsUnappropriated | reported | SEC companyfacts / 20-F |
| Treasury Stock | 2,221 | 28,763 | 27,684 | 36,329 | 36,141 | TreasuryStockValue | reported | SEC companyfacts / 20-F |
| Noncontrolling Interest | 124,059 | 123,406 | 115,327 | 68,535 | 57,539 | MinorityInterest | reported | SEC companyfacts / 20-F |

### 3.4 Balance Sheet — Last 5 Quarter-End Snapshots

| standard_line_item | FY25 Q4 | FY26 Q1 | FY26 Q2 | FY26 Q3 | FY26 Q4 | xbrl_tag_or_formula | mapping_status | source |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| Cash and Equivalents | 145,487 | 183,120 | 135,069 | 128,174 | 131,530 | 6-K balance sheet row | reported | 6-K Ex.99.1 |
| Short-term Investments | 228,826 | 191,737 | 193,246 | 179,955 | 155,310 | 6-K balance sheet row | reported | 6-K Ex.99.1 |
| Accounts Receivable | data_unavailable_after_official_source_check | data_unavailable_after_official_source_check | data_unavailable_after_official_source_check | data_unavailable_after_official_source_check | data_unavailable_after_official_source_check | not separately disclosed in quarterly 6-K balance summary | data_unavailable_after_sec_check | Quarterly 6-K balance tables aggregate receivables in other assets |
| Current Assets | 674,049 | 686,071 | 646,619 | 612,216 | 610,769 | 6-K balance sheet row | reported | 6-K Ex.99.1 |
| PP&E, Net | 203,348 | 220,835 | 246,539 | 254,478 | 282,699 | 6-K balance sheet row | reported | 6-K Ex.99.1 |
| Goodwill and Intangibles | 276,412 | 275,703 | 274,980 | 264,060 | 264,361 | Goodwill + intangible assets, net | derived | 6-K Ex.99.1 |
| Total Assets | 1,804,227 | 1,847,085 | 1,883,880 | 1,878,299 | 1,909,570 | 6-K balance sheet row | reported | 6-K Ex.99.1 |
| AP + Accrued Liabilities | 332,537 | 371,624 | 340,769 | 351,293 | 359,893 | 6-K balance sheet row | reported | 6-K Ex.99.1 |
| Current Liabilities | 435,346 | 473,627 | 444,137 | 459,811 | 476,398 | 6-K balance sheet row | reported | 6-K Ex.99.1 |
| Total Liabilities | 714,121 | 753,766 | 772,095 | 772,371 | 783,300 | 6-K balance sheet row | reported | 6-K Ex.99.1 |
| Shareholders' Equity | 1,009,858 | 1,013,672 | 1,032,495 | 1,039,655 | 1,060,886 | 6-K balance sheet row | reported | 6-K Ex.99.1 |
| Noncontrolling Interest | 68,535 | 69,726 | 69,406 | 58,522 | 57,539 | 6-K balance sheet row | reported | 6-K Ex.99.1 |

### 3.5 Cash Flow Statement — Annual

| standard_line_item | FY2022 | FY2023 | FY2024 | FY2025 | FY2026 | xbrl_tag_or_formula | mapping_status | source |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| Net Income | 47,079 | 65,573 | 71,332 | 125,976 | 102,127 | ProfitLoss | reported | SEC companyfacts / 20-F |
| D&A | 25,470 | 24,654 | 23,344 | 24,515 | 34,963 | DepreciationDepletionAndAmortization | reported | SEC companyfacts / 20-F |
| Stock-based Compensation | 23,971 | 30,831 | 18,546 | 13,970 | 11,180 | AllocatedShareBasedCompensationExpense | reported | SEC companyfacts / 20-F |
| Change in Working Capital | data_unavailable_after_sec_check | data_unavailable_after_sec_check | data_unavailable_after_sec_check | data_unavailable_after_sec_check | data_unavailable_after_sec_check | R8 component-sum not rendered in pack | data_unavailable_after_sec_check | Official R-file has components; not mapped to single XBRL tag |
| Cash from Operations | 142,759 | 199,752 | 182,593 | 163,509 | 76,213 | NetCashProvidedByUsedInOperatingActivities | reported | SEC companyfacts / 20-F |
| Capex | -53,309 | -34,330 | -32,087 | -85,972 | -126,063 | 20-F R8 row: Land use rights, property and equipment | reported | SEC rendered 20-F cash flow R8 fallback |
| Free Cash Flow (CFO + capex) | 89,450 | 165,422 | 150,506 | 77,537 | -49,850 | NetCashProvidedByUsedInOperatingActivities + R8 capex | derived | SEC companyfacts + SEC rendered 20-F R8 fallback |
| Cash from Investing | -198,592 | -135,506 | -21,824 | -185,415 | -67,336 | NetCashProvidedByUsedInInvestingActivities | reported | SEC companyfacts / 20-F |
| Share Repurchases | 61,225 | 74,746 | 88,745 | 86,662 | 7,638 | PaymentsForRepurchaseOfCommonStock | reported | SEC companyfacts / 20-F |
| Dividends Paid | 0 | 0 | 17,946 | 29,077 | 33,732 | PaymentsOfDividends | reported | SEC companyfacts / 20-F |
| Cash from Financing | -64,449 | -65,619 | -108,244 | -76,215 | -20,573 | NetCashProvidedByUsedInFinancingActivities | reported | SEC companyfacts / 20-F |

### 3.6 Cash Flow Statement — Last 5 Standalone Quarters

| standard_line_item | FY25 Q4 | FY26 Q1 | FY26 Q2 | FY26 Q3 | FY26 Q4 | xbrl_tag_or_formula | mapping_status | source |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| Net Income | 11,973 | 42,382 | 20,612 | 15,631 | 23,502 | 6-K income statement row | reported | 6-K Ex.99.1 |
| D&A | data_unavailable_after_official_source_check | data_unavailable_after_official_source_check | data_unavailable_after_official_source_check | data_unavailable_after_official_source_check | data_unavailable_after_official_source_check | not separately disclosed in quarterly cash-flow summary | data_unavailable_after_sec_check | Quarterly 6-K cash-flow tables are summarized |
| Stock-based Compensation | data_unavailable_after_official_source_check | data_unavailable_after_official_source_check | data_unavailable_after_official_source_check | data_unavailable_after_official_source_check | data_unavailable_after_official_source_check | not separately disclosed in quarterly cash-flow summary | data_unavailable_after_sec_check | Quarterly 6-K cash-flow tables are summarized |
| Cash from Operations | 27,520 | 20,672 | 10,099 | 36,032 | 9,410 | 6-K cash-flow summary row | reported | 6-K Ex.99.1 |
| Capex | -23,993 | -38,629 | -31,428 | -25,376 | -26,588 | 6-K free-cash-flow table: purchase of property and equipment | reported | 6-K Ex.99.1 |
| Free Cash Flow (issuer definition) | 3,743 | -18,815 | -21,840 | 11,346 | -17,300 | 6-K non-GAAP free cash flow row | reported | 6-K Ex.99.1 |
| Cash from Investing | -39,547 | 18,328 | -69,652 | -25,716 | 9,704 | 6-K cash-flow summary row | reported | 6-K Ex.99.1 |
| Cash from Financing | -4,102 | -2,731 | 10,902 | -13,742 | -15,002 | 6-K cash-flow summary row | reported | 6-K Ex.99.1 |

### 3.7 Statement of Stockholders' Equity — Annual

| standard_line_item | FY2022 | FY2023 | FY2024 | FY2025 | FY2026 | xbrl_tag_or_formula | mapping_status | source |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| Beginning Equity | 937,470 | 948,479 | 989,657 | 986,544 | 1,009,858 | prior-year StockholdersEquity | derived | SEC companyfacts / 20-F |
| Net Income Attributable to Parent | 62,249 | 72,783 | 80,009 | 130,109 | 103,592 | NetIncomeLoss | reported | SEC companyfacts / 20-F |
| Other Comprehensive Income | -16,097 | 23,835 | 14,385 | -191 | -16,813 | OtherComprehensiveIncomeLossNetOfTax | reported | SEC companyfacts / 20-F |
| Share-based Compensation in Equity | 23,971 | 30,831 | 18,546 | 13,970 | 11,180 | AllocatedShareBasedCompensationExpense | reported/approx | SEC companyfacts / 20-F |
| Share Issuance | data_unavailable_after_sec_check | data_unavailable_after_sec_check | data_unavailable_after_sec_check | data_unavailable_after_sec_check | data_unavailable_after_sec_check | readable in R7, not standardized in companyfacts | data_unavailable_after_sec_check | SEC rendered equity R7 has line; not normalized across all years |
| Share Repurchases | 61,225 | 74,746 | 88,745 | 86,662 | 7,638 | PaymentsForRepurchaseOfCommonStock | reported/CF proxy | SEC companyfacts / 20-F |
| Dividends Declared | n/a | n/a | 18,542 | 29,340 | 34,031 | Dividends | reported | SEC companyfacts / 20-F |
| Other / Cumulative-effect Adjustments | data_unavailable_after_sec_check | data_unavailable_after_sec_check | data_unavailable_after_sec_check | data_unavailable_after_sec_check | data_unavailable_after_sec_check | R7 residual needed for exact footing | data_unavailable_after_sec_check | Exact rollforward requires R7 line-by-line normalization |
| Ending Equity | 948,479 | 989,657 | 986,544 | 1,009,858 | 1,060,886 | StockholdersEquity | reported | SEC companyfacts / 20-F |

### 3.8 Notes Index

| note_id | note_topic | note_status | source_filing | source_endpoint_or_url | extracted_point | affected_statement_rows |
| --- | --- | --- | --- | --- | --- | --- |
| revenue_recognition | 收入确认 | extracted | FY2026 20-F / FY2026 6-K | SEC 20-F and Ex.99.1 | Alibaba reports platform customer management, direct sales, quick commerce, cloud and other revenue streams; direct-sales/logistics revenue is gross presentation where inventory/cost of inventory is recorded. | revenue, accounts_receivable |
| segment_disclosure | 分部披露 | extracted | FY2026 6-K | Q4 FY2026 Ex.99.1 | FY2026 segment revenue: China e-commerce RMB554.2bn, AIDC RMB144.2bn, Cloud RMB158.1bn, All others RMB254.4bn before elimination. | revenue, operating_income |
| debt_and_liquidity | 债务与流动性 | extracted | FY2026 20-F / FY2026 6-K | SEC R5 / Ex.99.1 | Cash and other liquid investments RMB520.8bn; debt proxy from R5 bank borrowings + notes + convertibles/exchangeables RMB260.0bn. | debt, cash_and_equivalents, interest_expense |
| leases_and_commitments | 租赁、承诺与或有事项 | extracted | FY2026 20-F | SEC 20-F notes | Lease/commitment details are in the 20-F notes; canonical pack did not normalize lease maturity rows into the statement tables. | pp_and_e_net, total_liabilities |
| share_based_compensation | 股权激励 | extracted | FY2026 20-F / FY2026 6-K | SEC companyfacts and Ex.99.1 | FY2026 share-based compensation expense in cost/expense table was RMB14.8bn; cash-flow equity-settled SBC row was RMB11.2bn. | stock_based_compensation, diluted_shares |
| buybacks_and_dividends | 回购与股息 | extracted | FY2026 20-F / FY2026 6-K | SEC R7/R8 and companyfacts | FY2026 cash repurchases RMB7.6bn; dividends paid RMB33.7bn; dividends declared RMB34.0bn. | share_repurchases, dividends, shareholders_equity |
| income_taxes | 所得税 | extracted | FY2026 20-F / FY2026 6-K | SEC companyfacts | FY2026 tax expense RMB30.0bn; pretax income RMB129.4bn; implied ETR about 23.2%. | tax_expense |
| subsequent_events_or_guidance | 期后事项或管理层指引 | extracted_gap | FY2026 Q4 6-K | Ex.99.1 webcast and safe-harbor section | No quantitative forward-guidance table was found in the official release; forward-looking content is qualitative and tied to the earnings webcast. | guidance |

## Management Discussion And Guidance

> Sources distilled in this section:
> - Latest annual filing: https://www.sec.gov/Archives/edgar/data/1577552/000119312526231755/baba-20260331.htm
> - FY2026 Q4 and annual results release: https://www.sec.gov/Archives/edgar/data/1577552/000110465926060224/tm2614494d1_ex99-1.htm
> - FY2026 Q3 results release: https://www.sec.gov/Archives/edgar/data/1577552/000110465926032060/tm269353d1_ex99-1.htm
> - FY2026 Q2 results release: https://www.sec.gov/Archives/edgar/data/1577552/000110465925115949/tm2532163d1_ex99-1.htm
> - FY2026 Q1 results release: https://www.sec.gov/Archives/edgar/data/1577552/000110465925085638/tm2524743d1_ex99-1.htm
> - FY2025 Q4 and annual results release: https://www.sec.gov/Archives/edgar/data/1577552/000110465925049400/tm2515233d1_ex99-1.htm
> - SEC companyfacts JSON: https://data.sec.gov/api/xbrl/companyfacts/CIK0001577552.json


### 4.1 Quarter Headline

March quarter FY2026 revenue was RMB243.4bn, +3% reported YoY and +11% like-for-like excluding Sun Art and Intime. Loss from operations was RMB0.8bn versus operating income of RMB28.5bn in the prior-year quarter. Net income was RMB23.5bn, but non-GAAP net income was only RMB0.1bn, reflecting the pressure from strategic investments and non-GAAP exclusions.

### 4.2 Business Line YoY

| segment | Q4 FY2026 revenue | Q4 YoY | FY2026 revenue | FY YoY | delta flag / attribution |
| --- | --- | --- | --- | --- | --- |
| Alibaba China E-commerce Group | 122,220 | +6% | 554,217 | +9% | Quick commerce +57% Q4; customer management +1% reported / +8% like-for-like |
| AIDC | 35,429 | +6% | 144,170 | +9% | Retail +5% Q4; wholesale +9% Q4 |
| Cloud Intelligence Group | 41,626 | +38% | 158,132 | +34% | AI-related product revenue triple-digit growth for the 11th consecutive quarter |
| All others | 65,459 | -21% | 254,367 | -25% | Disposed Sun Art/Intime and Cainiao decrease weighed on reported revenue |

### 4.3 Margin & Cost Story

Gross profit in FY2026 was RMB407.5bn, broadly flat versus FY2025, but operating income compressed sharply because sales and marketing rose to RMB245.0bn. In the March quarter, sales and marketing expense was RMB53.4bn, 21.9% of revenue. Management explicitly tied the adjusted EBITA decline to investments in quick commerce, technology businesses and user experiences, partly offset by Cloud/customer-management growth and operating efficiencies.

### 4.4 Capital & Liquidity

The balance sheet remains liquid: cash and equivalents were RMB131.5bn and short-term investments were RMB155.3bn at 2026-03-31; the issuer's broader cash and other liquid investments measure was RMB520.8bn. Debt proxy from 20-F R5 was about RMB260.0bn, mainly unsecured senior notes, bank borrowings, convertible notes and exchangeable bonds. FY2026 dividends paid were RMB33.7bn, while ordinary share repurchases were only RMB7.6bn versus RMB86.7bn in FY2025.

### 4.5 Tone Shift vs Prior Quarter / Prior Annual

The tone shifted from recovery/efficiency to investment absorption. Reported revenue growth stayed low-single-digit, but like-for-like growth was materially higher after adjusting for disposed businesses. Cloud commentary strengthened: AI-related product revenue sustained triple-digit growth for the eleventh consecutive quarter, while quick commerce moved from growth initiative to major margin and FCF drag.

### 4.6 Risks & Management Topics

Key management topics are capital allocation between AI/cloud and quick commerce, monetization of China e-commerce customer management, disposal effects from Sun Art/Intime, infrastructure capex intensity, and equity-investment fair-value volatility. FY2026 net income benefited from investment gains, while operating income and free cash flow show the underlying investment burden more directly.

### 4.7 Forward Guidance

Verbal/qualitative-only caveat: the latest official FY2026 Q4 6-K does not contain a quantitative Outlook/Guidance table. It provides webcast/conference-call registration links and safe-harbor language for forward-looking statements, but no revenue, margin, capex or EPS ranges. Therefore, no issuer-provided quantitative forward estimates are included in this pack.

## Price And Valuation Helpers

| metric | value | formula / source |
| --- | --- | --- |
| Last price | $130.230 | OpenBB/CBOE quote timestamp 2026-05-22 13:11:44 |
| Market cap | $302,466mm | last price × 18.580bn ordinary shares / 8 ADS |
| FY2026 P/E | 20.4x | $130.230 / FY2026 diluted EPS per ADS $6.38 |
| FY2026 P/S | 2.0x | market cap / FY2026 revenue $148,401mm |
| FY2026 P/B | 2.0x | market cap / FY2026 shareholders' equity $153,796mm |
| EV / FY2026 sales | 1.8x | market cap + debt proxy - cash and other liquid investments |

Price performance using CBOE historical close plus latest quote:

| window | base date | base close | return to latest quote |
| --- | --- | --- | --- |
| 1M | 2026-04-22 | 136.42 | -4.5% |
| 3M | 2026-02-20 | 154.45 | -15.7% |
| YTD | 2025-12-31 | 146.58 | -11.2% |
| 1Y | 2025-05-22 | 121.48 | 7.2% |

## Optional Ownership, Short, And Options Data

Not pulled in this pack. The company-financial-data-pack mandatory scope was satisfied with SEC financials, filings, MD&A, companyfacts, CBOE quote and price history. FINRA short interest, SEC 13F and options chain can be added as a separate market-positioning appendix.

## Analyst Commentary

BABA's FY2026 headline revenue growth understates core operating momentum because disposed Sun Art/Intime assets create a reported-growth drag; the issuer's like-for-like revenue growth was 11% for both Q4 and FY2026. The more important issue is not demand but reinvestment intensity: sales and marketing nearly doubled YoY in FY2026, Cloud capex rose, and issuer-defined FCF swung to a RMB46.6bn outflow.

The stock is no longer optically cheap on trailing GAAP earnings at roughly 20x FY2026 diluted ADS EPS, but EV/sales near 1.8x is more forgiving because the balance sheet is cash-rich. The investment question is whether quick commerce losses moderate before Cloud/AI growth and customer-management monetization become large enough to restore EBITA margin.

## Data Gaps

- Quarterly 6-K balance sheets do not separately disclose accounts receivable or inventory; these are marked unavailable rather than inferred.
- Quarterly D&A, SBC and detailed working-capital rows are not standardized in BABA's 6-K cash-flow summaries; annual values are available via 20-F/companyfacts/R-files.
- Exact five-year shareholders' equity rollforward components require full R7 normalization; this pack includes reported ending balances and major companyfacts/R-file proxies, with residual rows marked unavailable.
- No quantitative forward guidance was disclosed in the latest official release; this is a source gap, not an estimate.

## TOOLCHAIN

```text
[TOOLCHAIN]
OpenBB:
  contract: company-financial-data-pack.yaml
  mandatory_pass: true
  forbidden_provider_calls: 0
  calls:
    - endpoint: obb.regulators.sec.cik_map
      provider: sec
      attempts: 1
      success: 1
      failed: 0
    - endpoint: obb.equity.fundamental.filings
      provider: sec
      attempts: 2
      success: 2
      failed: 0
    - endpoint: obb.equity.fundamental.management_discussion_analysis
      provider: sec
      attempts: 1
      success: 1
      failed: 0
    - endpoint: obb.equity.compare.company_facts
      provider: sec
      attempts: 5
      success: 3
      failed: 2
    - endpoint: obb.equity.price.quote
      provider: cboe
      attempts: 2
      success: 2
      failed: 0
    - endpoint: obb.equity.price.historical
      provider: cboe
      attempts: 2
      success: 2
      failed: 0
SEC:
  companyfacts_json: success
  rendered_statement_rfiles: success
  official_6k_exhibits: success
WebAccess:
  used: false
  calls: 0
  official_sources_only: true
```
