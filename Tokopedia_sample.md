# Project Background

As a data analyst at Tokopedia, one of Indonesia's largest e-commerce marketplaces, I analyze the vast amounts of data we collect daily to drive business decisions. Tokopedia operates in the e-commerce industry and has been active since its founding, growing to become a major player in Indonesia's digital economy. Our business model connects 14 million merchants with millions of customers across Indonesia, facilitating approximately 1.8 billion product transactions daily[1].

Our key business metrics include merchant reliability, customer satisfaction, transaction volume, and marketplace effectiveness. My role involves synthesizing and analyzing millions of merchant and customer data points to identify trends, optimize operations, and improve the overall marketplace experience[1].

Insights and recommendations are provided on the following key areas:

- Category 1: Merchant Performance Analysis
- Category 2: Customer Behavior Patterns
- Category 3: Product Category Performance
- Category 4: Regional Sales Distribution

The SQL queries used to inspect and clean the data for this analysis can be found here [link].

Targeted SQL queries regarding various business questions can be found here [link].

An interactive Tableau dashboard used to report and explore sales trends can be found here [link].

# Data Structure & Initial Checks

The company's main database structure as seen below consists of four tables: Merchants, Customers, Products, and Transactions, with a total row count of 24.7 million records. A description of each table is as follows:

- Table 2: Merchants - Contains merchant profiles, including ID, name, category, location, and reliability score
- Table 3: Customers - Contains customer information, including demographics, purchase history, and satisfaction ratings
- Table 4: Products - Contains product details, including ID, name, category, price, and inventory status
- Table 5: Transactions - Contains transaction records, including purchase date, customer ID, merchant ID, product ID, and transaction value

[Entity Relationship Diagram here]

# Executive Summary

### Overview of Findings

Our analysis reveals that merchant reliability directly impacts customer satisfaction and transaction volume, with high-scoring merchants generating 37% more repeat purchases. Product categories showing the strongest growth include electronics and home essentials, with a 28% year-over-year increase. Regional analysis indicates that while Java dominates sales volume, emerging markets in Eastern Indonesia show the highest growth rates at 42% annually.

[Visualization, including a graph of overall trends or snapshot of a dashboard]

# Insights Deep Dive

## Category 1: Merchant Performance Analysis

### Main insight 1.

Merchant reliability scores strongly correlate with customer retention. Merchants with reliability scores above 85% show a 37% higher rate of repeat customers compared to those with scores below 70%. This trend has remained consistent over the past 12 months, indicating the importance of merchant quality in driving customer loyalty.

### Main insight 2.

New merchants (active less than 6 months) experience a 23% higher cart abandonment rate compared to established merchants. Analysis shows this is primarily due to inconsistent stock management and delayed shipping confirmations, highlighting the need for better onboarding and training for new sellers.

### Main insight 3.

Merchants who respond to customer inquiries within 2 hours achieve 42% higher conversion rates than those who respond after 24+ hours. This pattern is particularly pronounced in high-value product categories such as electronics and furniture, where customer decision-making often requires additional information.

### Main insight 4.

The implementation of our merchant scoring system has improved overall marketplace quality, with average merchant reliability increasing from 76% to 83% over the past year. This system has been particularly effective in identifying low-performing merchants and providing targeted improvement recommendations.

[Visualization specific to category 1]

## Category 2: Customer Behavior Patterns

### Main insight 1. 

Mobile app users complete 73% more transactions than web-only users, with an average basket size 18% larger. This trend has accelerated over the past 6 months, coinciding with our app redesign and improved mobile checkout experience launched in October 2024.

### Main insight 2. 

Customer retention rates vary significantly by age demographic, with 25-34 year olds showing the highest loyalty (68% making repeat purchases within 30 days) compared to 18-24 year olds (42%). Analysis of browsing patterns suggests younger users are more price-sensitive and compare across multiple platforms.

### Main insight 3. 

Customers who engage with product reviews are 3.2 times more likely to complete a purchase than those who don't. This behavior is consistent across all product categories but is most pronounced in electronics and fashion, where product quality assessment is crucial to purchase decisions.

### Main insight 4. 

Payment method preferences show strong regional variation, with digital wallets dominating in urban areas (62% of transactions) while cash-on-delivery remains prevalent in rural regions (47% of transactions). This insight has significant implications for our payment processing strategy and merchant training.

[Visualization specific to category 2]

## Category 3: Product Category Performance

### Main insight 1. 

Electronics and home essentials have shown the strongest growth at 28% year-over-year, outpacing the marketplace average of 17%. This growth accelerated particularly during Q1 2025, coinciding with our promotional campaign targeting home office setups.

### Main insight 2. 

Seasonal variation in product categories is significant, with fashion items peaking 45 days before major holidays and food/grocery items showing 3.2x normal volume during rainy season months (November-February). These patterns have remained consistent for three consecutive years.

### Main insight 3. 

Cross-category purchasing behavior reveals strong correlations between certain product groups. Customers who purchase baby products are 4.7 times more likely to also purchase home organization items within 60 days, suggesting an opportunity for targeted bundle promotions.

### Main insight 4. 

Product categories with the highest return rates (fashion at 18% and electronics at 12%) also show the highest sensitivity to detailed product descriptions. Items with comprehensive specifications and multiple images experience 37% fewer returns than those with minimal information.

[Visualization specific to category 3]

## Category 4: Regional Sales Distribution

### Main insight 1. 

While Java accounts for 68% of total transaction volume, emerging markets in Eastern Indonesia show the highest growth rates at 42% annually. Sulawesi in particular has emerged as a high-potential region with transaction volumes doubling in the past 18 months.

### Main insight 2. 

Urban-rural disparities in delivery times significantly impact customer satisfaction scores. Rural customers who receive deliveries within the estimated timeframe give satisfaction ratings 28% higher than the average, highlighting the importance of accurate delivery estimates.

### Main insight 3. 

Regional preferences for product categories show distinct patterns, with electronics dominating in urban centers (32% of sales) while agricultural supplies and household essentials lead in rural areas (41% combined). These patterns have remained stable over the past 24 months.

### Main insight 4. 

Promotional effectiveness varies by region, with flash sales driving 3.5x normal volume in Greater Jakarta but only 1.8x in outer islands. Conversely, free shipping promotions show stronger performance in distant regions, generating 2.7x lift compared to 1.4x in Java.

[Visualization specific to category 4]

# Recommendations:

Based on the insights and findings above, we would recommend the Marketplace Operations team to consider the following:

* Merchant reliability directly impacts customer retention and transaction volume. Implement a more comprehensive onboarding program for new merchants focused on inventory management and communication best practices.

* Mobile app users complete significantly more transactions with larger basket sizes. Increase investment in mobile app features and performance optimization, particularly focusing on the checkout experience.

* Product categories show strong seasonal variations and regional preferences. Develop region-specific promotional calendars that align with local seasonal patterns and product preferences.

* Cross-category purchasing behavior reveals strong correlations between product groups. Create targeted bundle promotions for highly correlated product categories, such as baby products and home organization items.

* Payment method preferences vary significantly by region. Expand payment options in rural areas while providing additional security features for digital wallet users in urban centers.

# Assumptions and Caveats:

Throughout the analysis, multiple assumptions were made to manage challenges with the data. These assumptions and caveats are noted below:

* Assumption 1: Merchants with no reliability score data (approximately 3% of the database) were excluded from the merchant performance analysis to avoid skewing results.

* Assumption 2: Transaction data for February 2025 showed anomalies due to system maintenance - values were normalized based on January 2025 data and historical February patterns.

* Assumption 3: Customer geographic location was determined by shipping address for analysis purposes, which may not reflect actual customer residence in all cases.
