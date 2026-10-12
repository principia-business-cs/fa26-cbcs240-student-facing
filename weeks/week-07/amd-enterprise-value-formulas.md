# AMD Enterprise Value From The 10-K

## Purpose

We are using AMD's SEC Form 10-K to practice calculating company value. The goal is to connect financial statement data to valuation formulas.

AMD 10-K filing used in class:

<https://ir.amd.com/financial-information/sec-filings/content/0000002488-26-000018/amd-20251227.htm>

## Key Terms

### Market Capitalization

Market capitalization is the value of the company's equity according to the stock market.

```text
Market Capitalization = Current Share Price x Shares Outstanding
```

For AMD:

```text
Market Cap = AMD stock price x AMD shares outstanding
```

The stock price comes from the market. Shares outstanding can be found in the 10-K or from a financial data source.

## Enterprise Value

Enterprise value estimates the value of the whole operating business, not just the equity.

```text
Enterprise Value = Market Capitalization + Total Debt - Cash and Cash Equivalents
```

A more complete version is:

```text
Enterprise Value = Market Capitalization + Total Debt + Preferred Stock + Minority Interest - Cash and Cash Equivalents
```

For this class, we will use the simpler version unless the filing shows major preferred stock or minority interest.

## Step 1: Find Market Capitalization

Use:

```text
Market Cap = Share Price x Shares Outstanding
```

Example layout:

```text
Share price:
Shares outstanding:
Market capitalization:
```

Excel formula:

```excel
=Share_Price_Cell * Shares_Outstanding_Cell
```

## Step 2: Find Total Debt

From the balance sheet, identify debt items such as:

```text
Current debt
Long-term debt
Other borrowings, if listed
```

Formula:

```text
Total Debt = Current Debt + Long-Term Debt
```

Excel formula:

```excel
=Current_Debt_Cell + Long_Term_Debt_Cell
```

## Step 3: Find Cash And Cash Equivalents

From the balance sheet, find:

```text
Cash and cash equivalents
```

Sometimes companies also list short-term investments. Decide whether to include them as excess cash or marketable securities.

Class version:

```text
Cash = Cash and Cash Equivalents
```

Expanded version:

```text
Cash and Investments = Cash and Cash Equivalents + Short-Term Investments
```

## Step 4: Calculate Enterprise Value

Basic formula:

```text
Enterprise Value = Market Cap + Total Debt - Cash
```

Expanded class formula:

```text
Enterprise Value = Market Cap + Total Debt - Cash and Short-Term Investments
```

Excel formula:

```excel
=Market_Cap_Cell + Total_Debt_Cell - Cash_Cell
```

or, if including short-term investments:

```excel
=Market_Cap_Cell + Total_Debt_Cell - Cash_Cell - Short_Term_Investments_Cell
```

## Step 5: Compare Enterprise Value To FCFF

Enterprise value is often compared to free cash flow to the firm.

```text
FCFF = Operating Cash Flow + After-Tax Interest Expense - Capital Expenditures
```

Then you can calculate an implied valuation multiple:

```text
EV / FCFF = Enterprise Value / Free Cash Flow To The Firm
```

Excel formula:

```excel
=Enterprise_Value_Cell / FCFF_Cell
```

## Optional: Simple FCFF Valuation

A simple one-stage FCFF valuation uses:

```text
Enterprise Value = FCFF x (1 + g) / (WACC - g)
```

Where:

```text
FCFF = Free cash flow to the firm
WACC = Discount rate / weighted average cost of capital
g = long-term growth rate
```

Excel formula:

```excel
=FCFF_Cell * (1 + Growth_Rate_Cell) / (WACC_Cell - Growth_Rate_Cell)
```

## Student Work Template

Fill this in:

```text
AMD current share price:
AMD shares outstanding:
Market capitalization:

Current debt:
Long-term debt:
Total debt:

Cash and cash equivalents:
Short-term investments, if included:

Enterprise value using cash only:
Enterprise value using cash plus short-term investments:

FCFF:
EV / FCFF:
```

## Discussion Questions

1. Why is enterprise value different from market capitalization?
2. Why do we add debt when calculating enterprise value?
3. Why do we subtract cash?
4. Should short-term investments be treated like cash? Why or why not?
5. What does EV / FCFF tell us about how expensive the company looks?
6. What assumptions might make AMD's market value very different from a simple FCFF valuation?

## Reminder

Market capitalization values the equity. Enterprise value values the operating business. FCFF belongs to the whole firm, so it should be compared to enterprise value, not just market capitalization.
