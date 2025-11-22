# Digital-Marketing-Campaign-Analytics
This project explores how digital platforms influence the performance of marketing campaigns

EXECUTIVE SUMMARY
 * This project explores how digital platforms influence the performance of marketing campaigns. It examines relationships between platform-specific activities and outcomes such as engagement, sales lift, lead generation, brand visibility, and customer retention. A structured database was built in MySQL to store and manage the data. Using SQL queries and aggregate functions, insights were generated on revenue growth, profit contribution, click performance, and platform effectiveness. These insights help guide budget allocation and strategic marketing decisions.

PROBLEM STATEMENT
 * The goal of this project is to determine how digital platforms contribute to campaign effectiveness by comparing cost and budget inputs to revenue and profit outputs. It also evaluates customer reach, ease of conversion, and the platforms that provide the highest value for money. Ultimately, the project identifies which channels deliver the best performance and where marketing funds should be prioritised.

TOOLS USED
 * MySQL, Excel, Power BI

DATA UNDERSTANDING
 * The project uses three core tables:
   * campaigns – campaign details, objectives, budgets, and timelines
   * ad_performance – impressions, clicks, revenue, and cost
   * platforms – monthly active users and platform characteristics

  * Each table was designed with appropriate data types, keys, and constraints to ensure referential integrity and accurate analysis.

METHODOLOGY
*  Database Setup
  * Removed any existing Digital_Marketing database to avoid duplicates.
  * Created a new database named Digital_Marketing in MySQL Workbench.
  * Selected the database for use with the USE statement.
  * Designed and created three tables: campaigns, ad_performance, and platforms.

<img width="1541" height="770" alt="Screenshot 2025-11-22 193133" src="https://github.com/user-attachments/assets/3c609b58-fd77-48ff-bf9a-d50404bc05c0" />
<img width="1550" height="772" alt="Screenshot 2025-11-22 193259" src="https://github.com/user-attachments/assets/a1cbcf78-3183-4c8a-858f-3c92a74c95c7" />
<img width="1558" height="929" alt="Screenshot 2025-11-22 193534" src="https://github.com/user-attachments/assets/b108fb54-9dc7-4457-9be5-e9462d000ea7" />

* Schema Design
  * For each column, the following specifications were applied:
    * VARCHAR, INT, BIGINT for text and numeric values
    * AUTO_INCREMENT for unique ID sequencing
    * PRIMARY KEY for table-level uniqueness
    * FOREIGN KEY constraints to establish relationships
    * DATE for all timeline fields
    * DECIMAL for monetary values and rates
    * NOT NULL to maintain data completeness
    * Defined appropriate length limits for all fields

   <img width="1541" height="768" alt="Screenshot 2025-11-22 193216" src="https://github.com/user-attachments/assets/52118db7-5923-4c51-b5ea-92503788ad37" />

* Data Preparation
  * Inserted multiple rows of data corresponding to each table.
  * Queried each table to validate successful data insertion and correctness.

<img width="1542" height="769" alt="Screenshot 2025-11-22 193236" src="https://github.com/user-attachments/assets/8f8b9377-8d48-4eea-b3a7-c0f25f3ed0b8" />

* Data Modeling
  * Relationships were built across datasets using common keys:

<img width="1731" height="592" alt="Screenshot 2025-11-22 164515" src="https://github.com/user-attachments/assets/a6789b4e-6ef2-46ef-875f-1b7afd61c25d" />
  
* Formulas and Key DAX Measures/Expressions

<img width="1239" height="350" alt="Screenshot 2025-11-22 164300" src="https://github.com/user-attachments/assets/76f6587d-20cc-47e1-b815-deacb742c8b4" />

* Exploratory Data Analysis
  * The Power BI dashboard leveraged DAX measures to explore revenue performance, profit contribution, platform reach, and campaign outcomes across marketing channels.
  * DAX calculations supported key KPIs such as Total Revenue, Profit Gained, Profit Margin, and ROI.
  * Insights were derived on platform efficiency, top-performing campaigns, and overall profit distribution

* Visualization
  * An interactive dashboard was developed to:
      * Present platform performance using bar charts showing reach, revenue, and profit share across all major channels.
      * Reveal seasonal and monthly shifts in earnings through a line chart illustrating the revenue trend across the year.
      * Compare platform efficiency using a bubble chart mapping impressions against monthly active users.

    *  The dashboard uses a well-blended color scheme and includes slicers for easy filtering and dynamic exploration, maintaining a clean, spacious layout for quick insights.
      
<img width="1164" height="652" alt="Screenshot 2025-11-22 171655" src="https://github.com/user-attachments/assets/c0c78e47-027c-4424-8dc7-2902c3ab9821" />
<img width="1162" height="653" alt="Screenshot 2025-11-22 162217" src="https://github.com/user-attachments/assets/6cc260ec-ac08-4da1-8bbe-56406efa7c27" />
<img width="1162" height="652" alt="Screenshot 2025-11-22 163143" src="https://github.com/user-attachments/assets/b7ee11f1-36ef-4f13-a0b7-cacf4375537d" />

* Analysis Approach
   * A range of SQL queries and aggregate functions were applied to derive insights:

      * Joined campaigns and ad_performance to analyse performance by campaign.
      * Calculated click-through rate (CTR) using total clicks and impressions.
      * Performed revenue vs cost computations to evaluate profit contributions.
      * Identified the top 5 performing campaigns by revenue.
      * Compared platform visibility through total impressions.

* Overall Performance Metrics
  * Total Impressions: 58.2K
  * Total Budget: 91.5K
  * Total Cost: 2145
  * Total Revenue: 6980
  * Total Profit: 4835
  * Profit Margin: 69%

* Impressions by Platform (Descending)
  * Facebook – 26K
  * Google Ads – 13.4K
  * Instagram – 12.7K
  * Twitter – 3300
  * LinkedIn – 2800

* Monthly Active Users (Global Estimates)
  * Total: 20.33 billion

  * Top platforms:
     * Google Ads – 3.5 billion
     * Facebook – 2.9 billion
     * YouTube – 2.3 billion
     * Instagram – 2 billion
     * WhatsApp – 2 billion

* Top Five Campaigns by Revenue and Profit
  * Campaign IDs: 5, 19, 8, 15, 1

* Top Five Months by Revenue
  * November – 2400
  * October – 850
  * July – 750
  * December – 700
  * September – 630

  * January recorded the lowest revenue at 130.


* Strategic Platform Opportunity Analysis (YouTube and WhatsApp)
  * YouTube and WhatsApp collectively account for 4.3 billion monthly active users, yet they were not utilised in the campaign strategies.
  * Their massive user bases present untapped opportunities to increase visibility, engagement, and ultimately revenue and profit.

YouTube Opportunity:
* YouTube’s video-driven environment makes it ideal for capturing user attention within the first few seconds.
* A significant portion of users do not subscribe to YouTube Premium, meaning ads are unavoidable and frequently repeated.
* This repetition strengthens brand recall and increases the likelihood of conversions.
* Video ads also provide richer storytelling and product demonstration opportunities, which can boost engagement and intent to purchase.

WhatsApp Opportunity:
* WhatsApp has become an everyday communication tool used across all age groups.
* The introduction of WhatsApp Channels presents a new and powerful avenue for digital marketing.
* Campaigns shared through channels or broadcast lists can spread quickly due to WhatsApp’s high engagement frequency.
* Since users open WhatsApp multiple times a day, the probability of repeated exposure is high, which can improve conversion rates.
* WhatsApp’s personal, conversational nature also enhances trust and increases the chances of customer interaction, referrals, and organic sharing.

   * Implication:
     * Leveraging YouTube and WhatsApp in future campaigns can significantly expand reach beyond the existing platforms and may lead to stronger brand awareness, higher conversions, and improved revenue performance.

* Platform Visibility Insights
  * Facebook (26K impressions): Wide global reach across all age groups, making it a highly effective channel for brand awareness and campaign engagement.
  * Google Ads (13.4K impressions): Dominates search-based advertising, ensuring that campaign-related ads appear prominently to users actively seeking relevant information.
  * Instagram (12.7K impressions): Leverages features like IG Shops and scrollable ad placements to engage users based on interests and demographics, boosting ad visibility.
  * Twitter (3.3K impressions): Lower visibility, likely due to its primarily text-based engagement and fast-moving feed.
  * LinkedIn (2.8K impressions): Niche platform focused on professional networking, recruitment, and B2B engagement, which limits broader campaign exposure

* Top Performing Campaigns
  * Top 5 campaigns by revenue and profit: Campaign IDs 5 > 19 > 8 > 15 > 1
    * Platforms used: Facebook and Google Ads
      * Insight: These campaigns demonstrate the effectiveness of combining high-reach platforms with strong ad strategies to maximise revenue and profit.

* Top Months by Revenue
  * Insights:
    * The second half of the year, particularly the last quarter, generates the highest revenue, suggesting that campaigns should be scaled and prioritised during these   months for maximum ROI.

    * Low-performing months: January recorded the lowest revenue at 130, with a slow trend continuing through mid-year, indicating limited engagement and conversion potential in the first half of the year.

* Financial Overview
  * The campaigns demonstrate strong value for money, generating significant returns relative to cost.
  * These profits could be reinvested into creating more engaging and targeted ads, expanding high-performing campaigns, and exploring new platforms to further increase reach, conversions, and revenue

RECOMMENDATIONS
* Allocate more budget to Facebook and Google Ads as they consistently deliver the highest revenue, profit, and conversions.
* Integrate YouTube and WhatsApp into future campaigns to leverage their massive user bases and habitual engagement for greater visibility and conversions.
* Focus marketing efforts on peak months, especially Q4 and November, to maximise revenue and ROI.
* Replicate strategies from the top 5 campaigns (IDs 5, 19, 8, 15, 1) and continuously optimise ad creatives, targeting, and messaging for improved performance.
* Track revenue, cost, and profit per campaign regularly to optimise budget allocation and identify underperforming campaigns early.
* Use multi-format advertising such as video, carousel, and interactive ads on YouTube and Instagram to boost engagement and conversion rates.
* Analyse the customer conversion path to identify drop-offs and refine engagement strategies for higher conversion efficiency.

CONCLUSION
* This project analysed digital marketing campaign performance across multiple platforms. Facebook and Google Ads delivered the highest visibility, conversions, and profit, with a total revenue of 6,980, profit of 4,835, and 361 conversions. Insights highlight the value of targeted campaigns, seasonal scaling, and opportunities to expand into untapped platforms like YouTube and WhatsApp. A data-driven approach ensures efficient budget use, maximises ROI, and supports long-term campaign growth.

