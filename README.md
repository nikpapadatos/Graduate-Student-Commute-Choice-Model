# Graduate Student Commute Choice Model

This project models the commute choices of graduate students in town X during the spring season, focusing on alternatives such as driving, biking, and walking. The analysis applies a **multinomial logit model** to examine how students choose a commuting mode based on **cost** and **time** variables.

### Key Components:
1. **Multinomial Logit Model**: The representative utility for each commuting alternative is modeled as a linear function of cost and time:
   $$V_{nj} = \alpha_j + \beta C_{nj} + \gamma T_{nj}$$
   where $\alpha_j$ are alternative-specific intercepts, and $\beta$ and $\gamma$ capture the effects of cost and time on commuting choices.

2. **Parameter Estimation**: Parameters are estimated using **Maximum Likelihood Estimation (MLE)**, with standard errors, z-statistics, and p-values calculated to assess statistical significance.

3. **Likelihood Ratio Test**: A **likelihood ratio test** evaluates the significance of alternative-specific intercepts and time coefficients. Results show that including these terms significantly improves model fit, indicating that different commuting modes have inherent preferences.

### Results:
- **Cost Sensitivity**: The model reveals a higher sensitivity to cost than time, with cost having a stronger negative impact on commuting utility.
- **Inherent Preferences**: Positive intercepts for walking and driving suggest inherent preferences for these modes, while the bus option shows no strong preference.

This project demonstrates the use of MLE and likelihood ratio testing in modeling discrete choice behavior.
