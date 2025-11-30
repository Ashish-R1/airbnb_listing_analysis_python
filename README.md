# **airbnb_listing_analysis_python**

## Client Background: Airbnb

Airbnb is a leading global platform connecting travelers with hosts offering unique short-term accommodations. Operating in over 220 countries, Airbnb uses technology and data analytics to match guests with spaces, optimize pricing, and foster trust.

## Project Context

### **Business Objective:**

Unlock key business drivers for Airbnb stakeholders in NYC.
- **For property owners:** Pinpoint the most profitable room types and neighborhoods.
- **For Airbnb strategy teams:** Identify regions with supply/demand imbalance or pricing inefficiencies.
- **For investors:** Evaluate micro-market trends to guide investment decisions.

## Executive Summary

- The analysis covers over 100,000 active Airbnb listings spanning all major NYC neighborhoods.
- **Key discoveries:**
    - Median listing price: $625 (range: $50–$1200).
    - Manhattan and Brooklyn show the highest supply concentration (based on countplot generation).
    - Entire home/apt commands the highest revenue potential.
    - Long-term hosts enjoy better review volumes and occupancy rates.
- These insights can help optimize pricing strategies, target marketing efforts, and improve host retention.

## Stakeholder Insights & Recommendation

| **Finding** (Derived Insight) | **Supporting Metric** | **Recommendation** |
| --- | --- | --- |
| Queens leads the market in listing price | **Avg Price: $629.98** | Neighborhood-based premium pricing benchmarking for hosts |
| Bronx shows comparable high pricing tiers | **Avg Price: $627.63** | Expand listings while competition is still moderate |
| Brooklyn remains a strong priced supply hub | **Avg Price: $626.48** | Assist hosts in optimizing listings instead of price cuts |
| Staten Island listings price below top 3, but strong guest rating | **Avg Price: $623.31**, **Review Rate: 3.40** | Use guest satisfaction to drive visibility & bookings |
| Manhattan price below top boroughs but still competitive | **Avg Price: $622.82**, **Review Rate: 3.27** | Apply targeted incentives only in low-engagement zones |
| Entire home/apt outperforms other room categories | **Highest price tier in room-type box & comparison plots** | Guide new qualified hosts → entire home listings |

## Business-Relevant Questions Answered

- What is the optimal room type to maximize revenue?
- Which neighborhoods present high-growth opportunities for new listings?
- Are pricing clusters/outliers present?

## Pricing clusters and outlier zones.

  ![image alt](https://github.com/Ashish-R1/airbnb_listing_analysis_python/blob/9666c85aa0c444644e6cc4149a80ce93997ba78e/airbnb_images/DistributionOfListingPrice.png)

- **Insight:** Airbnb listing prices in NYC span a wide range, with most clustered in the lower and mid-price tiers, but several listings reach very high prices.
- **Actionable steps:**
    - Hosts should benchmark their prices against the median and 75th percentile to remain competitive.
    - Stakeholders can identify luxury vs. budget segments for targeted campaigns or product enhancements.

## 'Entire home/apt' outperforms by revenue

 ![image alt](https://github.com/Ashish-R1/airbnb_listing_analysis_python/blob/9666c85aa0c444644e6cc4149a80ce93997ba78e/airbnb_images/Price_roomType.png)

- **Insight:** "Entire home/apartment" listings command significantly higher prices than "Private rooms" or other room types.
- **Actionable steps:**
    - Encourage new hosts to list entire homes if maximizing revenue is a priority.
    - For investors, focus resource allocation on properties suited to entire home/apartment listings.
 

## Demand hotspots and opportunities.

![image alt](https://github.com/Ashish-R1/airbnb_listing_analysis_python/blob/3603d7e56bf2824d71fa27a0a16bcebc6ffd6abb/airbnb_images/NeighbourhoodGroup_listing1.png)

- **Insight:** Manhattan and Brooklyn have the highest number of listings, indicating supply concentration and potentially greater competition. Queens, Bronx, and Staten Island represent underserved markets.

- **Actionable steps:**
    - Targeted host onboarding drives in Queens/Bronx/Staten Island to grow supply where competition is lower.
    - Provide supply balancing guidance in oversaturated boroughs like Manhattan.
    - Promote regional marketing campaigns tailored to emerging boroughs with growth headroom.

## Markets for targeted host onboarding

![image alt](https://github.com/Ashish-R1/airbnb_listing_analysis_python/blob/3603d7e56bf2824d71fa27a0a16bcebc6ffd6abb/airbnb_images/Price_NeighbourhoodGroup1.png)

- **Insight:** Queens commands the highest average price, followed closely by Bronx and Brooklyn. Manhattan is priced lower than expected—indicating possible price inefficiencies or stronger competition.

- **Actionable steps:**
    - Optimize pricing algorithms to reflect **true borough-level revenue potential**.
    - Encourage hosts in Queens and Bronx to maintain **premium positioning** with amenities/quality.
    - Recommend Manhattan hosts use **dynamic pricing** or seasonal promotions to boost engagement.

![image alt](https://github.com/Ashish-R1/airbnb_listing_analysis_python/blob/3603d7e56bf2824d71fa27a0a16bcebc6ffd6abb/airbnb_images/Reviews_over_time1.png)

**Insight:** Review activity varies noticeably over time, indicating seasonal demand cycles. Peaks likely align with travel seasons or holiday periods; dips reflect off-season lulls.

**Actionable steps:**
    - Implement seasonal pricing strategies —higher during peak tourism periods.
    - Encourage hosts to offer discounts during slow months to maintain occupancy.
    - Airbnb can use seasonality trends to schedule marketing boosts and host performance reminders.


## Analysis Approach

- **Data Cleaning:**
    - Handled missing, malformed, or outlier records (e.g., removed listings with unverified hosts, dropped redundant columns like Licence / House rules).
    - Converted prices, service fees from string formats to floats.
    - Filled missing reviews with sensible defaults, ensuring robust time series analysis.
- **Exploratory Analysis:**
    - Descriptive statistics for numeric drivers.
    - Distribution and correlation analysis for price, review count, room type, zip/neighborhood.
- **Visual Storytelling:**
    - Used clear histograms, boxplots, and scatterplots with top-line takeaways.
    - Each plot is paired with written business impact.
 
## Key Takeaways

**What could a stakeholder or manager do today, based on this analysis?**

- Rebalance marketing spend to underserved, high-opportunity neighborhoods.
- Benchmark listing price versus local median to spot competitive gaps.
- Launch retention strategies for long-standing hosts.
- Guide new hosts toward higher-demand property types.

## Next Steps

*For further business impact, I would:*

- Merge property occupancy data and external tourism demand signals for richer forecasting.
- Model host churn and retention predictors over time.
- Add seasonality and city regulation overlays to anticipate market shocks.
  
