Chapter 03. Linear Regression
================

  - using `Advertising` data with `sales` for a particular product as a
    function of advertising budgets on `TV`, `radio`, and `newspaper`
      - ask the following questions:
          - Is there a relationship between advertising budget and
            sales?
          - How strong is the relationship?
          - Which advertising media contribute to sales?
          - How accurately can we estimate these effects?
          - How accurately can we predict future sales?
          - Is the relationship linear?
          - Is there synergy among advertising media?

## 3.1 Simple Linear Regression

  - a straightforward approach for predicting a quantitative response
    \(Y\) on the basis of a single predictor variable \(X\)
      - *regressing \(Y\) on \(X\)*

\(Y \approx \beta_0 + \beta_1X\)

### 3.1.1 Estimating the Coefficients

  - in practice \(\beta_0\) and \(\beta_1\) are unknown
  - the data is in \(n\) \(x\) and \(y\) pairs:
    \((x_1, y_1), (x_2, y_2), ..., (x_n, y_n)\)
  - want to find values for \(\beta_0\) and \(\beta_1\) such that the
    line is as close as possible to these points
      - measure “closeness” using *least squares* criterion
  - if \(\hat{y}_i = \hat{\beta}_0 + \hat{\beta}_1 x_i\), then the
    \*residual is \(e_i = y_i - \hat{y}_i\)
      - then the *residual sum of squares* is
        \(\text{RSS} = e_1^2 + e_2^2 + ... + e_n^2 = \sum_i^n e_i^2\)
      - can find solutions to minimize the RSS using a bit of calculus
