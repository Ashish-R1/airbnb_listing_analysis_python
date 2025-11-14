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
    - Brooklyn offers undervalued opportunities with high review rates in certain areas, while Manhattan listings command premium pricing but narrower review distribution.
    - Entire home/apt listings consistently outperform private room listings in both price and occupancy.
    - Long-term hosts enjoy better review volumes and occupancy rates.
- These insights can help optimize pricing strategies, target marketing efforts, and improve host retention.

## Stakeholder Insights & Recommendation

| **Finding** | **Recommendation** |
| --- | --- |
| Manhattan commands higher prices but mid-level review rates. | Target pricing promotions in underperforming Manhattan areas. |
| Brooklyn has lower pricing on average but higher review rates in select neighborhoods. | Prioritize host acquisition and support in emerging Brooklyn districts. |
| High review volume correlates with host tenure (listing age). | Invest in host loyalty programs to boost retention and occupancy. |
| Entire home/apt dominates both bookings and price. | Encourage new hosts to list entire homes for maximal returns. |

## Business-Relevant Questions Answered

- What is the optimal room type to maximize revenue?
- Which neighborhoods present high-growth opportunities for new listings?
- Where do seasonal review surges occur, and how can hosts leverage them?

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

![image alt](https://github.com/Ashish-R1/airbnb_listing_analysis_python/blob/9666c85aa0c444644e6cc4149a80ce93997ba78e/airbnb_images/NeighbourhoodGroup_listing.png)

- **Insight:** Some neighborhoods (e.g., Manhattan, Brooklyn) have far more listings than others, indicating supply concentration.
- **Actionable steps:**
    - Target marketing, onboarding, and support in neighborhoods with less supply but increasing demand (e.g., Queens or Bronx).
    - Use this data for city regulation negotiations or to identify saturation versus growth opportunities
 

## Markets for targeted host onboarding

![image alt](https://github.com/Ashish-R1/airbnb_listing_analysis_python/blob/9666c85aa0c444644e6cc4149a80ce93997ba78e/airbnb_images/Price_NeighbourhoodGroup.png)

- **Insight:** Average listing price varies by neighborhood group, with Manhattan and Brooklyn near the top, but some less obvious groups may have pockets of opportunity.
- **Actionable steps:**
    - Host pricing strategies should be tailored to neighborhood, not just room type.
    - Company could launch promotions or recommend pricing adjustments based on real-time neighborhood trends.

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
  
