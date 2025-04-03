# LinkedIn Growth AnaLysis


## Project Overview
This project leverages LinkedIn data to analyze audience behavior, demographics, and interaction patterns. By examining key metrics such as impressions, engagements, follower growth, and geographic reach, the analysis provides actionable insights for improving LinkedIn performance. The findings aim to bridge gaps between impressions and engagements, identify growth opportunities, and enhance overall audience connection on the platform.


## Problem Statement
Despite high visibility and diverse audience demographics on LinkedIn, engagement remains lower than anticipated. Periods of inactivity and underperformance hinder the ability to maximize LinkedIn as a tool for growth and connection. Without addressing these gaps, the platform’s potential to foster meaningful professional relationships and conversions remains underutilized.


## Project Objective
The objective of this LinkedIn-focused analysis is to:

**Understand Audience Behavior**: Identify key trends and patterns in LinkedIn engagement, follower growth, and demographic interaction.

**Enhance Platform Performance**: Address gaps such as low engagement rates and inconsistent activity to optimize LinkedIn strategies.

**Leverage Data-Driven Insights**: Use data to guide content creation, improve impressions-to-engagement conversion, and maintain consistent growth.

**Expand Reach and Impact**: Develop tailored approaches to strengthen professional connections and broaden the audience base on LinkedIn.


Our data for this analysis was exported from LinkedIn and contains an excel file, having five different sheets.


### 1. Discovery Sheet
**Overall Performance**:
This column covers key metrics that summarize the performance of LinkedIn activities over the specified date range (from July 31, 2024, to March 30, 2025). It could include cumulative data such as impressions, engagements, follower growth, or other overarching statistics.


### 2. Engagement Sheet
**Date**:
The specific calendar date when LinkedIn posts or activities occurred.


**Impressions**:
The total number of times your LinkedIn posts were displayed to users on the platform.

**Engagements**:
The total number of interactions with your posts, including likes, comments, shares, or other forms of audience interaction.


### 3. Top Posts Sheet
**Post URL**:
The direct link to the LinkedIn post, enabling quick access to review its content and details.


**Post Date**:
The publication date of the LinkedIn post, showing when it was shared on the platform.


**Engagements**:
The total number of interactions (e.g., likes, comments, shares) that the specific post received.


**Impressions**:
The number of times the post was displayed to users. This metric indicates its visibility and reach.


**Note**: The initial version of the sheet contained duplicate or extra columns (like Unnamed: 3). After cleaning, the columns were simplified for clarity and usability, retaining only the essential fields.


### 4. Followers Sheet
**Date**:
The specific date on which the follower growth data was recorded.


**New Followers**:
The number of new LinkedIn followers gained on that date. This provides insight into audience growth over time.


### 5. Demographics Sheet
**Top Demographics**:
The categorization of your audience based on attributes such as job titles, locations, industries, or seniority levels.


**Value**:
The specific subgroup within the demographic category (e.g., "Data Analyst," "Lagos").


**Percentage**:
The proportion of the audience that belongs to this subgroup, expressed as a percentage of the overall audience.


This breakdown provides a comprehensive understanding of the data structure across the sheets. The cleaned dataset ensures clarity, making it easier to derive actionable insights such as performance trends, audience engagement patterns, follower growth, and demographic composition.


## Discovery Table
From the discovery table, we did the following analysis:

#### Impressions (10,839) 
 - This is the total number of times our content was displayed. It includes repeated views from the same users. It Measures how well our content is being distributed by LinkedIn’s algorithm. A rising trend suggests good content strategy and platform optimization

#### Members Reached (1,493)
 - This is the number of unique people who saw our content. Shows how many unique people are seeing our content. If this grows, our network and organic reach are expanding.

#### What this means?
- On average, each person who saw your content saw it multiple times (7.26 times)
- A higher impressions-to-reach ratio suggests strong content visibility, possibly due to LinkedIn's algorithm resurfacing our posts.

#### Actionable Insight:
 - If Impressions are high but Reach is low, it means LinkedIn is showing our posts to the same audience repeatedly. We might need to engage with new people, use hashtags, or post at different times to expand reach.


## Engagement Table
From the engagement table, we did the following analysis

**Date Conversion**: The Date column in the engagement table (df_eng) is converted into a datetime format, enabling advanced time-based operations.

**Monthly Aggregation**: The engagement data is grouped by months using the .dt.to_period("M") function. This groups all rows from the same month and sums up numeric columns (like Impressions and Engagements).

**Formatting for Plotting**: The resulting monthly data's index (representing months) is converted into strings, making it easier to use for plotting or further analysis.

**Output**: The df_monthly table contains aggregated monthly totals for numeric columns (e.g., total Impressions and Engagements), offering a clear view of trends over time.

This summarized table reveals how engagement metrics (impressions and engagements) have evolved month by month, which is useful for identifying trends or seasonal patterns in LinkedIn activity.

Furthermore, the sum of all impressions is 10,839, indicating the total visibility of LinkedIn posts, while the sum of all engagements is 261, reflecting the overall audience interactions (likes, comments, shares, etc.) within the specified timeframe. This provides a snapshot of LinkedIn performance metrics.


![Monthly Impression Trend](https://github.com/Phenomkay/LinkedIn-Growth-Analysis/blob/353c2b3885b1ca83604a4206b9294efc0b947887/Monthly%20Impression%20trend.png)

### Key insights
**Upward and Downward Trends**: The impressions increased steadily from July to October 2024, peaking at approximately 1600 impressions in October. This upward trend suggests strong engagement during these months.
A sharp drop occurred in November 2024, where impressions hit around 450. This is an anomaly worth investigating, perhaps an operational issue, seasonal effect or lack of consistent posting.

**Notable Recovery**: Impressions rebounded in December 2024, reaching a new peak around December 2024 with approximately 1960 impressions. This sharp recovery could be due to a campaign launch, holiday season, or some other impactful event.

**Stability with Growth**: After a slight drop in January 2025, there's a stable upward trajectory in February and March 2025, ending again at around 2000 impressions. This consistent growth indicates positive engagement or a successful strategy being implemented during this period.

### Insights and Recommendations:
**November and January's low Impressions**: We will examine why impressions dropped in November and January. Was there a data glitch, system downtime, or was it intentional?

**Sustain the Momentum**: The upward trend in February and March is promising, we will continue whatever strategies are driving engagement.

**Evaluate Seasonal Effects**: October and December show peaks, we will consider whether certain times of year drive higher impressions and plan campaigns accordingly.


![Monthly Engagement Trend](https://github.com/Phenomkay/LinkedIn-Growth-Analysis/blob/dcc658906dd816ccefdfd10c69c2562aea2eb13b/Monthly%20Engagement%20Trend.png)

### Key Observations and Insights:
**Engagement Peaks**: September 2024 shows the highest engagement (67). March 2025 approaches this peak with 63 engagements.

**Engagement Declines**: July 2024, November 2024, and January 2025 show 1 and 9 engagements respectively. It’s worth investigating what led to these stagnations, they may have been due to system downtime, lack of activity, or other external factors.

**Sharp Fluctuations**: There’s a sharp drop from September 2024 (67) to October 2024 (24). A similar drop occurs between December 2024 (44) and January 2025 (9). However, February and March 2025 demonstrate a consistent recovery trend.

**Overall Recovery**: Engagements consistently grow from February to March 2025, signaling improved strategies or reactivation efforts.

### Recommendations:
**Investigate Low Engagement Months**: We will examine November 2024, and January 2025 to understand what caused the inactivity.

**Build on Peaks**: We will also identify what drove engagement in September 2024 and replicate similar strategies. The growth from February to March 2025 is also promising, consider scaling these initiatives.

**Address Sudden Drops**: Understand the reasons behind sharp engagement drops (e.g., October to November 2024, December 2024 to January 2025) to avoid similar declines in the future.


### Engagement Rate
The Engagement Rate for each month in the df_monthly table was determined by dividing the total monthly engagements by the total monthly impressions and multiplying by 100 to express it as a percentage. The new column, "Engagement Rate (%)", adds insight into how effectively impressions translate into interactions on a monthly basis. 


![Monthly Engagement Rate Trend](https://github.com/Phenomkay/LinkedIn-Growth-Analysis/blob/dcc658906dd816ccefdfd10c69c2562aea2eb13b/Monthly%20Engagement%20rate%20trend.png)

### Key Observations:
**Peak Engagement**: The 5.3% engagement rate in September 2024 is remarkable. It suggests impactful campaigns, activities, or external factors driving high interaction.

**Periods of Inactivity**: November 2024 and January 2025 recorded 0.2% and 1.2% engagement rates respectively. These months require further investigation to identify causes like operational pauses, external disruptions, or changes in strategies.

**Recovery Trend**: Despite lows in November and January, the engagement rate shows steady improvement from February to March 2025, reaching  approximately 3%.

### Insights and Recommendations:
**Examine September's Peak**: We will identify drivers of the high engagement rate in September and determine how to replicate these successes.

**Investigate Zero Engagement**: November and January warrant attention, so we will look into system downtime, lack of campaigns, or other influencing factors during these months.

**Capitalizing on Recovery**: The upward trend from February to March reflects renewed interest. We will build on this momentum with targeted campaigns or activities to sustain growth.

**Consistency is Key**: We will consider implementing strategies to maintain stable engagement throughout the year rather than facing sharp fluctuations.

| Date       | Engagements | Impressions | Engagement Rate (%) |
|------------|-------------|-------------|----------------------|
| 2024-07    | 0           | 0           | NaN                 |
| 2024-08    | 19          | 835         | 2.275449            |
| 2024-09    | 67          | 1264        | 5.300633            |
| 2024-10    | 24          | 1602        | 1.498127            |
| 2024-11    | 1           | 440         | 0.227273            |
| 2024-12    | 44          | 1955        | 2.250639            |
| 2025-01    | 9           | 708         | 1.271186            |
| 2025-02    | 34          | 1888        | 1.800847            |
| 2025-03    | 63          | 2147        | 2.934327            |


We also calculated the average engagement rate across all months in the dataset by taking the mean of the "Engagement Rate (%)" column in df_monthly. The result is approximately 2.19%, indicating that on average, about 2.19% of impressions resulted in engagements during the analyzed period. This metric provides a benchmark for evaluating LinkedIn audience interaction over time.


## Top Post Table
For the top post table, we did the following

Cleaning the "Top Posts" table for clarity and better usability. 
 - First, column names were standardized to ensure consistency and readability. Duplicate columns, such as repetitive Post URLs and Post Dates, along with irrelevant fields, were removed to simplify the dataset. The "Post Date" column was converted to a datetime format to enable sorting the posts chronologically. Finally, the table was sorted by "Post Date," and the index was reset to provide a streamlined and organized structure for analysis. This cleaned table now effectively presents key metrics, including Post URL, Post Date, Engagements, and Impressions, for further examination.

Then we prepared the data for proper chronological analysis. The "Post Date" column was converted into a datetime format to ensure accurate sorting. The data was then sorted by the "Post Date" column, organizing the posts in ascending order based on their publication dates. This step provided a clearer timeline for analyzing the performance of posts over time.

## Challenge

### Why We Could Not Automate LinkedIn Post Caption Extraction

#### LinkedIn’s Privacy & Security Restrictions
 - LinkedIn does not provide public access to post captions via an API unless the user grants explicit developer access.

- Attempting to scrape post captions directly violates LinkedIn’s terms of service, which could lead to account restrictions or bans.

#### Exported Data Does Not Include Captions
 - The LinkedIn data export only includes Post URLs, Impressions, and Engagements, but not the actual text of the posts.

 - Without captions, automated analysis of post content (e.g., keyword extraction) is not possible.

#### Scraping Prevention by LinkedIn
 - LinkedIn has anti-bot protections that block automated data extraction from personal accounts.

 - Even if scraping were attempted, it would require complex browser automation and proxy rotation, which is risky.

### Alternative Approach: Analyzing Top Posts by Post Date
Since captions could not be extracted automatically, we decided to analyze and visualize post performance based on the date they were made.
This approach helps identify trends over time, such as:
 - Which days had the highest engagements
 - How impressions varied over time
 - Patterns in audience interaction

![Engagement and Impression by Post Dates](https://github.com/Phenomkay/LinkedIn-Growth-Analysis/blob/dcc658906dd816ccefdfd10c69c2562aea2eb13b/Engagement%20and%20Impression%20by%20Post%20Dates.png)
