# Chart Selection Justification

| Chart | Business Question | Why Appropriate | Encoding | Design Principle | Mistake Avoided |
|---|---|---|---|---|---|
| Sales Trend Line Chart | How do sales change over time? | Line charts best represent trends | Label: Sales | Temporal continuity | Using bars for long time series |
| Regional Bar Chart | Which regions perform best? | Enables easy ranking | Color: Profit Margin; Label: Sales | Pre-attentive comparison | Pie chart comparison |
| Regional Map | Where are profitable regions located? | Geographic relationships matter | Color: Profit Margin | Spatial encoding | Using non-geographic visuals |
| Category Profitability Bubble/Heat View | Which categories drive profit? | Supports multi-dimensional comparison | Size+Color: Profit Margin | Visual hierarchy | Overcrowded tables |
| Customer Segment Chart | How do customer segments differ? | Facilitates segment comparison | Color: Profit Margin | Group comparison | Excessive dimensions |
| Discount vs Profit Scatter Plot | How do discounts affect profit? | Shows correlation and outliers | Detail: Product | Correlation analysis | Using aggregated averages |
| Return Analysis | Which products/orders are returned? | Highlights exceptions | Color: Return Rate | Exception detection | Hiding low-frequency events |
| Shipping Performance | How efficient is delivery? | Bucketed analysis simplifies interpretation | Color: Delivery Speed | Categorization | Showing raw distributions only |
