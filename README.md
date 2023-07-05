# ecommerce-ltv-prediction

### Introduction:

Understanding the Customer Lifetime Value (CLV), the total net profit a company can expect to generate from a customer,
can be measured with a reasonable degree of precision. By predicting the CLV, business-owners and stakeholders can gain insights into customer behavior and make informed decisions regarding customer acquisition and retention.

### Aim:
To develop a model that can:

• Distinguish active customers from inactive customers.
• Generate transaction forecasts for individual customers.
• Predict the purchase volume of the entire customer base.

### Methods:
• RFM Matrix: Recency, Frequency, Monetary value matrix based on the transaction log.
• Define a calibration and holdout period to split data.
• Training model: Modified Beta Geometric/Negative Binomial Distribution (MBG/NBD) model using the lifetimes package. It fits the model to the columns of the feature set.
• Using Gamma Gamma model, estimate the CLV (calculates predicted purchases for each customer and assigns a probability of being alive based on the MBG/NBD model).

