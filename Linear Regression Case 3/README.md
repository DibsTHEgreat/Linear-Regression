# Linear-Regression Case 3: SAT Score & Rand 1, 2, 3 vs. GPA Prediction

## Overview
This repository contains experiments with Linear Regression through a couple of case studies using practice datasets.

### Objective
The goal of this analysis is to investigate the change in the relationship between a student's SAT score and GPA score by introducing a new random variable which will label each student 1, 2, 3. There is an assumption that this new variable will not positively impact the model, since Rand 1, 2, 3 has no way of predicting the college GPA. The goal is to observe the Adjusted R-Square, and see the change from Case 1 and Case 3.

### Methodology
I performed a linear regression analysis on the dataset to understand the correlation between SAT scores, Rand 1, 2, 3 and subsequent university GPAs.

### Results
I observed that somehow the R-Square value went up from 0.406 to 0.407, however, I was penalized for adding an additional variable since my adjusted R-Sqaure value went down; from 0.399 to 0.392. Additionally, we can see in the coefficient table that the constant for Rand 1, 2, 3 is in the negatives (-0.0083), and the P value is 0.762. Thus we cannot reject the null hypothesis at the 76% level. (P-value < 0.05 is good)

### Conclusion
Based on the analysis, it can be concluded that we lost value from our model since we added a variable that did not help the model gain a better fit of the data. Not only did it worsen the explanatory power of the model but is also insignificant, therefore, it is in the best interest of the model to drop the variable: Rand 1, 2, 3.