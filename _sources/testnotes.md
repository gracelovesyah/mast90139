# Tests
## Q1 (Model with Ungroped Data)
### Goodness of fit of a Model?
1. if anova table provided, then, yes, we can conclude whether a model is adequate. 
2. if no anova, only know residual deviance. Then no, we can't conclude anything. The reason for not using residual deviance to infer model's goodness of fit is explained in <a href="https://canvas.lms.unimelb.edu.au/courses/151965/discussion_topics/962186" target="_blank">Canvas Discussion Topic</a>
### Covariance?
1. odds ratio (if 2 var are changing): 
```{math}
e^{\beta_1 + \beta_2}
```
2. 95% CI of odds ratio 
```{math}
e^{\beta_1 + \beta_2 +- 1.96 * co-std}
```
to calculate co-std: firstly calculate covariance
$$co\-std = \sqrt{cov}$$
way 1:
$cov = [x x x x][c][x x x x]^T$

way 2:
$cov = \sqrt{std1^2 + std2^2 + cov(std1, std2)}$
## Q2 (Model with Grouped Data)
### Can't predict probability of individual?
Although model allow us to estimate the odds ratio accurately, it is not able to accurately predict the probability of xxx for an individual from his/her xxx. Explain why.

> xxx model is a logistic regression model for grouped data. Variations are into groups. Hence, inaccurate predictions for individuals. 