# Local Business Valuation Activity

## Purpose

Today we are using the time value of money to estimate the value of three small businesses. Each business has future cash flows, but the cash flows are not equally valuable because they happen in the future and each business has a different risk profile.

Your job is to discount future cash flows back to present value and decide which business you would rather own or invest in.

## Key Idea

A dollar in the future is worth less than a dollar today because:

- You could invest today's dollar and earn a return.
- The future is uncertain.
- Riskier cash flows should usually be discounted at a higher rate.

## Excel Formulas You May Use

### Present value of one future cash flow

If the future cash flow is in cell `B2`, the discount rate is in cell `B1`, and the year is in cell `A2`:

```excel
=B2/(1+$B$1)^A2
```

### Net present value of several future cash flows

If the discount rate is in `B1` and cash flows for Years 1-5 are in `B2:B6`:

```excel
=NPV(B1,B2:B6)
```

Important: Excel's `NPV` assumes the first cash flow happens one period from now. That works for this activity because Year 1 cash flow is one year from now.

### Value after subtracting purchase price

If the present value of future cash flows is in `B8` and the asking price is in `B9`:

```excel
=B8-B9
```

This tells you whether the business appears undervalued or overvalued based on your discount rate.

## Instructions

Your group will evaluate all three businesses.

For each business:

1. Enter the expected cash flows in Excel.
2. Use the suggested discount rate.
3. Calculate the present value of each year's cash flow.
4. Add the present values together.
5. Compare the total present value to the asking price.
6. Decide whether your group would buy the business.

## Business 1: Elsah Coffee Cart

### Description

A student-friendly mobile coffee cart operates near campus events, morning classes, and weekend community gatherings. It has a loyal customer base, simple operations, and low growth. The owner is graduating and wants to sell the cart, equipment, brand name, and supplier contacts.

### Risk Profile

This is the lowest-risk business. Demand is steady, costs are understandable, and the equipment is simple. Growth is limited, but the cash flows are fairly predictable.

Suggested discount rate: **8%**

Asking price: **$92,000**

### Expected Annual Cash Flow

| Year | Expected Cash Flow |
|---:|---:|
| 1 | $22,000 |
| 2 | $24,000 |
| 3 | $25,000 |
| 4 | $26,000 |
| 5 | $27,000 |

### Questions

1. What is the present value of the five years of cash flow?
2. Is the present value higher or lower than the asking price?
3. What makes this business safer than the others?
4. What might limit its upside?

## Business 2: Riverbend HVAC Service

### Description

A small HVAC repair and maintenance company serves nearby homes, rental properties, and small businesses. It has repeat customers and strong demand during extreme weather. The current owner is willing to stay for six months to train the buyer.

### Risk Profile

This business has moderate risk. Demand is real, but the business depends on skilled labor, scheduling, reputation, and emergency calls. It can grow if the owner hires technicians, but hiring and service quality are not guaranteed.

Suggested discount rate: **14%**

Asking price: **$165,000**

### Expected Annual Cash Flow

| Year | Expected Cash Flow |
|---:|---:|
| 1 | $38,000 |
| 2 | $44,000 |
| 3 | $52,000 |
| 4 | $60,000 |
| 5 | $68,000 |

### Questions

1. What is the present value of the five years of cash flow?
2. Is the present value higher or lower than the asking price?
3. What hard skills would the owner need to understand this business?
4. What could go wrong if the business grows too quickly?

## Business 3: Campus Gear Rental App

### Description

A small startup rents outdoor gear, tools, project equipment, and event supplies to students and local residents through a simple app. The idea has strong growth potential, but it is still early. The business needs better software, marketing, and operational systems.

### Risk Profile

This is the highest-risk business. The upside could be large, but the cash flows are uncertain. It depends on student adoption, inventory management, app reliability, theft/loss control, and whether the idea can expand beyond one campus.

Suggested discount rate: **24%**

Asking price: **$110,000**

### Expected Annual Cash Flow

| Year | Expected Cash Flow |
|---:|---:|
| 1 | -$8,000 |
| 2 | $12,000 |
| 3 | $34,000 |
| 4 | $75,000 |
| 5 | $130,000 |

### Questions

1. What is the present value of the five years of cash flow?
2. Is the present value higher or lower than the asking price?
3. Why does this business require a higher discount rate?
4. What would you need to learn before trusting these projections?

## Group Decision

After valuing all three businesses, answer:

```text
Business 1 present value:
Business 1 asking price:
Would we buy it? Why or why not?

Business 2 present value:
Business 2 asking price:
Would we buy it? Why or why not?

Business 3 present value:
Business 3 asking price:
Would we buy it? Why or why not?
```

Then choose one:

```text
If our group had to buy one business, we would choose:

Our reason is:

The biggest risk is:

The first thing we would investigate before buying is:
```

## Discussion Questions

1. Which business looked most valuable before discounting?
2. Which business looked most attractive after discounting?
3. How did the discount rate change your opinion?
4. Which business has the best risk/reward tradeoff?
5. Which business would require the most hard skills from the owner?
6. What information would you want before making a real investment decision?

## Optional Challenge

Try changing each discount rate by 3 percentage points.

For example:

- Coffee cart: 8% becomes 5% or 11%
- HVAC service: 14% becomes 11% or 17%
- Gear rental app: 24% becomes 21% or 27%

Then answer:

```text
Which business valuation changed the most?

Why did that business change more than the others?

What does this teach us about risk and future cash flows?
```

## Final Reflection

Answer individually:

```text
One thing I learned about valuing a business is:

One thing that surprised me is:

One question I still have about discounting future cash flow is:
```
