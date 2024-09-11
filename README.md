# Graduate Student Commute Choice Model

This project models the commute choices of graduate students in town X, focusing on the spring season when driving, biking, and walking are feasible alternatives. The analysis uses a **multinomial logit model** to understand how students choose their commuting mode based on **cost** and **time** factors. 

### Key Components:
1. **Multinomial Logit Model**: We express the **representative utility** for each commuting alternative as a function of cost and time with the equation:
   $$V_{nj} = \alpha_j + \beta C_{nj} + \gamma T_{nj}$$
   where $\alpha_j$ are alternative-specific intercepts, and $\beta$ and $\gamma$ represent the sensitivity to cost and time, respectively.

2. **Parameter Estimation**: We estimated the model parameters using **Maximum Likelihood Estimation (MLE)** with the `minimize()` function from SciPy. This includes calculating **standard errors, z-statistics**, and **p-values** for the coefficients.

3. **Likelihood Ratio Test**: We performed a **likelihood ratio test** to assess the joint significance of alternative-specific intercepts and time coefficients. The test showed that adding these intercepts and coefficients significantly improves the model fit, indicating that commuting choices are influenced by inherent preferences for different modes.

### Results:
- **Cost Sensitivity**: Students are significantly more sensitive to cost than time when choosing a commuting mode, with cost having a larger negative impact on utility.
- **Inherent Preferences**: There are significant positive intercepts for walking and driving, showing inherent preferences for these modes. The bus option, however, has no strong inherent preference.

This project demonstrates the application of MLE, likelihood ratio testing, and logit models in discrete choice analysis.
