# **A/B Testing Evaluation**
***>>> For further details, please refer to AB_Testing_Evaluation.ipynb <<<***
## **1.  Goal**

To determine whether the **Test Campaign outperforms the Control Campaign** across key performance metrics:

- Click-Through Rate (CTR)
- Conversion Rate
- Cost per Click (CPC)
- Cost per Purchase (CPP)
## **2. Results**
- Based on statistical evidence, the Test Campaign does ***not fully outperform*** the Control Campaign across the key business performance metrics.

- The Test campaign shows a **statistically significant increase in CTR**, indicating stronger user engagement.

- However, there is **no statistically significant improvement** in Conversion Rate, CPC, CPP
  
  <img width="574" height="170" alt="image" src="https://github.com/user-attachments/assets/890972ff-4a57-482b-97bb-1df58a74ae83" />


## **3. Method**
- **One-tailed T-test** were conducted to determine whether the observed differences between the Test and Control campaigns are statistically significant.

- **Holm–Bonferroni method** was applied to adjust for multiple hypothesis testing, ensuring that the overall alpha is properly controlled.

## **4. Main Steps**

- **Data Quality Check and Cleaning**: Assessed missing values and removed it.
- **Metric Aggregation**
  - Calculated key performance metrics: CTR, Conversion Rate, CPC, and CPP.
  - Reviewed metric distributions using boxplots.

- **Uplift Analysis**: Calculated percentage uplift between the Test and Control campaigns.

- **Hypothesis Testing**
  - Defined null (H0) and alternative (H1) hypotheses for each metric.
  - Conducted one-tailed t-tests.
  - Applied Holm–Bonferroni correction for multiple comparisons.
  - Determined statistical significance based on the adjusted significance level.
