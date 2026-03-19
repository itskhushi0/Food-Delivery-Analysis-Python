# FoodHub Data Analysis Project

## Context
The number of restaurants in New York is growing rapidly, catering to busy professionals and students who rely on convenient food delivery options. **FoodHub**, a food aggregator company, allows customers to order from multiple restaurants via a single app. Once an order is confirmed, a delivery person picks up the food from the restaurant and delivers it to the customer. **FoodHub earns revenue by collecting a commission on each order**. The company has accumulated a dataset of customer orders and wants to analyze it to understand demand patterns, improve delivery efficiency, and optimize customer experience.

## Presentation
Check out the full presentation of this analysis [here](https://github.com/your-username/your-repo-name) 
---

## Business Summary & Key Insights
- **Top Cuisines:** American, Japanese, Italian, and Chinese.  
- **Top Restaurant:** Shake Shack.  
- **Demand Surge:** 71% of orders occur during weekends.  
- **Delivery Efficiency:** Weekday deliveries are slower (**28 minutes**) than weekends (**22 minutes**).  
- **Customer Ratings:** 39% of orders have no ratings.  
- **High-Value Orders:** Orders above **$20 account for 29.24% of revenue**.  
- **Premium Promotional Restaurants:** 4 restaurants qualify based on ratings (>50 ratings and average >4).  
- **Long Fulfillment:** 10.54% of orders take more than 60 minutes to deliver (preparation + delivery).  

---

## Methodology & Analysis

### 1. Data Preparation & Cleaning
- Imported dataset using `pandas` and `numpy`.  
- Checked data types, missing values, and cleaned `rating` column by converting to numeric where necessary.  
- Verified **dataset dimensions:** **1,898 rows × 9 columns**.  

### 2. Descriptive & Univariate Analysis
- **Summary Statistics (Food Preparation Time):**  
  - Min: 20 minutes  
  - Average: ~27 minutes  
  - Max: 35 minutes  

- **Top 5 Restaurants by Number of Orders:**

| Restaurant Name               | Number of Orders |
|-------------------------------|----------------|
| Shake Shack                    | 219            |
| The Meatball Shop              | 132            |
| Blue Ribbon Sushi              | 119            |
| Blue Ribbon Fried Chicken      | 96             |
| Parm                           | 68             |

- **Top 5 Frequent Customers (for promotions):**

| Customer ID | Number of Orders |
|------------|----------------|
| 52832      | 13             |
| 47440      | 10             |
| 83287      | 9              |
| 250494     | 8              |
| 82041      | 7              |

---

### 3. Multivariate Analysis
- **High-Performing Restaurants for Promotions (≥50 ratings, avg rating >4):**

| Restaurant Name              | Average Rating |
|------------------------------|----------------|
| The Meatball Shop            | 4.51           |
| Blue Ribbon Fried Chicken    | 4.33           |
| Shake Shack                  | 4.28           |
| Blue Ribbon Sushi            | 4.22           |

- **Revenue Analysis (Tiered Commission):**  
  - ≤$5: 0% commission  
  - $5–$20: 15% commission  
  - >$20: 25% commission  
  - **Total Net Revenue:** ~$6,166  

- **Orders Taking >60 Minutes (Preparation + Delivery):** 10.54%  
- **Mean Delivery Time by Day:**  
  - Weekdays: 28 minutes  
  - Weekends: 22 minutes  

---

### 4. Strategic Insights
- Implement a **customer feedback incentive program** to reduce unrated orders.  
- Optimize **weekday delivery operations** to improve speed and efficiency.  
- Promote **high-value bundled orders** (> $20) to increase revenue from the 25% commission tier.  
- Introduce a **minimum order value** or small order fee to capture revenue from low-cost orders.  
- Run **targeted marketing campaigns** for less popular cuisines to attract new customer segments.  

---

## Conclusion
This analysis provides FoodHub with actionable insights to optimize operations, improve customer experience, and increase revenue. By focusing on high-value orders, promoting top-performing restaurants, incentivizing customer feedback, and optimizing weekday deliveries, the company can improve service quality, increase profitability, and expand its customer base.
