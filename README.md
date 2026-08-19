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

