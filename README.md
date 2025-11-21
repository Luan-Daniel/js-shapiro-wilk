# Js-Shapiro-Wilk

This project provides a JavaScript implementation of the **Shapiro-Wilk normality test**, ported from R. The Shapiro-Wilk test is one of the most powerful statistical tests for assessing whether a dataset is normally distributed.

It evaluates the null hypothesis that a sample $x_1, x_2, \dots, x_n$ comes from a normally distributed population.
- **Test statistic $W$:**  
  The Shapiro-Wilk statistic $W$ measures how well the data fits a normal distribution.  
  - Values of $W$ close to $1$ indicate the data is approximately normal.  
  - Smaller values of $W$ suggest deviations from normality.

- **p-value:**  
  The p-value helps interpret the result:  
  - If $p > 0.05$, we fail to reject the null hypothesis → the data is consistent with normality.  
  - If $p ≤ 0.05$, we reject the null hypothesis → the data is not normally distributed.

Note: Like all statistical tests, the Shapiro-Wilk test is sensitive to sample size. Very large samples may detect trivial deviations, while very small samples may lack power.

The main functions are:

### 1. `ShapiroWilk(data)`
This is the **core function** that computes the Shapiro-Wilk test.

### 2. `SHAPIROTEST(cell_range)`
This is a **wrapper function** for Google AppScript. Let you apply this test in Google Sheets ranges.
