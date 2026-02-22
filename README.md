Customer Shopping Behavior Analysis
## Project Overview
This project provides a comprehensive end-to-end analysis of customer purchasing patterns using a dataset of 3,900 transactions. The primary objective is to leverage consumer data to identify trends, improve engagement, and optimize marketing strategies. By integrating Python for data engineering, PostgreSQL for deep-dive analysis, and Power BI for interactive visualization, the project identifies key drivers of revenue and customer loyalty.
+4

## Tech Stack
Data Cleaning & Engineering: Python (Pandas, NumPy)

Database Management: PostgreSQL

Business Intelligence: Power BI

## Key Insights
### 1. Demographic & Revenue Drivers

Gender Contribution: Male customers generated significantly higher revenue ($157,890) compared to female customers ($75,191).
+1


High-Value Age Groups: Young Adults are the highest revenue contributors ($62,143), followed by Middle-aged customers ($59,197).
+2


Top Category: Clothing is the leading category in both total sales volume and revenue.
+1

### 2. Customer Segmentation & Loyalty

Loyal Segment: 3,116 customers are classified as "Loyal" based on extensive purchase history.


Subscription Landscape: Only 27% of customers are currently subscribers.


Subscription Parity: Interestingly, average spend is nearly identical between subscribers ($59.49) and non-subscribers ($59.87), suggesting a need to enhance subscriber-exclusive benefits.

### 3. Purchasing Behavior

Promotional Sensitivity: 839 customers used a discount while still spending above the average purchase amount ($59.76).
+1


Shipping Impact: Express shipping users tend to spend slightly more on average ($60.48) than standard shipping users ($58.46).


Product Performance: Top-rated items include Gloves (3.86) and Sandals (3.84).

## Project Workflow
### Phase 1: Data Preparation (Python)

Missing Data: Handled 37 missing values in the Review Rating column by imputing the median rating of the corresponding product category.
+1


Standardization: Renamed columns to snake_case and converted purchase amounts to a standard numeric format.


Feature Engineering: * Created age_group bins to analyze demographic spending.

Calculated purchase_frequency_days to understand customer return cycles.

Dropped the redundant promo_code_used column as it perfectly mirrored discount_applied.

### Phase 2: SQL Analysis
The cleaned data was migrated to PostgreSQL to answer critical business questions:


Product Performance: Identified top 3 products per category (e.g., Jewelry, Sunglasses, and Belts for Accessories).


Discount Rates: Found that items like Hats and Sneakers have the highest percentage of discounted purchases (~50%).


Segment Counting: Quantified the number of New, Returning, and Loyal customers.

### Phase 3: Visualization (Power BI)
Developed an interactive Customer Behavior Dashboard:
+1

KPI Tracking: Real-time monitoring of Number of Customers (3.9K), Avg. Purchase Amount ($59.76), and Avg. Review Rating (3.75).
+2


Behavioral Filters: Ability to slice data by Shipping Type, Category, Gender, and Subscription Status.
+2

## Business Recommendations

Subscription Growth: Promote exclusive benefits or loyalty rewards for subscribers to differentiate their spending from non-subscribers.


Loyalty Retention: Implement targeted "thank you" campaigns for the 3,116 Loyal customers to ensure long-term retention.


Targeted Marketing: Focus high-budget marketing efforts on the Young Adult demographic and Express Shipping users, as they show the highest revenue potential.


Inventory Optimization: Prioritize stock and prime placement for top-rated items like Gloves and Sandals.
