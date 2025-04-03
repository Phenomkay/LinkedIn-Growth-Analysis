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


### Discovery Table
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


### Engagement Table
From the engagement table, we did the following analysis

**Date Conversion**: The Date column in the engagement table (df_eng) is converted into a datetime format, enabling advanced time-based operations.

**Monthly Aggregation**: The engagement data is grouped by months using the .dt.to_period("M") function. This groups all rows from the same month and sums up numeric columns (like Impressions and Engagements).

**Formatting for Plotting**: The resulting monthly data's index (representing months) is converted into strings, making it easier to use for plotting or further analysis.

**Output**: The df_monthly table contains aggregated monthly totals for numeric columns (e.g., total Impressions and Engagements), offering a clear view of trends over time.

This summarized table reveals how engagement metrics (impressions and engagements) have evolved month by month, which is useful for identifying trends or seasonal patterns in LinkedIn activity.

Furthermore, the sum of all impressions is 10,839, indicating the total visibility of LinkedIn posts, while the sum of all engagements is 261, reflecting the overall audience interactions (likes, comments, shares, etc.) within the specified timeframe. This provides a snapshot of LinkedIn performance metrics.


![Monthly Impression Trend](https://github.com/Phenomkay/LinkedIn-Growth-Analysis/blob/353c2b3885b1ca83604a4206b9294efc0b947887/Monthly%20Impression%20trend.png)
