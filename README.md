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

