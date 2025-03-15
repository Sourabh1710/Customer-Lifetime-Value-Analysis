# Customer Lifetime Value (CLV) Analysis

## Overview
Customer Lifetime Value (CLV) analysis is used to estimate the total value of customers to the business over the lifetime of their relationship. It helps companies determine how much to invest in customer acquisition and retention, as well as identify the most valuable customers to prioritize for retention efforts.

By analyzing customer lifetime value, I can identify the most effective marketing channels and campaigns for acquiring high-value customers, as well as develop targeted retention strategies to keep those customers engaged and loyal.

---

## Dataset
The [dataset](https://statso.io/customer-lifetime-value-analytics-case-study/) used in this project consists of customer acquisition data with the following attributes:

- **customer_id**: Unique identifier for each customer
- **channel**: Acquisition channel (e.g., referral, paid advertising, email marketing, social media)
- **cost**: Cost of acquiring the customer
- **conversion_rate**: Probability of converting the acquired customer
- **revenue**: Revenue generated from the customer

### Sample Data:
```python
import pandas as pd
import plotly.graph_objs as go
import plotly.express as px
import plotly.io as pio
pio.templates.default = "plotly_white"

data = pd.read_csv("customer_acquisition_data.csv")
print(data.head())
```

```
   customer_id           channel       cost  conversion_rate  revenue
0            1          referral   8.320327         0.123145     4199
1            2  paid advertising  30.450327         0.016341     3410
2            3   email marketing   5.246263         0.043822     3164
3            4      social media   9.546326         0.167592     1520
4            5          referral   8.320327         0.123145     2419
```

---

## Data Visualization
### 1. Distribution of Acquisition Cost and Revenue
#### Acquisition Cost Distribution:
![Acquisition Cost Distribution](https://github.com/Sourabh1710/Customer-Lifetime-Value-Analysis/blob/main/images/Distribution%20of%20Acquisition%20Cost.png)

#### Revenue Distribution:
![Revenue Distribution](https://github.com/Sourabh1710/Customer-Lifetime-Value-Analysis/blob/main/images/Distribution%20of%20Revenue.png)

### 2. Acquisition Cost by Channel
![Acquisition Cost by Channel](https://github.com/Sourabh1710/Customer-Lifetime-Value-Analysis/blob/main/images/Customer%20Acquisition%20Cost%20by%20Channel.png)

- **Paid advertising** is the most expensive acquisition channel.
- **Email marketing** is the least expensive channel.

### 3. Conversion Rate by Channel
![Conversion Rate by Channel](https://github.com/Sourabh1710/Customer-Lifetime-Value-Analysis/blob/main/images/Conversion%20Rate%20by%20Channel.png)

- **Social Media** is the most effective channel for converting customers.
- **Paid advertising** is the least effective channel.

### 4. Total Revenue by Channel
![Total Revenue by Channel](https://github.com/Sourabh1710/Customer-Lifetime-Value-Analysis/blob/main/images/Total%20Revenue%20by%20Channel.png)

- **Email marketing** generates the highest revenue.
- However, there is no significant difference between revenue contributions of all channels.

### 5. Return on Investment (ROI) by Channel
![ROI by Channel](https://github.com/Sourabh1710/Customer-Lifetime-Value-Analysis/blob/main/images/Return%20on%20Investment%20(ROI)%20by%20Channel.png)

- **Email marketing** has the highest ROI.
- **Paid advertising** has the lowest ROI.

### 6. Customer Lifetime Value (CLV) Calculation
#### Formula:
```
CLTV = (revenue - cost) * conversion_rate / cost
```

![CLTV Calculation](https://github.com/Sourabh1710/Customer-Lifetime-Value-Analysis/blob/main/images/Customer%20Lifetime%20Value%20by%20Channel.png)

- **Social Media** and **Referral** channels have the highest CLV.

### 7. CLTV Comparison: Social Media vs. Referral
![CLTV Comparison](https://github.com/Sourabh1710/Customer-Lifetime-Value-Analysis/blob/main/images/CLTV%20Distribution%20by%20Channel.png)

- The difference is minimal, but **Social Media** has a slightly higher CLTV than Referral.

---

## Summary
Customer lifetime value analysis is used to estimate the total value of customers to the business over the lifetime of their relationship. It helps companies determine how much to invest in customer acquisition and retention, as well as identify the most valuable customers to prioritize for retention efforts.

---

## Author
Sourabh Sonker <br>
Data Scientist
