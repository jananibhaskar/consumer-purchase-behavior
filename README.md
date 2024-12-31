# Consumer-purchase-behavior
This project uses **Weka** to explore various data mining techniques and derive valuable insights to address a business challenge.
## Dataset: 
[Link to the Dataset](https://www.kaggle.com/code/waqi786/electronic-sales-insights-sep-2023-sep-2024/notebook)
20,000 records. Sales data covers a wide range of products (smartphones, tablets, laptops, etc.)
## Project Objectives
- Analyze customer purchasing patterns
- Identify high-selling products across categories (smartphones, laptops, tablets)
- Examine seasonal trends such as holiday sales
- Explore customer demographics and preferences
- Optimize cross-sales strategies by identifying products frequently purchased together
- Improve inventory management by predicting demand.
## Cleaning and preprocessing Dataset
- Missing Value Handling:Only the “Add-Ons Purchased” attribute had missing values (24% or 4868 instances).
Replaced blank entries with "0" to avoid negative impact on results.
- Normalize Data:Scaling "Total Price" and "Quantity" to fall within a consistent range (e.g., 0-1) for use in K-Means or regression models.
- KMeans - NominalToBinary,Linear Regression - NominaltoBinary,Apriori - NumerictoNominal
## Models Used
**Classification**
- J48 Decision Tree: Identify products driving customer loyalty.
- Random Forest: Classify completed vs. canceled orders.
**Regression**
- Linear Regression: Predict future sales trends.
**Clustering**
- K-Means Clustering: Segment customers based on demographic and purchase patterns.
**Associate** 
- Apriori: Discover cross-selling opportunities.
## Conclusion
- J48 Decision Tree: Smartphone are strongly associated with customer loyalty, suggesting that targeted promotions for smartphones and tablets could enhance member retention.
- Linear Regression: 93.31% of Canceled orders were correctly classified.
- Random Forest: RF effectively distinguished between Canceled and Completed orders, demonstrating high accuracy and reliability in its classifications.The model provides valuable insights into customer behavior and order patterns.
- Association Rule Mining:Suggest bundling headphones with smartphones to increase sales.![image](https://github.com/user-attachments/assets/81a25836-5952-415c-ae1c-1907b2ae4dc3)
## Acknowledgments
- Dataset sourced from [Kaggle](https://www.kaggle.com).
- Weka: [Official Website](https://www.cs.waikato.ac.nz/ml/weka/).
