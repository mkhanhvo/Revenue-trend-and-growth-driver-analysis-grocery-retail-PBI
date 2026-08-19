## 📊 Revenue Trend & Growth Driver Analysis | Grocery Retail | Power BI

### Author: Vo Tran Mai Khanh
### Date: 08/2026

## 📌 Background & Overview

### 📖 Objective
- Trace the revenue decline back to abnormal points in the trend line (the Dec 2016 peak followed by a sustained drop) to pinpoint when and where the shift began
- Break down performance by market and product category to isolate which segments (e.g. Meat) are driving the abnormal pattern versus following the general trend
- Examine store level attributes (Store Area, Opening Hours, etc.) to identify structural factors that distinguish above vs. below average performing stores

### 👤 Who is this project for?
- Business stakeholders / management in retail who need to understand revenue trends and identify where to act to prevent further decline
- Sales & category management teams looking to evaluate performance by market and product category (e.g. which categories or markets need intervention)
- Store operations teams interested in how store attributes (hours, area) relate to performance

### 👤 Client Background
The U.S. based retail company operating across 11 markets offers a mix of food and non food product categories. The business runs at store level with performance tracked through revenue, product category breakdowns and store attributes such as opening hours, store area, hours own, hours lease, etc. giving visibility into how each market and store contributes to overall results

### 📊 Data Structure & Relationships

#### 1️⃣ Tables Used:
- Sale figures: contains 7,650 records, each representing the total revenue of a single product category, for a single store, at a single point in time. It also carries the store's opening hours and opening type as repeated single values on every row, even though these attributes only vary at the store level
- Opening scheme contains 600 records, each representing a store's opening scheme for a given month. It captures store name, country, and city, indicating where each store is located
- Dimensions tables: date, store, dept (category)

#### 2️⃣ Table Schema & Data Snapshot

#### Table 1: Sale figures
<img width="485" height="95" alt="image" src="https://github.com/user-attachments/assets/478dec55-42e7-4049-a56a-f0c5e895e201" />

#### Table 2: Opening scheme
<img width="1037" height="94" alt="image" src="https://github.com/user-attachments/assets/b71b0e87-eab8-45d2-add4-24a1f93a4a6c" />

#### Table 3: Dim date

<img width="885" height="241" alt="image" src="https://github.com/user-attachments/assets/61c2eaed-4000-4f05-b77f-e9522adec913" />

#### Table 4: Dim dept (category)

<img width="146" height="283" alt="image" src="https://github.com/user-attachments/assets/fe8703fe-cd24-4250-bb71-062b1787e29f" />

#### Table 5: Dim store

<img width="256" height="545" alt="image" src="https://github.com/user-attachments/assets/acbe1f12-8369-4616-b6f3-9c65d8babe71" />

## 📊 Key Insights & Visualizations

### 1️⃣ Revenue & Trend Summary

<img width="819" height="539" alt="image" src="https://github.com/user-attachments/assets/262e3087-6309-48fc-a529-7aece93fe1dc" />

Total revenue reached $7.4B, generated from 2B units sold across all markets. Revenue climbed through Q4 2016, peaked in December, then dropped sharply in early 2017 before stabilizing at a lower, consistent level through mid-2017. Average revenue per store stands at $148.9M, with stores collectively operating 160K opening hours across the period

#### Regional trend
The December downturn wasn't isolated to a single market since nearly all countries recorded a similar drop around the same time, suggesting a shared external driver (seasonal demand shift, pricing or supply issue) rather than a market specific problem

#### Product performance
Most product categories tracked closely with the overall revenue trend but Meat stood out as an outlier, its performance swings appear to be the main driver behind the broader sales dip, making it the category to investigate first

#### Market view
Across every country, Meat consistently outperforms other categories, confirming it as the most in demand product and a strong candidate for further investment. However, Meat also saw the sharpest decline at the end of 2016 and has yet to recover, which is likely dragging overall revenue down with it

#### Germany vs. Denmark
Germany contributes the highest revenue across the entire period, while Denmark consistently sits at the opposite end, contributing the least in nearly every month. Since revenue is largely driven by sales volume, Denmark's lower unit sales rather than pricing and appear to be the main factor behind its weaker revenue contribution

### 2️⃣Operational Factors

#### *Monthly Snapshot - Nov 2016*

<img width="1568" height="621" alt="image" src="https://github.com/user-attachments/assets/694903b4-e8bb-4df7-9fd9-3a37e09c4bc8" />

#### *Monthly Snapshot - Dec 2016*

<img width="1568" height="630" alt="image" src="https://github.com/user-attachments/assets/d19d0e02-bc2a-4469-8df4-4e4f9ff5528a" />

#### *Monthly Snapshot - Jan 2017*

<img width="1568" height="625" alt="image" src="https://github.com/user-attachments/assets/5fad7a88-f41f-4796-9eab-51006e3f2438" />

### 📌 Analysis 1. Revenue & Volume Correlation
Total revenue and total sold units moved in near perfect lockstep across Nov 2016 – Jan 2017 (+12.9%/+14.3%, +30.6%/+27.2%, then -43.3%/-40.4%), confirming revenue changes in this period were volume driven, not price driven. Since both metrics rose and fell together at the same magnitude and direction, the shift in customer demand is the primary lever behind revenue performance

#### 📌 Analysis 2. Opening Hours Moves Inversely to Demand
Notably, opening hours decreased in both Nov (-3.0%) and Dec (-5.5%), the two months revenue peaked, then increased in Jan (+9.1%), the month revenue collapsed. This inverse relationship rules out more hours open as the driver of the Nov - Dec surge and also rules out fewer hours open as the cause of the Jan crash. It reinforces that the swing is demand driven, most likely a seasonal, holiday driven spike in Nov - Dec followed by a natural post holiday correction in January, rather than an operational or capacity issue

#### 📌 Analysis 3. Category Level Consistency
Meat remained the top performing category throughout all three months and mirrored the same swing pattern as total revenue, spiking in December alongside the aggregate trend, then pulling back sharply in January across every major market (Germany, UK, France, Italy) at a similar pace. This uniform movement across markets and the leading category further confirms the driver is systemic/seasonal rather than isolated to one product line or region

#### 📌 Analysis 4. Revenue per Store tracks Total Revenue exactly
Revenue/Store rose and fell by the identical percentage as Total Revenue in all three months (12.9%, 30.6%, -43.3%), indicating the number of active stores stayed constant across this period, the swing is purely a same-store demand effect, not a result of stores opening or closing

### 3️⃣Market & Product Contribution

#### *Snapshot Q4 2016*

<img width="985" height="256" alt="image" src="https://github.com/user-attachments/assets/941c9708-8094-4639-8cc2-be1e67eda093" />

#### *Snapshot H1 2017*

<img width="984" height="257" alt="image" src="https://github.com/user-attachments/assets/e7d5d941-1a25-47a3-b5f2-210f0caaf870" />

#### 📌 Analysis 1. Country Revenue Contribution
Despite the differing time ranges (Q4 2016 vs. six months in H1 2017), Germany consistently leads total revenue contribution across all markets in both periods, driven by top performance in most categories, including Meat, Dry, Clothing, Frozen and Household. Germany trails slightly behind France and the UK only in Delivery, but this gap is too small to affect its overall lead. Given its scale and consistency across nearly every category, Germany stands out as the strongest market for continued investment

#### 📌 Analysis 2. Product Contribution
Despite the differing time ranges, Meat remains the top revenue generating category in virtually every market across both periods, reflecting consistent customer demand regardless of country. This makes Meat the clearest category level priority, not just a Germany specific trend, but a demand pattern that holds globally

Non Food|Others category shows zero revenue across all 11 markets in both periods, this is unlikely to reflect genuine zero demand and more likely points to a data quality issue (an inactive category or mapping gap) that should be verified before drawing conclusions. Similarly, Belgium shows zero Delivery revenue in both periods while every other market reports some level of activity, suggesting Delivery may not have been offered in Belgium during this timeframe rather than a demand issue

Hardware and Household consistently rank as the lowest performing active categories across nearly every market, with no significant outliers by country. This is consistent with the store's grocery led format - customers prioritize food categories over durable/non-food goods, which is expected behavior rather than a concern

### Recommendation
#### 1. Capitalize on seasonal demand (Nov-Dec)
Nov - Dec 2016 revenue spike appears driven by seasonal demand (likely holiday related) rather than extended opening hours or pricing changes. Inventory, staffing, and marketing campaigns should be planned earlier to maximize this peak window, particularly for the Meat category.
#### 2. Double down on the Meat category
Meat leads revenue in nearly every market across both periods, making it the clear priority for continued investment - supply, shelf space and promotions while also being closely monitored, as it's the category most responsible for driving overall revenue swings
#### 3. Prioritize Germany as the core growth market
Germany leads revenue across most categories and remains consistent across periods, positioning it as the strongest candidate for further investment - additional stores, extended hours or expanded assortment before scaling efforts to other markets
#### 4. Diagnose low contributing markets before investing (e.g. Denmark, Belgium)
Before allocating more budget, confirm why these markets underperform - fewer stores, smaller store area, shorter opening hours or genuinely lower local demand. Benchmark them against a similarly sized but better performing market (e.g. Netherlands, Sweden) on the same store attributes to isolate the real gap and pilot any adjustment (e.g. extended hours at a few stores) before scaling. Note that Germany's scale skews comparisons - the goal is checking underperformance relative to each market's own potential, not forcing parity with Germany.
#### 5. Investigate the January post holiday drop
While the drop appears to be a natural post-holiday correction, further investigation is needed to confirm contributing factors (e.g. leftover inventory from December, early-year spending pullback) to better manage this seasonal dip in future cycles.
Resolve data quality issues before further analysis
#### 6. Deprioritize Hardware & Household expansion
These categories consistently rank lowest but remain active across all markets, consistent with the store's grocery led format. Maintain minimal viable stock rather than expanding investment here, if underperformance persists, consider reallocating their shelf space toward higher demand food categories like Meat
