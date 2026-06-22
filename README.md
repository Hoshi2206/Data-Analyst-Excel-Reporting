# Data-Analyst-Excel-Reporting
End-to-end data preparation and executive reporting project in Microsoft Excel utilising 42,000+ rows of uncleaned Amazon product data.

# Amazon Products Sales Analysis (Excel Dashboard)

<img width="1627" height="1147" alt="image" src="https://github.com/user-attachments/assets/d05834dd-a0c2-4fda-811e-0169886def94" />

## Project Overview
This project focuses on the end-to-end data preparation, cleaning, and visual reporting of an Amazon product sales dataset containing over 42,000 items. Using **Microsoft Excel exclusively**, I transformed a messy, uncleaned dataset into an interactive executive dashboard to uncover product performance, pricing strategies, and customer engagement metrics.

## Data Source & Reference

The analysis and dashboard built in this project are powered by the following open-source dataset:

*   **Dataset Title:** Amazon Products Sales Dataset (42k+ Items)
*   **Source:** [Kaggle Dataset Repository](https://www.kaggle.com/datasets/ikramshah512/amazon-products-sales-dataset-42k-items-2025?select=amazon_products_sales_data_uncleaned.csv)
*   **Dataset Creator:** Ikram Shah
*   **Scope:** 42,000+ rows of uncleaned, real-world Amazon e-commerce product listings containing categorical variables, top-line performance metrics, and fragmented promotional attributes.

## Tech Stack & Skills Showcased
* **Data Organization:** Sorting, filtering, and cleaning structural inconsistencies across 42,000+ rows of messy data.
* **Data Summarization:** Building dynamic **Excel Pivot Tables** to aggregate large-scale product revenue and quantities.
* **Data Visualisation:** Creating clean Excel charts, slicers, and timelines for an interactive reporting dashboard.
* **Basic Formatting:** Applying number formatting (currency, percentages) and clean layouts to ensure the report is business-ready.

## Business Insights & Recommendations

## Promotional & Discount Strategy Analysis

<details>
<summary><b> 1. The Problem (Click to expand)</b></summary>

Product categories exhibit fragmented promotional responses, meaning customers in different segments prefer entirely different incentive structures (Coupon Discounts vs. Free Delivery). A one-size-fits-all promotional framework leads to revenue leakage and inefficient marketing spend.

</details>

<details>
<summary><b> 2. Key Insights (Click to expand)</b></summary>

* **Inelastic & Necessity-Driven Segments:** Customers purchasing *Office & Batteries* and *Printers & Ink* exhibit low promotional sensitivity. Because these items are workplace necessities, demand remains stable regardless of financial incentives.
* **The Shipping coupon:** *Apple Ecosystem* consumers show an overwhelming preference for **Free Delivery** over coupon discounts. Without explicit customer location data, this pattern strongly serves as a **hypothesis** that the target demographic faces unique shipping fee barriers or high baseline delivery friction, making shipping incentives far more enticing than standalone product discounts.
* **Coupon-Sensitive Segments:** In contrast, the *PC Components & Storage* segment is highly responsive to direct price slashes via **Coupon Discounts**.

</details>

<details>
<summary><b> 3. Strategic Recommendations (Click to expand)</b></summary>

* **Protect Margins on Necessities:** Systematically scale back both coupon and delivery promotions for *Office & Batteries* and *Printers & Ink* to directly increase net profit margins without hurting sales volume.
* **Hypothesis Testing via Targeted Marketing:** Validate the shipping friction hypothesis by running an A/B test on premium tech segments (like the *Apple Ecosystem*), selectively altering "Free Delivery" visibility to isolate whether delivery pricing is the definitive driver of high-value conversions.
* **Reallocate Promotional Capital:** Shift the budget saved from the office supplies segment to boost targeted **Coupon Discounts** for *PC Components & Storage* to maximize sales velocity.

</details>
</details>

## Ratings Cliff & Consumer Behavior Analysis

<details>
<summary><b> 1. The Problem (Click to expand)</b></summary>

When a product's average rating drops below the **4.0 threshold**, consumer conversion rates and purchase volume experience an absolute collapse, severely impacting platform GMV (Gross Merchandise Volume).

</details>

<details>
<summary><b> 2. Key Insights (Click to expand)</b></summary>

* **The 4.0 Critical Threshold:** Sales volume remains healthy between the 4.1 and 4.8 rating bands, but drops to near-zero once a product hits 4.0 or lower.
* **The High-Tier Premium Paradox:** Interestingly, items with near-perfect ratings (**4.9 and 5.0**) display surprisingly low transaction volumes. Further data cross-referencing reveals that these top-tier rated items carry the **highest average unit prices** on the platform. The lower volume is not due to poor reception, but because these are premium, high-ticket items with a naturally smaller, highly targeted buyer pool.

</details>

<details>
<summary><b> 3. Strategic Recommendations (Click to expand)</b></summary>

* **Implement Automated Merchant Alerts:** Develop an early-warning system in the merchant portal that flags products sliding down toward a 4.1 rating, prompting sellers to address customer friction before hitting the 4.0 conversion cliff.
* **Establish Seller Quality Governance:** Introduce strict compliance policies for underperforming merchants. Sellers who consistently allow products to drop below a 3.5 rating should face search-index deprioritization or temporary listing suspension to protect overall customer trust.

</details>

## Sales Dependency & Revenue Concentration Risk

<details>
<summary><b> 1. The Problem (Click to expand)</b></summary>

The business exhibits a high level of **revenue concentration risk**, where a massive portion of total volume and earnings is dependent on just a few critical product categories. If any of these top-performing categories experience a supply chain disruption or stockout, it will trigger an immediate downfall in platform revenue and damage customer fulfillment satisfaction.

</details>

<details>
<summary><b>2. Key Insights (Click to expand)</b></summary>

* **Filtering the Noise (Other Items):** While the *Other Items* category shows high volume, it represents an aggregate of various unrelated sub-categories. Therefore, its risk is naturally diversified and is excluded from the immediate threat zone.
* **The High-Risk:** The true operational vulnerability lies in the **Apple Ecosystem** and **Printers & Ink** categories. These segments represent concentrated pillars of the store's total volume. Because of their high sales velocity, any inventory shortage in these specific categories will disproportionately harm the business's bottom-line financial health.

</details>

<details>
<summary><b> 3. Strategic Recommendations (Click to expand)</b></summary>

* **Establish Safety Stock Buffers:** Implement a strict "Safety Stock" threshold for the *Apple Ecosystem* and *Printers & Ink* segments, ensuring minimum inventory levels are maintained to absorb sudden demand spikes or shipping delays.
* **Diversify Supplier Networks:** Form secondary sourcing partnerships for high-dependency components to mitigate the risk of a single point of failure in the supply chain.

</details>

## Paid vs. Organic Advertisement Performance

<details>
<summary><b> 1. The Problem (Click to expand)</b></summary>

The platform displays heavy volume variations between sponsored and organic traffic. However, because the raw dataset lacks financial advertising attributes (such as Cost-Per-Click or total campaign fees), the business faces blind spots regarding true net profitability and marketing efficiency.

</details>

<details>
<summary><b> 2. Key Insights & Constraints (Click to expand)</b></summary>

Based on the performance metrics in `image_8f1065.png` and `image_8f10ab.png`:
* **High-Volume Revenue Anchors:** The heavily sponsored segments serve as the primary revenue drivers for the platform. *Office & Batteries* generates **$61.76M** (2.47M units) and *Printers & Ink* pulls in **$100.04M** (1.41M units). This explicitly proves the advertising framework successfully scales top-line customer reach.
* **The Net Profit Margin Hypothesis:** Because *Office & Batteries* requires 8,436.05 sponsored units compared to only 3,484.05 organic units, the business is highly dependent on paid traffic. **Due to the lack of specific ad fee data, we must hypothesize** that if customer acquisition costs (CAC) follow industry-standard averages, the true net profit margins for these high-performing categories may be heavily compressed by hidden marketing overhead.

</details>

<details>
<summary><b> 3. Strategic Recommendations (Click to expand)</b></summary>

* **Maintain Current Paid Baselines:** Because these categories anchor our largest revenue pools ($61.76M and $100.04M), maintain current campaign settings to protect top-line cash flow until cost metrics are available.
* **Initiate a Data Infrastructure Request:** Partner with the data engineering or marketing teams to ingest ad spend/fee metrics into the database. This will allow the data model to transition from a top-line revenue view to a true Return on Ad Spend (ROAS) and net profitability analysis.
* **Proactive Organic SEO Testing:** To hedge against the hypothesis of compressed margins, begin low-cost organic search optimization (SEO) targeting for *Office & Batteries* keywords to naturally lift organic volume.

</details>
