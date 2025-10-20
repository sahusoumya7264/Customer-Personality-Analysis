# Customer-Personality-Analysis
Customer personality analysis helps a business to modify its product based on its target customers from different types of customer segments.
# Analysis
- Data Size and Structure: The dataset contains 2240 rows and 29 columns, including a mix of numerical and categorical data.
- Missing Values: Only the 'Income' column initially had missing values (24), which we filled using the mean of the existing values. The 'Dt_Customer' column also had issues with format and missing values after conversion, which we addressed.
- Duplicate Values: There are no duplicate rows in the dataset.
- Date Format: The 'Dt_Customer' column had inconsistent date formats, which we standardized to datetime objects and then formatted to 'dd-mm-yyyy'.
- Constant Value Columns: The 'Z_CostContact' and 'Z_Revenue' columns have constant values and were dropped as they do not provide useful information for correlation or variance-based analysis.
- Correlations: From the correlation matrix of the numeric columns, we can observe relationships between variables. For example, 'Income' shows strong positive correlations with spending on various products ('MntWines', 'MntFruits', 'MntMeatProducts', etc.) and with purchase channels ('NumCatalogPurchases', 'NumStorePurchases'). 'Kidhome' and 'Teenhome' show negative correlations with spending, suggesting that households with children (especially younger ones) tend to spend less on these products. There are also correlations among the different marketing campaign acceptance columns.
