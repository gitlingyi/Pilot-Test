# Microsoft Corporation (NASDAQ: MSFT) — Company Financial Data Pack

_Build date: 2026-05-18 (UTC). Currency: USD. Scale: USD millions unless noted._
_Reporting issuer: US domestic registrant (10-K / 10-Q). Fiscal year ends June 30. Taxonomy: us-gaap._

## Coverage And Sources

| Item | Value |
|---|---|
| Entity name | MICROSOFT CORPORATION |
| CIK | 0000789019 |
| Ticker | MSFT |
| Issuer profile | us_domestic_company |
| Fiscal year end | June 30 |
| Latest fiscal year (FY) | FY2025 (ended 2025-06-30) |
| Latest interim quarter | Q3 FY2026 (ended 2026-03-31) |
| Annual periods presented | FY2021, FY2022, FY2023, FY2024, FY2025 |
| Quarterly periods presented | Q3 FY2025, Q4 FY2025, Q1 FY2026, Q2 FY2026, Q3 FY2026 (Q4 = standalone fiscal quarter; **Q4 derived as `FY − YTD_Q3`** for IS/CF, BS uses 10-K period-end snapshot) |
| Primary structured source | SEC companyfacts XBRL via `D:\GoodAI\claude\.claude\shared\sec\companyfacts.py` (helper wraps OpenBB `obb.equity.compare.company_facts` + raw `data.sec.gov` JSON) |
| Statement-level source (CF combined line, SoE, notes) | SEC 10-K / 10-Q rendered financial statements (R-files located via `FilingSummary.xml`) — FY2025 10-K (acc 0000950170-25-100235), FY2023 10-K, and Q2/Q3 FY25 + Q1/Q2/Q3 FY26 10-Qs. Used for the cash-flow "Depreciation, amortization, and other" line, the Stockholders' Equity rollforward, and note figures — these are company XBRL extensions absent from companyfacts. |
| Filings source | `obb.equity.fundamental.filings` (sec) — 10 10-Q + assorted filings |
| MD&A source (latest) | `obb.equity.fundamental.management_discussion_analysis` (sec) — latest 10-Q |
| MD&A source (prior)  | SEC EDGAR HTML for prior 10-Q (https://www.sec.gov/Archives/edgar/data/789019/000119312526027207/msft-20251231.htm) parsed via ITEM 2 regex |
| Price source | `obb.equity.price.historical` / `quote` (cboe) |

**Period-key methodology**: each XBRL value is keyed by its `end` date — FY filtered 350–380 days, 3M-quarter 85–95 days, YTD ~92/184/273 days. Comparative-period rows tagged with the filer's current `fy/fp` in the JSON are de-duplicated by end-date, not by `fy/fp` strings. See `shared/sec/companyfacts.py` for the canonical implementation.

## Financial Snapshot

| Metric | LFY (FY2025) | TTM (through 2026-03-31) | LFY YoY |
|---|---|---|---|
| Revenue (USD M) | 281,724 | 318,273 | +14.9% |
| Gross Profit (USD M) | 193,893 | 217,410 | +13.4% |
| Operating Income (USD M) | 128,528 | 148,957 | +17.4% |
| Net Income (USD M) | 101,832 | 125,216 | +15.5% |
| Cash from Operations (USD M) | 136,162 | 170,141 | +14.9% |
| Free Cash Flow (USD M) | 71,611 | 72,916 | −3.3% |
| Diluted EPS (USD) | 13.64 | 16.77 | +15.6% |
| Gross Margin | 68.8% | 68.3% | −94 bps |
| Operating Margin | 45.6% | 46.8% | +98 bps |
| Net Margin | 36.1% | 39.3% | +19 bps |

## Four Statements And Notes

### 3.1 Income Statement — Annual (USD millions; EPS in USD; shares in millions)

| Line Item | FY2021 | FY2022 | FY2023 | FY2024 | FY2025 | XBRL Tag / Formula | Mapping | Source |
|---|---|---|---|---|---|---|---|---|
| Revenue | 168,088 | 198,270 | 211,915 | 245,122 | 281,724 | `RevenueFromContractWithCustomerExcludingAssessedTax` | reported | OpenBB `obb.equity.compare.company_facts` (sec) + SEC companyfacts JSON |
| Cost of Revenue | 52,232 | 62,650 | 65,863 | 74,114 | 87,831 | `CostOfGoodsAndServicesSold` | reported | OpenBB `obb.equity.compare.company_facts` (sec) + SEC companyfacts JSON |
| Gross Profit | 115,856 | 135,620 | 146,052 | 171,008 | 193,893 | `GrossProfit` | reported/derived | OpenBB `obb.equity.compare.company_facts` (sec) + SEC companyfacts JSON |
| Research & Development | 20,716 | 24,512 | 27,195 | 29,510 | 32,488 | `ResearchAndDevelopmentExpense` | reported | OpenBB `obb.equity.compare.company_facts` (sec) + SEC companyfacts JSON |
| Sales & Marketing | 20,117 | 21,825 | 22,759 | 24,456 | 25,654 | `SellingAndMarketingExpense` | reported | SEC companyfacts JSON (CIK 0000789019) |
| General & Administrative | 5,107 | 5,900 | 7,575 | 7,609 | 7,223 | `GeneralAndAdministrativeExpense` | reported | OpenBB `obb.equity.compare.company_facts` (sec) + SEC companyfacts JSON |
| Operating Income | 69,916 | 83,383 | 88,523 | 109,433 | 128,528 | `OperatingIncomeLoss` | reported | OpenBB `obb.equity.compare.company_facts` (sec) + SEC companyfacts JSON |
| Other Income / (Expense), Net | 98 | -32 | -223 | -1,319 | -4,725 | `OtherNonoperatingIncomeExpense` | reported | SEC companyfacts JSON (CIK 0000789019) |
| Pretax Income | 71,102 | 83,716 | 89,311 | 107,787 | 123,627 | `IncomeLossFromContinuingOperationsBeforeIncomeTaxesExtraordinaryItemsNoncontrollingInterest` | reported | OpenBB `obb.equity.compare.company_facts` (sec) + SEC companyfacts JSON |
| Income Tax Expense | 9,831 | 10,978 | 16,950 | 19,651 | 21,795 | `IncomeTaxExpenseBenefit` | reported | OpenBB `obb.equity.compare.company_facts` (sec) + SEC companyfacts JSON |
| Net Income | 61,271 | 72,738 | 72,361 | 88,136 | 101,832 | `NetIncomeLoss` | reported | OpenBB `obb.equity.compare.company_facts` (sec) + SEC companyfacts JSON |
| Diluted EPS | 8.05 | 9.65 | 9.68 | 11.80 | 13.64 | `EarningsPerShareDiluted` | reported | OpenBB `obb.equity.compare.company_facts` (sec) + SEC companyfacts JSON |
| Diluted Shares (M) | 7,608 | 7,540 | 7,472 | 7,469 | 7,465 | `WeightedAverageNumberOfDilutedSharesOutstanding` | reported | OpenBB `obb.equity.compare.company_facts` (sec) + SEC companyfacts JSON |

### 3.2 Income Statement — Last 5 Standalone Quarters (3M periods; Q4 derived from FY − YTD_Q3)

| Line Item | Q3 FY2025<br>(2025-03-31) | Q4 FY2025*<br>(2025-06-30) | Q1 FY2026<br>(2025-09-30) | Q2 FY2026<br>(2025-12-31) | Q3 FY2026<br>(2026-03-31) | XBRL Tag / Formula | Mapping | Source |
|---|---|---|---|---|---|---|---|---|
| Revenue | 70,066 | 76,441 | 77,673 | 81,273 | 82,886 | `RevenueFromContractWithCustomerExcludingAssessedTax` | reported (Q1–Q3); derived (Q4 = FY − YTD_Q3) | OpenBB `obb.equity.compare.company_facts` (sec) + SEC companyfacts JSON |
| Cost of Revenue | 21,919 | 24,014 | 24,043 | 25,978 | 26,828 | `CostOfGoodsAndServicesSold` | reported (Q1–Q3); derived (Q4 = FY − YTD_Q3) | OpenBB `obb.equity.compare.company_facts` (sec) + SEC companyfacts JSON |
| Gross Profit | 48,147 | 52,427 | 53,630 | 55,295 | 56,058 | `GrossProfit` | derived | OpenBB `obb.equity.compare.company_facts` (sec) + SEC companyfacts JSON |
| Research & Development | 8,198 | 8,829 | 8,146 | 8,504 | 8,915 | `ResearchAndDevelopmentExpense` | reported (Q1–Q3); derived (Q4 = FY − YTD_Q3) | OpenBB `obb.equity.compare.company_facts` (sec) + SEC companyfacts JSON |
| Sales & Marketing | 6,212 | 7,285 | 5,717 | 6,584 | 6,814 | `SellingAndMarketingExpense` | reported (Q1–Q3); derived (Q4 = FY − YTD_Q3) | SEC companyfacts JSON (CIK 0000789019) |
| General & Administrative | 1,737 | 1,990 | 1,806 | 1,932 | 1,931 | `GeneralAndAdministrativeExpense` | reported (Q1–Q3); derived (Q4 = FY − YTD_Q3) | OpenBB `obb.equity.compare.company_facts` (sec) + SEC companyfacts JSON |
| Operating Income | 32,000 | 34,323 | 37,961 | 38,275 | 38,398 | `OperatingIncomeLoss` | reported (Q1–Q3); derived (Q4 = FY − YTD_Q3) | OpenBB `obb.equity.compare.company_facts` (sec) + SEC companyfacts JSON |
| Other Income / (Expense), Net | -1,013 | -1,864 | -4,923 | 9,541 | -491 | `OtherNonoperatingIncomeExpense` | reported (Q1–Q3); derived (Q4 = FY − YTD_Q3) | SEC companyfacts JSON (CIK 0000789019) |
| Pretax Income | 31,377 | 32,616 | 34,301 | 48,246 | 39,340 | `IncomeLossFromContinuingOperationsBeforeIncomeTaxesExtraordinaryItemsNoncontrollingInterest` | reported (Q1–Q3); derived (Q4 = FY − YTD_Q3) | OpenBB `obb.equity.compare.company_facts` (sec) + SEC companyfacts JSON |
| Income Tax Expense | 5,553 | 5,383 | 6,554 | 9,788 | 7,562 | `IncomeTaxExpenseBenefit` | reported (Q1–Q3); derived (Q4 = FY − YTD_Q3) | OpenBB `obb.equity.compare.company_facts` (sec) + SEC companyfacts JSON |
| Net Income | 25,824 | 27,233 | 27,747 | 38,458 | 31,778 | `NetIncomeLoss` | reported (Q1–Q3); derived (Q4 = FY − YTD_Q3) | OpenBB `obb.equity.compare.company_facts` (sec) + SEC companyfacts JSON |
| Diluted EPS | 3.46 | 3.65 | 3.72 | 5.16 | 4.27 | `EarningsPerShareDiluted` | reported (Q1–Q3); derived (Q4 = FY − YTD_Q3) | OpenBB `obb.equity.compare.company_facts` (sec) + SEC companyfacts JSON |

> `*` Q4 column is derived (`FY annual − YTD_Q3 from latest 10-Q`); MSFT does not file a Q4 10-Q. Foots to the annual within ±$1M rounding.

### 3.3 Balance Sheet — Annual (USD millions)

| Line Item | FY2021 | FY2022 | FY2023 | FY2024 | FY2025 | XBRL Tag / Formula | Mapping | Source |
|---|---|---|---|---|---|---|---|---|
| Cash & Equivalents | 14,224 | 13,931 | 34,704 | 18,315 | 30,242 | `CashAndCashEquivalentsAtCarryingValue` | reported | OpenBB `obb.equity.compare.company_facts` (sec) + SEC companyfacts JSON |
| Short-term Investments | 116,110 | 90,826 | 76,558 | 57,228 | 64,323 | `ShortTermInvestments` | reported | OpenBB `obb.equity.compare.company_facts` (sec) + SEC companyfacts JSON |
| Accounts Receivable, Net | 38,043 | 44,261 | 48,688 | 56,924 | 69,905 | `AccountsReceivableNetCurrent` | reported | OpenBB `obb.equity.compare.company_facts` (sec) + SEC companyfacts JSON |
| Inventory, Net | 2,636 | 3,742 | 2,500 | 1,246 | 938 | `InventoryNet` | reported | OpenBB `obb.equity.compare.company_facts` (sec) + SEC companyfacts JSON |
| Total Current Assets | 184,406 | 169,684 | 184,257 | 159,734 | 191,131 | `AssetsCurrent` | reported | OpenBB `obb.equity.compare.company_facts` (sec) + SEC companyfacts JSON |
| PP&E, Net | 59,715 | 74,398 | 95,641 | 135,591 | 204,966 | `PropertyPlantAndEquipmentNet` | reported | OpenBB `obb.equity.compare.company_facts` (sec) + SEC companyfacts JSON |
| Operating Lease ROU Asset | 11,088 | 13,148 | 14,346 | 18,961 | 24,823 | `OperatingLeaseRightOfUseAsset` | reported | SEC companyfacts JSON (CIK 0000789019) |
| Goodwill | 49,711 | 67,524 | 67,886 | 119,220 | 119,509 | `Goodwill` | reported | OpenBB `obb.equity.compare.company_facts` (sec) + SEC companyfacts JSON |
| Intangible Assets, Net | 7,800 | 11,298 | 9,366 | 27,597 | 22,604 | `FiniteLivedIntangibleAssetsNet` | reported | OpenBB `obb.equity.compare.company_facts` (sec) + SEC companyfacts JSON |
| **Total Assets** | 333,779 | 364,840 | 411,976 | 512,163 | 619,003 | `Assets` | reported | OpenBB `obb.equity.compare.company_facts` (sec) + SEC companyfacts JSON |
| Accounts Payable | 15,163 | 19,000 | 18,095 | 21,996 | 27,724 | `AccountsPayableCurrent` | reported | OpenBB `obb.equity.compare.company_facts` (sec) + SEC companyfacts JSON |
| Short-term Borrowings | 8,072 | 2,749 | 5,247 | 2,249 | 2,999 | `LongTermDebtCurrent` | reported | OpenBB `obb.equity.compare.company_facts` (sec) + SEC companyfacts JSON |
| Total Current Liabilities | 88,657 | 95,082 | 104,149 | 125,286 | 141,218 | `LiabilitiesCurrent` | reported | OpenBB `obb.equity.compare.company_facts` (sec) + SEC companyfacts JSON |
| Long-term Debt | 50,074 | 47,032 | 41,990 | 42,688 | 40,152 | `LongTermDebtNoncurrent` | reported | OpenBB `obb.equity.compare.company_facts` (sec) + SEC companyfacts JSON |
| Operating Lease Liability, NC | 9,629 | 11,489 | 12,728 | 15,497 | 17,437 | `OperatingLeaseLiabilityNoncurrent` | reported | SEC companyfacts JSON (CIK 0000789019) |
| **Total Liabilities** | 191,791 | 198,298 | 205,753 | 243,686 | 275,524 | `Liabilities` | reported | OpenBB `obb.equity.compare.company_facts` (sec) + SEC companyfacts JSON |
| Common Stock & APIC | 83,111 | 86,939 | 93,718 | 100,923 | 109,095 | `CommonStocksIncludingAdditionalPaidInCapital` | reported | OpenBB `obb.equity.compare.company_facts` (sec) + SEC companyfacts JSON |
| Retained Earnings | 57,055 | 84,281 | 118,848 | 173,144 | 237,731 | `RetainedEarningsAccumulatedDeficit` | reported | OpenBB `obb.equity.compare.company_facts` (sec) + SEC companyfacts JSON |
| Accumulated OCI | 1,822 | -4,678 | -6,343 | -5,590 | -3,347 | `AccumulatedOtherComprehensiveIncomeLossNetOfTax` | reported | OpenBB `obb.equity.compare.company_facts` (sec) + SEC companyfacts JSON |
| **Total Stockholders' Equity** | 141,988 | 166,542 | 206,223 | 268,477 | 343,479 | `StockholdersEquity` | reported | OpenBB `obb.equity.compare.company_facts` (sec) + SEC companyfacts JSON |

### 3.4 Balance Sheet — Last 5 Quarter-End Snapshots (Q4 = fiscal year-end from 10-K)

| Line Item | Q3 FY2025<br>(2025-03-31) | Q4 FY2025<br>(2025-06-30) | Q1 FY2026<br>(2025-09-30) | Q2 FY2026<br>(2025-12-31) | Q3 FY2026<br>(2026-03-31) | XBRL Tag / Formula | Mapping | Source |
|---|---|---|---|---|---|---|---|---|
| Cash & Equivalents | 28,828 | 30,242 | 28,849 | 24,296 | 32,105 | `CashAndCashEquivalentsAtCarryingValue` | reported (instant) | OpenBB `obb.equity.compare.company_facts` (sec) + SEC companyfacts JSON |
| Short-term Investments | 50,790 | 64,323 | 73,163 | 65,166 | 46,167 | `ShortTermInvestments` | reported (instant) | OpenBB `obb.equity.compare.company_facts` (sec) + SEC companyfacts JSON |
| Accounts Receivable, Net | 51,700 | 69,905 | 52,894 | 56,535 | 60,041 | `AccountsReceivableNetCurrent` | reported (instant) | OpenBB `obb.equity.compare.company_facts` (sec) + SEC companyfacts JSON |
| Inventory, Net | 848 | 938 | 1,130 | 1,059 | 1,219 | `InventoryNet` | reported (instant) | OpenBB `obb.equity.compare.company_facts` (sec) + SEC companyfacts JSON |
| Total Current Assets | 156,644 | 191,131 | 189,066 | 180,190 | 175,329 | `AssetsCurrent` | reported (instant) | OpenBB `obb.equity.compare.company_facts` (sec) + SEC companyfacts JSON |
| PP&E, Net | 183,939 | 204,966 | 230,861 | 261,126 | 283,228 | `PropertyPlantAndEquipmentNet` | reported (instant) | OpenBB `obb.equity.compare.company_facts` (sec) + SEC companyfacts JSON |
| Operating Lease ROU Asset | 24,475 | 24,823 | 24,791 | 25,103 | 24,403 | `OperatingLeaseRightOfUseAsset` | reported (instant) | SEC companyfacts JSON (CIK 0000789019) |
| Goodwill | 119,329 | 119,509 | 119,497 | 119,622 | 119,661 | `Goodwill` | reported (instant) | OpenBB `obb.equity.compare.company_facts` (sec) + SEC companyfacts JSON |
| Intangible Assets, Net | 23,968 | 22,604 | 21,236 | 20,289 | 19,325 | `FiniteLivedIntangibleAssetsNet` | reported (instant) | OpenBB `obb.equity.compare.company_facts` (sec) + SEC companyfacts JSON |
| **Total Assets** | 562,624 | 619,003 | 636,351 | 665,302 | 694,228 | `Assets` | reported (instant) | OpenBB `obb.equity.compare.company_facts` (sec) + SEC companyfacts JSON |
| Accounts Payable | 26,250 | 27,724 | 32,580 | 37,328 | 37,513 | `AccountsPayableCurrent` | reported (instant) | OpenBB `obb.equity.compare.company_facts` (sec) + SEC companyfacts JSON |
| Short-term Borrowings | 2,999 | 2,999 | 7,832 | 4,837 | 8,839 | `LongTermDebtCurrent` | reported (instant) | OpenBB `obb.equity.compare.company_facts` (sec) + SEC companyfacts JSON |
| Total Current Liabilities | 114,206 | 141,218 | 134,996 | 130,005 | 136,661 | `LiabilitiesCurrent` | reported (instant) | OpenBB `obb.equity.compare.company_facts` (sec) + SEC companyfacts JSON |
| Long-term Debt | 39,882 | 40,152 | 35,376 | 35,425 | 31,423 | `LongTermDebtNoncurrent` | reported (instant) | OpenBB `obb.equity.compare.company_facts` (sec) + SEC companyfacts JSON |
| Operating Lease Liability, NC | 17,686 | 17,437 | 17,348 | 17,345 | 16,703 | `OperatingLeaseLiabilityNoncurrent` | reported (instant) | SEC companyfacts JSON (CIK 0000789019) |
| **Total Liabilities** | 240,733 | 275,524 | 273,275 | 274,427 | 279,861 | `Liabilities` | reported (instant) | OpenBB `obb.equity.compare.company_facts` (sec) + SEC companyfacts JSON |
| Common Stock & APIC | 106,965 | 109,095 | 110,964 | 112,788 | 115,069 | `CommonStocksIncludingAdditionalPaidInCapital` | reported (instant) | OpenBB `obb.equity.compare.company_facts` (sec) + SEC companyfacts JSON |
| Retained Earnings | 219,759 | 237,731 | 254,873 | 280,789 | 302,526 | `RetainedEarningsAccumulatedDeficit` | reported (instant) | OpenBB `obb.equity.compare.company_facts` (sec) + SEC companyfacts JSON |
| Accumulated OCI | -4,833 | -3,347 | -2,761 | -2,702 | -3,228 | `AccumulatedOtherComprehensiveIncomeLossNetOfTax` | reported (instant) | OpenBB `obb.equity.compare.company_facts` (sec) + SEC companyfacts JSON |
| **Total Stockholders' Equity** | 321,891 | 343,479 | 363,076 | 390,875 | 414,367 | `StockholdersEquity` | reported (instant) | OpenBB `obb.equity.compare.company_facts` (sec) + SEC companyfacts JSON |

> Q4 column = fiscal year-end snapshot (sourced from 10-K) — not derived. Ties exactly to §3.3 FY column.

### 3.5 Cash Flow Statement — Annual (USD millions)

| Line Item | FY2021 | FY2022 | FY2023 | FY2024 | FY2025 | XBRL Tag / Formula | Mapping | Source |
|---|---|---|---|---|---|---|---|---|
| Net Income | 61,271 | 72,738 | 72,361 | 88,136 | 101,832 | `NetIncomeLoss` | reported | OpenBB `obb.equity.compare.company_facts` (sec) + SEC companyfacts JSON |
| Depreciation, Amortization & Other | 11,686 | 14,460 | 13,861 | 22,287 | 34,153 | `DepreciationAmortizationAndOther` (CF reconciling line; company XBRL extension) | reported | SEC 10-K cash flow statement (R6) — CIK 0000789019 |
| Stock-Based Compensation | 6,118 | 7,502 | 9,611 | 10,734 | 11,974 | `ShareBasedCompensation` | reported | OpenBB `obb.equity.compare.company_facts` (sec) + SEC companyfacts JSON |
| **Cash from Operations** | 76,740 | 89,035 | 87,582 | 118,548 | 136,162 | `NetCashProvidedByUsedInOperatingActivities` | reported | OpenBB `obb.equity.compare.company_facts` (sec) + SEC companyfacts JSON |
| Capex | 20,622 | 23,886 | 28,107 | 44,477 | 64,551 | `PaymentsToAcquirePropertyPlantAndEquipment` | reported | OpenBB `obb.equity.compare.company_facts` (sec) + SEC companyfacts JSON |
| Free Cash Flow | 56,118 | 65,149 | 59,475 | 74,071 | 71,611 | `CFO − |Capex|` | derived | derived |
| Cash from Investing | -27,577 | -30,311 | -22,680 | -96,970 | -72,599 | `NetCashProvidedByUsedInInvestingActivities` | reported | OpenBB `obb.equity.compare.company_facts` (sec) + SEC companyfacts JSON |
| Share Repurchases | 27,385 | 32,696 | 22,245 | 17,254 | 18,420 | `PaymentsForRepurchaseOfCommonStock` | reported | OpenBB `obb.equity.compare.company_facts` (sec) + SEC companyfacts JSON |
| Dividends Paid | 16,521 | 18,135 | 19,800 | 21,771 | 24,082 | `PaymentsOfDividendsCommonStock` | reported | SEC companyfacts JSON (CIK 0000789019) |
| Proceeds from Stock Issuance | 1,693 | 1,841 | 1,866 | 2,002 | 2,056 | `ProceedsFromIssuanceOfCommonStock` | reported | OpenBB `obb.equity.compare.company_facts` (sec) + SEC companyfacts JSON |
| Cash from Financing | -48,486 | -58,876 | -43,935 | -37,757 | -51,699 | `NetCashProvidedByUsedInFinancingActivities` | reported | OpenBB `obb.equity.compare.company_facts` (sec) + SEC companyfacts JSON |

> `Depreciation, Amortization & Other` is Microsoft's single combined cash-flow reconciling line (company XBRL extension — not exposed by SEC companyfacts us-gaap whitelist; sourced from the 10-K cash flow statement). FY2025 components per notes (rounded): depreciation ~$22.0B, intangible amortization ~$6.0B, finance-lease ROU amortization $3.4B, other ~$2.8B. The standalone `Depreciation` ($22.0B) and `AmortizationOfIntangibleAssets` ($6.0B) us-gaap tags are rounded note disclosures, not the cash-flow line, and do not foot to it.

### 3.6 Cash Flow Statement — Last 5 Standalone Quarters (3M periods; Q4 derived)

| Line Item | Q3 FY2025<br>(2025-03-31) | Q4 FY2025*<br>(2025-06-30) | Q1 FY2026<br>(2025-09-30) | Q2 FY2026<br>(2025-12-31) | Q3 FY2026<br>(2026-03-31) | XBRL Tag / Formula | Mapping | Source |
|---|---|---|---|---|---|---|---|---|
| Net Income | 25,824 | 27,233 | 27,747 | 38,458 | 31,778 | `NetIncomeLoss` | reported (Q1–Q3); derived (Q4 = FY − YTD_Q3) | OpenBB `obb.equity.compare.company_facts` (sec) + SEC companyfacts JSON |
| Depreciation, Amortization & Other | 8,740 | 11,203* | 13,061 | 9,198 | 10,167 | `DepreciationAmortizationAndOther` (CF reconciling line; company XBRL extension) | reported (3M read from 10-Q); derived (Q4 = FY − YTD_Q3) | SEC 10-Q / 10-K cash flow statements (R6) — CIK 0000789019 |
| Stock-Based Compensation | 2,980 | 3,073 | 2,983 | 3,219 | 3,081 | `ShareBasedCompensation` | reported (Q1–Q3); derived (Q4 = FY − YTD_Q3) | OpenBB `obb.equity.compare.company_facts` (sec) + SEC companyfacts JSON |
| **Cash from Operations** | 37,044 | 42,647 | 45,057 | 35,758 | 46,679 | `NetCashProvidedByUsedInOperatingActivities` | reported (Q1–Q3); derived (Q4 = FY − YTD_Q3) | OpenBB `obb.equity.compare.company_facts` (sec) + SEC companyfacts JSON |
| Capex | 16,745 | 17,079 | 19,394 | 29,876 | 30,876 | `PaymentsToAcquirePropertyPlantAndEquipment` | reported (Q1–Q3); derived (Q4 = FY − YTD_Q3) | OpenBB `obb.equity.compare.company_facts` (sec) + SEC companyfacts JSON |
| Free Cash Flow | 20,299 | 25,568 | 25,663 | 5,882 | 15,803 | `CFO − |Capex|` | derived | derived |
| Cash from Investing | -12,714 | -30,572 | -34,559 | -22,705 | -27,405 | `NetCashProvidedByUsedInInvestingActivities` | reported (Q1–Q3); derived (Q4 = FY − YTD_Q3) | OpenBB `obb.equity.compare.company_facts` (sec) + SEC companyfacts JSON |
| Share Repurchases | 4,781 | 4,546 | 5,650 | 7,415 | 4,627 | `PaymentsForRepurchaseOfCommonStock` | reported (Q1–Q3); derived (Q4 = FY − YTD_Q3) | OpenBB `obb.equity.compare.company_facts` (sec) + SEC companyfacts JSON |
| Dividends Paid | 6,169 | 6,169 | 6,169 | 6,762 | 6,756 | `PaymentsOfDividendsCommonStock` | reported (Q1–Q3); derived (Q4 = FY − YTD_Q3) | SEC companyfacts JSON (CIK 0000789019) |
| Proceeds from Stock Issuance | 546 | 548 | 689 | 259 | 541 | `ProceedsFromIssuanceOfCommonStock` | reported (Q1–Q3); derived (Q4 = FY − YTD_Q3) | OpenBB `obb.equity.compare.company_facts` (sec) + SEC companyfacts JSON |
| Cash from Financing | -13,036 | -10,844 | -11,799 | -17,617 | -11,351 | `NetCashProvidedByUsedInFinancingActivities` | reported (Q1–Q3); derived (Q4 = FY − YTD_Q3) | OpenBB `obb.equity.compare.company_facts` (sec) + SEC companyfacts JSON |

> 3M standalone basis. Non-Q4 cells derived from successive YTD values (`Q1 = YTD_Q1; Q2 = YTD_Q2 − YTD_Q1; Q3 = YTD_Q3 − YTD_Q2`). Q4 = FY − YTD_Q3. The 4 cells for each FY sum to the §3.5 FY column within ±$1M.

### 3.7 Statement of Stockholders' Equity — Annual (USD millions)

| Line Item | FY2021 | FY2022 | FY2023 | FY2024 | FY2025 | XBRL Tag / Formula | Mapping | Source |
|---|---|---|---|---|---|---|---|---|
| Beginning Equity | 118,304 | 141,988 | 166,542 | 206,223 | 268,477 | `StockholdersEquity` (prior-FY close) | reported | SEC 10-K Stockholders' Equity statement (R7) |
| Cumulative Effect of Accounting Change | -22 | — | — | — | — | equity statement opening adjustment | reported | SEC 10-K Stockholders' Equity statement (R7) |
| Net Income | 61,271 | 72,738 | 72,361 | 88,136 | 101,832 | `NetIncomeLoss` | reported | SEC 10-K Stockholders' Equity statement (R7) |
| Other Comprehensive Income (Loss) | -1,374 | -6,500 | -1,665 | 753 | 2,243 | `OtherComprehensiveIncomeLossNetOfTax` | reported | SEC 10-K Stockholders' Equity statement (R7) |
| Common Stock Issued | 1,963 | 1,841 | 1,866 | 2,002 | 2,056 | equity statement "Common stock issued" | reported | SEC 10-K Stockholders' Equity statement (R7) |
| Stock-Based Compensation | 6,118 | 7,502 | 9,611 | 10,734 | 11,974 | `ShareBasedCompensation` | reported | SEC 10-K Stockholders' Equity statement (R7) |
| Common Stock Repurchased (APIC + RE) | -27,418 | -32,648 | -22,264 | -17,259 | -18,424 | equity statement repurchase (PIC + RE components) | reported | SEC 10-K Stockholders' Equity statement (R7) |
| Common Stock Cash Dividends (declared) | -16,871 | -18,552 | -20,226 | -22,293 | -24,677 | equity statement dividends (RE charge) | reported | SEC 10-K Stockholders' Equity statement (R7) |
| Other, Net | 17 | 173 | -2 | 181 | -2 | equity statement "Other, net" | reported | SEC 10-K Stockholders' Equity statement (R7) |
| **Ending Equity** | 141,988 | 166,542 | 206,223 | 268,477 | 343,479 | `StockholdersEquity` | reported | SEC 10-K Stockholders' Equity statement (R7) |

> Reconciles exactly for all five years: Begin + Cum. effect + NI + OCI + Issued + SBC − Repurchases − Dividends + Other = End. Repurchases are the total charged to equity, which MSFT splits across common stock/APIC and retained earnings; dividends are the **declared** amount charged to retained earnings (differs from cash-flow dividends *paid* — FY2025 declared $24,677M vs paid $24,082M). Cash dividends declared per share: FY2021 $2.24 · FY2022 $2.48 · FY2023 $2.72 · FY2024 $3.00 · FY2025 $3.32.

## Management Discussion And Guidance

> Sources distilled in this section (verbatim at the source links):
> - Latest 10-Q · Q3 FY26 · period ending 2026-03-31 · https://www.sec.gov/Archives/edgar/data/789019/000119312526191507/msft-20260331.htm
> - Prior 10-Q · Q2 FY26 · period ending 2025-12-31 · https://www.sec.gov/Archives/edgar/data/789019/000119312526027207/msft-20251231.htm
> - Q3 FY26 earnings release (8-K Exhibit 99.1) · 2026-04-29 · https://www.sec.gov/Archives/edgar/data/789019/000119312526191457/msft-ex99_1.htm
> - **MSFT IR Q4 outlook** · 2026-04-29 · https://aka.ms/outlookfy26q3
> - **MSFT IR Q&A transcript** · 2026-04-29 · https://aka.ms/transcriptfy26q3
> - MSFT IR slides deck · https://aka.ms/slidesfy26q3

### 4.1 Quarter Headline (Q3 FY26, reported 2026-04-29)

- Revenue **$82.9B (+18% YoY)** · OI **$38.4B (+20%)** · NI **$31.8B (+23%)** · Diluted EPS **$4.27 (+23%)**
- Microsoft Cloud revenue **$54.5B (+29%)**
- 9M FY26: revenue $241.8B (+18%) · OI $114.6B (+22%) · NI $98.0B (+31%) · EPS $13.14 (+32%)
- FX tailwind: +3% revenue / +4% OI (USD weakness)
- OpenAI investment impact on NI: Q3 −$14M (vs Q3 FY25 −$583M / −$0.08 EPS)

### 4.2 Business Line YoY (Q3 FY26 vs Q2 FY26)

| Line | Q3 FY26 | Q2 FY26 | Δ |
|---|---|---|---|
| Azure & other cloud services | +40% | +39% | re-accel |
| M365 Consumer cloud | +33% | +29% | accel |
| Commercial RPO ($627B) | +99% | +110% | slight decel, still parabolic |
| Dynamics 365 | +22% | +19% | accel |
| M365 Commercial cloud | +19% | +17% | accel |
| Search ads ex-TAC | +12% | +10% | accel |
| LinkedIn | +12% | +11% | flat |
| Xbox content & svc | −5% | −5% | flat decline |
| Windows OEM & Devices | −2% | +1% | **turned negative** |

### 4.3 Margin & Cost Story

- **Microsoft Cloud GM% compressed to 66%** — management explicitly attributes this to AI infrastructure + AI product-usage investment, partly offset by Azure / M365 efficiency gains
- Opex +9% (continued R&D + AI talent + data investment); **total company headcount down YoY**
- 9M FY26 P&E additions +$32.7B YoY — the capex cycle is consuming FCF (9M FCF −3.3% YoY)
- Effective tax rate: Q3 19% (prior year 18%) / 9M 20% (prior year 18%) — US/foreign earnings mix shift (**no longer** attributed to the OpenAI recapitalization)

### 4.4 Capital & Liquidity (as of 2026-03-31)

- Cash + ST inv **$78.3B** (FYE 2025: $94.6B → down a further $11.2B QoQ vs $89.5B at end-Q2)
- Equity & other investments **$33.7B** (FYE: $15.4B → doubled, mainly the OpenAI restructuring stake remeasurement)
- 9M FY26 CFO **$127.5B** (+$34.0B YoY): higher customer collections + lower tax payments
- 9M financing −$40.8B: buyback +$3.8B, dividends +$1.8B, debt repayment −$6B
- **Buyback authorization $44.0B remaining of $60B**; 27M shares repurchased for $13.3B over 9M
- 9M dividends declared **$20.3B**
- **Unearned revenue $53.7B** (Q4 FY26 contracted release $24.8B — a contracted minimum-revenue signal)

### 4.5 Tone Shift vs Prior 10-Q (Q2 FY26 → Q3 FY26)

Substantive changes in management's wording / narrative (the numeric comparison is in §4.2; this is qualitative only):

- **Re-acceleration signals**: Azure 39→40%, M365 Consumer cloud 29→33%, Search ads ex-TAC 10→12%
- **Deceleration / turning negative**:
  - Windows OEM & Devices +1% → **−2%** (weakening PC-cycle signal)
  - Commercial RPO +110% → +99% (first drop below triple digits, though absolute value still $627B)
- **First explicit disclosure**: Microsoft Cloud GM% proactively called out at 66% in Q3 (not broken out in Q2) — margin pre-staging
- **Evolution of the OpenAI narrative**:
  - Q2 wording: "October 2025 new definitive agreement" (one-time event)
  - Q3 wording: "October 2025 and April 2026, we extended this partnership" (**two extensions — from event to ongoing**)
  - Revenue-share description: Q2 "reciprocal arrangements" → Q3 "will continue to receive revenue-sharing payments"
- **Tax-rate attribution shift**:
  - Q2: 20% ETR → attributed to "OpenAI Recapitalization dilution gain" (one-time)
  - Q3: 19% / 20% → attributed to "US/foreign earnings mix" (**structural**)
- **Balance-sheet trend**: cash $89.5B → $78.3B (capex keeps consuming it); equity investments $21.2B → $33.7B (OpenAI stake remeasurement)
- **Unchanged language**: IRS NOPAs $28.9B, forward-looking boilerplate, segment definitions, accounting policies

### 4.6 Risks & Management Topics

- **OpenAI partnership extended twice** (2025-10 + 2026-04); MSFT retains rights to use OpenAI IP (models + infrastructure), and the revenue-share arrangement continues
- **IRS NOPAs** (FY2004–2013 transfer-pricing case): IRS seeks **$28.9B + penalties/interest** in additional tax; MSFT disagrees and plans to appeal; status unchanged
- Management states explicitly that AI-infrastructure investment "will continue to increase operating costs and may decrease operating margins"
- Reiterated risks: geopolitics / international trade policy / tariffs / export controls → supply-chain and demand volatility

### 4.7 Forward Guidance — Q4 FY26 + CY2026 + FY27

Source: MSFT IR official Q4 outlook slides (https://aka.ms/outlookfy26q3), released alongside CFO Amy Hood's prepared remarks on the 2026-04-29 earnings call. The 8-K Exhibit 99.1 explicitly defers to the webcast and contains no specific numbers itself.

#### Q4 FY26 (quarter ending 2026-06-30)

| Item | Guidance |
|---|---|
| **Total Company revenue** | **$86.7 – $87.8B** |
| Productivity & Business Processes revenue | $37.0 – $37.3B |
| Intelligent Cloud revenue | $37.95 – $38.25B |
| More Personal Computing revenue | $11.75 – $12.25B |
| **Azure & other cloud services growth (CC)** | **+39% – +40%** |
| M365 Commercial cloud growth (CC) | +13% – +14% (or +15% – +16% adjusted for prior-year in-period revenue recognition) |
| M365 Consumer cloud growth | low-twenties |
| M365 Commercial products growth | mid-single digits |
| LinkedIn growth | ~+10% |
| Dynamics 365 growth | low-double digits |
| Search ads ex-TAC growth | high-single digits |
| Windows OEM & Devices growth | decline **mid- to high-teens** |
| Xbox content & services growth | decline **low-teens** |
| Server products growth | decline mid-single digits |
| Commercial bookings | "healthy growth on growing expiry base, adjusted for prior-year OpenAI contracts" |
| **Microsoft Cloud GM%** | **~64%** (vs Q3 actual 66%, a further ~2pp compression) |
| COGS | $29.4 – $29.6B |
| Operating expenses | $19.3 – $19.4B |
| Other income/(expense) | ~$(100)M (ex-OpenAI impact) |
| Effective tax rate | ~19% (ex-OpenAI impact) |
| **Capex (Q4 stand-alone)** | **>$40B** |
| FX impact: revenue | +<1pt overall (~+1pt P&BP & MPC, no meaningful IC) |
| FX impact: COGS / Opex | COGS +~1pt / Opex 0 |

#### Calendar Year 2026

- **Capex ~$190B**, of which ~$25B comes from higher component pricing
- Azure growth: "modest acceleration" in 2H CY26 vs 1H

#### Fiscal Year 2027

- Total revenue: grow **double-digits**
- Operating expenses: grow **mid- to high-single digits**
- Operating income: grow **double-digits**

> Capex cadence signal: Q3 FY26 P&E additions ~$21.4B (implied by 9M $64.5B) → the Q4 guide of ">$40B" implies nearly 2x QoQ; the full-year CY26 $190B implies heavy front-loading in 2H. AI-infrastructure investment is still ramping, so FCF pressure will persist.

## Price And Valuation Helpers

| Metric | Value | Source / Formula |
|---|---|---|
| Last close | $419.67 | `obb.equity.price.quote` cboe; last_timestamp 2026-05-15T15:59:59.000 |
| 52-week range | $356.28 – $555.45 | quote payload |
| Diluted shares (FY2025 weighted) | 7,465 M | `WeightedAverageNumberOfDilutedSharesOutstanding` |
| Approx. market cap | $3,133B | last_price × FY-weighted diluted shares |
| LFY P/E | 30.8x | last_price / FY2025 diluted EPS (13.64) |
| Trailing (TTM) P/E | 25.0x | last_price / (sum last 4 standalone-quarter NI / FY-weighted diluted shares) |
| LFY EV/EBIT | 24.0x | (Mkt cap + ST&LT debt − cash − ST inv) / Operating Income |
| LFY Price / FCF | 43.7x | Mkt cap / FCF |
| Implied 30-day vol (cboe iv30) | 29.3% | quote payload |

> TTM is now a clean trailing-4-quarter sum (`Q4 FY2025 + Q1 FY2026 + Q2 FY2026 + Q3 FY2026`) thanks to the derived Q4 column. No more 9-month roll-forward approximation.

## Optional Ownership, Short, And Options Data

### 6.1 Insider Trading (Form 4) — Recent

| Filing Date | Reporting Person | Transaction Date | Type | Shares | Price |
|---|---|---|---|---|---|
| 2026-04-15 | Coleman Amy | 2026-04-15 | Disposition | 1363.733 | 393.11 |
| 2026-03-16 | Coleman Amy | 2026-03-16 | Disposition | 31.095 | 395.55 |
| 2026-03-13 | Rainey John D | 2026-03-12 | Acquisition | 0.328 | 0.0 |
| 2026-03-13 | MacGregor Catherine | 2026-03-12 | Acquisition | 4.357 | 0.0 |
| 2026-03-13 | Walmsley Emma N | 2026-03-12 | Acquisition | 2.507 | 0.0 |
| 2026-03-13 | PETERSON SANDRA E | 2026-03-12 | Acquisition | 58.507 | 0.0 |
| 2026-03-13 | List Teri | 2026-03-12 | Acquisition | 52.01 | 0.0 |
| 2026-03-13 | PRITZKER PENNY S | 2026-03-12 | Acquisition | 31.743 | 0.0 |
| 2026-03-13 | Johnston Hugh F | 2026-03-12 | Acquisition | 4.253 | 0.0 |
| 2026-03-13 | Hoffman Reid | 2026-03-12 | Acquisition | 37.726 | 0.0 |
| 2026-03-09 | Hogan Kathleen T | 2026-03-06 | Disposition | 12320.87 | 409.52 |
| 2026-03-03 | Numoto Takeshi | 2026-03-02 | Disposition | 1351.169 | 392.74 |
| 2026-03-03 | Jolla Alice L. | 2026-03-02 | Disposition | 424.204 | 392.74 |
| 2026-03-03 | SMITH BRADFORD L | 2026-03-02 | Disposition | 3589.532 | 392.74 |
| 2026-03-03 | Hood Amy | 2026-03-02 | Disposition | 4789.714 | 392.74 |

### 6.2 FINRA Short Interest (latest 12 of 113 unique settlement dates; range 2021-07-15 … 2026-04-15)

| Settlement Date | Current Short Position (sh) | Δ vs Prior | Δ % | Avg Daily Volume (sh) | Days to Cover |
|---|---|---|---|---|---|
| 2025-10-31 | 52,549,516 | 204,636 | +0.39% | 22,626,543 | 2.32 |
| 2025-11-14 | 48,553,497 | -3,996,019 | -7.60% | 23,988,414 | 2.02 |
| 2025-11-28 | 61,948,927 | 13,395,438 | +27.59% | 25,987,206 | 2.38 |
| 2025-12-15 | 66,675,893 | 4,726,966 | +7.63% | 23,823,417 | 2.80 |
| 2025-12-31 | 52,944,379 | -13,731,514 | -20.59% | 20,803,939 | 2.54 |
| 2026-01-15 | 54,651,789 | 1,707,410 | +3.22% | 23,669,106 | 2.31 |
| 2026-01-30 | 58,407,538 | 3,755,749 | +6.87% | 43,544,863 | 1.34 |
| 2026-02-13 | 56,124,540 | -2,282,998 | -3.91% | 46,894,552 | 1.20 |
| 2026-02-27 | 74,347,979 | 18,223,439 | +32.47% | 32,148,149 | 2.31 |
| 2026-03-13 | 79,835,909 | 5,487,930 | +7.38% | 31,867,264 | 2.51 |
| 2026-03-31 | 80,991,357 | 1,155,448 | +1.45% | 35,067,520 | 2.31 |
| 2026-04-15 | 83,407,242 | 2,415,885 | +2.98% | 29,802,350 | 2.80 |

### 6.3 Form 13F

> MSFT is not a 13F filer (not an institutional investment manager). MSFT holders must be reverse-aggregated from holders' 13F filings.

### 6.4 SEC Fails-to-Deliver (FTD)

_Endpoint: `obb.equity.shorts.fails_to_deliver` (sec). 163 daily observations from 2025-05-01 to 2026-04-28._

| Window | Days | Total FTD shares | Avg FTD/day |
|---|---|---|---|
| Last 30 obs | 30 | 1,031,615 | 34,387 |
| Last 90 obs | 90 | 1,334,714 | 14,830 |
| Full dataset | 163 | 3,068,963 | 18,828 |

## Analyst Commentary

- **Top line scale & growth**: FY2025 revenue $281.7B grew 14.9% YoY. Five-year stack from FY2021 ($168.1B) implies 13.8% CAGR.
- **Quarterly momentum (3M sequential)**: Revenue stepped $70.1B → $76.4B → $77.7B → $81.3B → $82.9B across the last 5 standalone quarters.
- **Operating leverage**: FY2025 operating margin 45.6% on operating income $128.5B; YoY change 17.4%. Gross margin 68.8%.
- **Cash conversion**: FY2025 CFO $136.2B vs. net income $101.8B (CFO/NI = 1.34x). Capex $64.6B yields FCF $71.6B; FCF margin 25.4%.
- **Capital return**: FY2025 buybacks $18.4B + dividends $24.1B = $42.5B.
- **Balance sheet**: Total assets $619B; equity $343B (book leverage 1.80x). Cash $30.2B + ST inv $64.3B vs. LT debt $40.2B → net-cash structurally.
- **Valuation**: At $419.67, LFY P/E 30.8x, TTM P/E 25.0x, LFY P/FCF 43.7x. cboe iv30 29.3%.

Caveat: commentary is descriptive of disclosed financials only; not an investment recommendation.

## Notes — Footnote Topic Index

| Note Id | Topic | Key Disclosure (FY2025) | Status | Source |
|---|---|---|---|---|
| N1 | Revenue Recognition | Total revenue $281,724M, disaggregated by significant product/service offering — largest category Server products & cloud services $98,435M. Remaining performance obligation (RPO): ~40% expected to be recognized within 12 months. Unearned revenue $53.7B at quarter-end. | extracted | 10-K — Accounting Policies / Segment & Geographic (R11, R108) |
| N2 | Segment Disclosure | Three reportable segments (revenue / operating income): Productivity & Business Processes $120,810M / $69,773M; Intelligent Cloud $106,265M / $44,589M; More Personal Computing $54,649M / $14,166M. | extracted | 10-K — Segment Information and Geographic Data (R28, R105) |
| N3 | Debt & Liquidity | Long-term debt total face value $49,206M; carrying value $43,151M (incl. $4,864M debt-exchange premium, $(1,155)M unamortized discount & issuance costs). Cash & equivalents $30,242M + short-term investments $64,323M. | extracted | 10-K — Debt (R20, R72) |
| N4 | Leases & Commitments | Operating lease cost $5,524M; total finance lease cost $4,825M (ROU amortization $3,408M + interest $1,417M). Operating lease ROU asset $24,823M; non-current operating lease liability $17,437M. | extracted | 10-K — Leases (R23, R88) |
| N5 | Share-Based Compensation | SBC expense $11,974M; related income-tax benefit $2,027M. Unrecognized compensation cost $21.6B, expected to be recognized over a ~3-year weighted-average period. 98M shares authorized for future grant. | extracted | 10-K — Employee Stock and Savings Plans (R27, R99, R100) |
| N6 | Buybacks & Dividends | FY2025 repurchases $18,424M charged to equity (under the 2021 $60B program + 2024 program). Dividends declared $24,677M = $3.32/share ($0.83/quarter). | extracted | 10-K — Stockholders' Equity (R25, R95, R96) |
| N7 | Income Taxes | Effective tax rate 17.6% (FY2025) vs 18.2% (FY2024). Reconciliation from 21% federal: foreign earnings (1.5pp), FDII (1.0pp), state +1.5pp, R&D credit (1.1pp), other (1.4pp). IRS NOPAs for FY2004–2013 transfer pricing (~$28.9B plus interest) contested; MSFT plans to appeal. | extracted | 10-K — Income Taxes (R21, R78, R82) |
| N8 | Subsequent Events / Guidance | No material subsequent events beyond ordinary course in the 10-K. Forward guidance (Q4 FY26 + CY2026 + FY27) and commercial RPO $627B are detailed in §4.7 from the Q3 FY26 8-K and IR outlook. | see §4.7 | Latest 8-K earnings release + IR outlook; see §4.7 |

## Data Gaps

- **Q4 standalone**: derived as `FY − YTD_Q3` per `companyfacts.derive_q4_3m`. Reconciled to the dollar for Revenue, NI, Operating Income, CFO, and Capex across FY2025.
- **Stand-alone interest expense / nonoperating components**: pulled from raw SEC companyfacts JSON (outside OpenBB's Literal whitelist). Some sub-items reported only annually.
- **Form 13F**: MSFT is not a 13F filer.
- **Working-capital sub-components on the cash-flow statement**: MSFT discloses individual deltas (AR, deferred revenue) but not under a single aggregated XBRL tag.
- **Note narrative**: full footnote text is not extracted; locations cited in §8 with 10-K URLs.

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
    - endpoint: obb.equity.compare.company_facts
      provider: sec
      attempts: 38
      success: 38
      failed: 0
    - endpoint: obb.equity.fundamental.filings
      provider: sec
      attempts: 2  # initial + deeper limit=100 + form_type=10-Q
      success: 2
    - endpoint: obb.equity.fundamental.management_discussion_analysis
      provider: sec
      attempts: 1
      success: 1
    - endpoint: obb.regulators.sec.htm_file  # used only because OpenBB MD&A endpoint returns latest only
      provider: sec
      attempts: 1
      success: 1  # prior 10-Q HTML for MD&A trend comparison
    - endpoint: obb.equity.price.historical
      provider: cboe
      attempts: 1
      success: 1
    - endpoint: obb.equity.price.quote
      provider: cboe
      attempts: 1
      success: 1
    - endpoint: obb.equity.ownership.insider_trading
      provider: sec
      attempts: 1
      success: 1
    - endpoint: obb.equity.shorts.short_interest
      provider: finra
      attempts: 1
      success: 1
    - endpoint: obb.equity.shorts.fails_to_deliver
      provider: sec
      attempts: 2
      success: 1
SEC:
  companyfacts_json: success   # routed via shared/sec/companyfacts.py (CIK 0000789019)
  rendered_statements_rfiles: success   # 10-K/10-Q R-files via FilingSummary.xml (urllib + org-email UA, light SEC fetch) for CF combined line, SoE rollforward, note figures
WebAccess:
  used: false
  calls: 0
  official_sources_only: true
```
