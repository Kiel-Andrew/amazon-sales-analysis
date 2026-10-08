# Amazon Pricing Strategy & Consumer Sentiment Analysis

## 🎯 Business Use Case
E-commerce sellers and retail managers frequently struggle to optimize their pricing strategies. A common assumption is that massive discounts are necessary to drive sales volume, but there is often a fear that pricing a product too low will damage its brand perception and make it look "cheap" to consumers. 

The focus of this analysis is to evaluate real-world Amazon product data to determine the actual relationship between discount strategies, market saturation, and customer satisfaction. 

### Core Questions Addressed:
1. **Engagement vs. Margin:** Do steeper discounts actually drive enough user engagement (review volume) to justify the price cut?
2. **Perception of Quality:** Does heavily discounting a product negatively impact its average customer rating?
3. **Category Baselines:** Which specific product categories rely the most on aggressive promotional pricing to survive?
4. **Market Saturation:** Do cheaper product categories automatically dominate market inventory?

## 🛠️ Tools & Techniques Used
*   **Microsoft Excel:** Data Cleaning, Data Modeling, Pivot Tables, Advanced Charting (Combo Charts, Secondary Axes).
*   **Statistical Control:** Applied minimum sample size thresholds ($n \ge 30$) to filter out low-volume anomalies and ensure statistical significance across all category averages.

## 🧹 Data Cleaning & Preparation
The raw dataset required extensive cleaning before analysis could begin. Key transformations included:
*   **String Manipulation:** Extracted primary product categories from nested strings using text-to-columns and `SUBSTITUTE()` formulas.
*   **Data Type Standardization:** Stripped currency symbols and commas from pricing and rating count columns to convert text into calculable integers.
*   **Bias Mitigation:** Identified a low-sample-size bias in niche categories and applied Value Filters to exclude categories with fewer than 30 products, ensuring accurate average calculations.

## 📊 The Dashboard
<img width="1005" height="474" alt="image" src="https://github.com/user-attachments/assets/1f92b547-e140-4ff0-8cd5-47673a497de1" />
<img width="1006" height="475" alt="image" src="https://github.com/user-attachments/assets/fa744a87-2a13-4d80-a208-43a9b8bfc130" />
<img width="1006" height="474" alt="image" src="https://github.com/user-attachments/assets/386176bf-768e-4652-9642-d47477cf8d31" />
<img width="1006" height="474" alt="image" src="https://github.com/user-attachments/assets/aebf1811-370f-424a-8d6d-b6dad09e958a" />


## 💡 Key Business Findings

**1. Massive discounts drive massive attention.**
Slashing prices is a proven way to get eyes on a product. Items discounted by more than 60% generate significantly more customer reviews—a strong indicator of high sales volume—compared to items sold near full retail price.

**2. Discounts do not damage brand reputation.**
A common business fear is that heavy discounts make a product look "cheap" or low-quality. The data disproves this. Products in the highest discount brackets maintained strong average customer ratings (exceeding 4.2 out of 5 stars), proving that shoppers simply feel they are getting a great deal rather than buying a subpar item.

**3. Pricing strategies must be tailored by category.**
There is no one-size-fits-all approach to sales. The **Computers & Accessories** category relies heavily on constant promotional pricing, averaging a 54% discount just to compete. In contrast, **Office Products** rarely go on sale (averaging just a 12% discount) but still maintain excellent customer satisfaction and consistent sales.

**4. High prices do not stop a market from growing.**
Market saturation is not tied to cheap goods. The **Electronics** category dominates the market with the highest number of available products in the dataset, despite carrying a massive average price point of over $10,000. Consumers are highly willing to spend money in this space, making it both lucrative and highly competitive.

## 🚀 Strategic Recommendations
*   **Launch Strategy:** Use steep flash sales (>60% off) to build early review momentum for new products, as this drives engagement without harming the perceived quality rating.
*   **Margin Protection:** Avoid deep discounts on needs-based items like Office Products. Customers buy these based on necessity rather than impulse, so lowering the price cuts into profits without significantly increasing the volume sold.
