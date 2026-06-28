# Business Insights

## Required Calculated Fields

| Calculated Field | Tableau Formula | Business Purpose |
|---|---|---|
| Profit Margin | `([Profit]/[Sales])*100` | Measure profitability efficiency |
| Cost | `[Sales]-[Profit]` | Estimate cost base |
| Average Order Value | `SUM([Sales])/COUNT([Order Id])` | Track customer spending |
| Return Rate | `AVG([Return Flag])*100` | Monitor product/service quality |
| Shipping Delay Bucket | `IF [Delivery Days]<=2 THEN "Fast" ELSEIF [Delivery Days]<=5 THEN "Standard" ELSE "Delayed" END` | Segment delivery performance |

## Business Insights

1. **Sales Trend**  
- Observation: Dashboard includes a dedicated sales trend analysis.  
- Data evidence: Time-series view based on Order Date and Sales.  
- Business interpretation: Revenue seasonality and growth patterns can be identified.  
- Recommended action: Analyze peak and low-performing periods for demand planning.

2. **Regional Performance**  
- Observation: Regional profitability varies significantly.  
- Data evidence: Regional bar chart and geographic map colored by Profit Margin.  
- Business interpretation: Certain regions generate sales but not profits.  
- Recommended action: Review pricing and operating costs by region.

3. **Category Profitability**  
- Observation: Sub-category profit margins are uneven.  
- Data evidence: Category profitability visualization uses Profit Margin for color and size.  
- Business interpretation: Some categories drive revenue while eroding margins.  
- Recommended action: Optimize portfolio and discontinue low-margin products.

4. **Customer Segment Behavior**  
- Observation: Customer segments contribute differently to revenue and profitability.  
- Data evidence: Customer segment chart uses Sales and Profit Margin.  
- Business interpretation: High-revenue customers may not be most profitable.  
- Recommended action: Develop segment-specific strategies.

5. **Discount Impact**  
- Observation: Discounting appears associated with profit variation.  
- Data evidence: Discount vs Profit analysis at product level.  
- Business interpretation: Excessive discounting may reduce profitability.  
- Recommended action: Define discount thresholds.

6. **Shipping Performance**  
- Observation: Delivery performance varies across orders.  
- Data evidence: Delivery Days grouped into speed buckets.  
- Business interpretation: Delayed shipping may impact customer satisfaction.  
- Recommended action: Review logistics partners and service levels.

7. **Return Pattern**  
- Observation: Returns are measurable across products/orders.  
- Data evidence: Return analysis and Return Rate KPI.  
- Business interpretation: Product quality or expectation gaps may exist.  
- Recommended action: Investigate high-return categories.

8. **Business Risk/Opportunity**  
- Observation: Profitability concentration risk may exist across regions/categories.  
- Data evidence: Combined profitability dashboards and KPI cards.  
- Business interpretation: Overdependence on a few profitable segments increases risk.  
- Recommended action: Diversify growth investments and perform cohort analysis.
