## 🛒 End-to-End E-Commerce Customer Behavior Analysis

**📌 Project Overview**
This project analyzes customer shopping behavior using transactional data from 3,900 purchases across various product categories. The goal is to uncover insights into spending patterns, customer segments, product preferences, and subscription behavior to guide strategic business decisions.

**🛠️ Tech Stack & Workflow**
This project demonstrates a complete, end-to-end data analysis pipeline:


Python (Pandas): Performed initial data preparation and cleaning. Handled missing data by imputing the median rating for the review rating column based on product category. Standardized column names to snake case for better readability and engineered new features like age_group.


PostgreSQL: Connected the Python script to PostgreSQL and loaded the cleaned DataFrame for SQL analysis. Executed complex aggregations and structured queries to answer key business questions.


Power BI: Built an interactive dashboard to visually present KPIs, demographic breakdowns, and category performance for stakeholders.

📊 **Key Business Insights**
**1. Demographic Revenue Gaps**

**Insight:** Male customers accounted for significantly more revenue ($157,890) compared to Female customers ($75,191).

**Recommendation:** Investigate the steep drop-off in Female customer revenue. Reassess the female product line inventory and launch targeted marketing campaigns to capture this missing market share.

**2. The 80/20 Rule (Pareto Principle) Busted**
**Insight:** Contrary to standard retail expectations, revenue is perfectly flat across all 25 color variants. The top 5 selling colors combined generate only 22.5% of total revenue, and it takes the top 19 colors to reach nearly 80% of sales.

**Recommendation:** The brand must maintain a wide color assortment. Consolidating the catalog by cutting bottom-performing colors to save warehouse space would result in a significant loss of total revenue.

**3. Inventory Discount Dependency**
**Insight:** "Safe" neutral colors like White and Charcoal showed the highest dependency on discounts, requiring markdowns roughly 50% of the time to sell. Conversely, vibrant colors like Pink, Peach, and Brown were purchased at full retail price over 60% of the time.

**Recommendation:** Exclude low-dependency vibrant colors from site-wide sales to protect profit margins. Reserve deep discount campaigns specifically for moving high-dependency neutral inventory.

**4. Subscription Impact**

**Insight:** While non-subscribers make up 73% of the customer base , promoting exclusive benefits for subscribers and rewarding repeat buyers can help transition more users into the loyal segment.

**🚀 How to Run the Project**
Clone the repository to your local machine.

Review the Jupyter Notebook in the /notebooks folder to see the Python data cleaning and exploratory data analysis steps.

Execute the .sql scripts in your PostgreSQL environment to recreate the database and analysis.

Open the .pbix file in Power BI Desktop to interact with the visual dashboard.

Author: *Sauryayan Ralhi*
