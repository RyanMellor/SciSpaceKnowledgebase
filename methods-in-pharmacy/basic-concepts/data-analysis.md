---
description: >-
  Process of cleaning, transforming, and modelling data to uncover useful
  information
---

# Data Analysis

## Equations

### Coefficient of Determination ($$R^2$$)

Pronounced 'R squared', the coefficient of determination is statistic that gives some information about the goodness of fit of a model.

$$SS_{res} = \sum\limits_i(y_i-f_i)^2$$

$$SS_{tot}=\sum\limits_i(y_i-\bar{y})^2$$

$$R^2=1-\frac{SS_{res}}{SS_{tot}}$$

Where:

* $$SS_{res}$$= Residual sum of squares
* $$SS_{tot}$$= Total sum of squares
* $$\bar{y}$$= Mean of observed data
* $$y_i$$= Each observed datum
* $$f_i$$= Each predicted datum

### Least Squares

Finds optimal parameter values for a function such that $$SS_{res}$$ is minimized.

$$SS_{res} = \sum\limits_i(y_i-f_i)^2$$

Where:

* $$SS_{res}$$= Sum of squares of residuals
* $$y_i$$= Each observed data point
* $$f_i$$= Each predicted data point

In general were no closed form solution exists, optimal parameters are determined by selecting initial parameters which are iteratively refined.

### Linear Regression

An approach to modelling data sets with a linear correlation. Most commonly fitted using the [least squares](data-analysis.md#least-squares) approach. Has a closed form solution.

$$y=a+bx$$

$$b = \frac{\sum(x-\bar x)(y-\bar y)}{\sum(x-\bar x)^2}$$

$$a = \bar y - b\bar x$$

Where:

* $$y$$= The dependent (or outcome) variable
* $$x$$= The independent (or predictor) variable
* $$a$$ = Intercept of the y-axis
* $$b$$ = Slope
* $$\bar y$$= [Mean ](data-analysis.md#mean)of the y data
* $$\bar x$$= [Mean ](data-analysis.md#mean)of the x data

### Mean ($$\mu$$)

$$\mu= \frac{\sum\limits_{i=1}^n x_i}{n}$$

* $$x_i$$ = Each data point
* $$n$$ = Number of data points

### Relative Standard Deviation ($$\%RSD$$)

A standardized measure of dispersion. It is used to quantify [precision](validation.md#precision-repeatability).

Closely related to the coefficient of variation (CV)

$$\%RSD=100\frac{\sigma}{\mu}$$

Where:

* $$\sigma$$ = [Standard deviation](data-analysis.md#standard-deviation)
* $$\mu$$ = [Mean ](data-analysis.md#mean)of data

### Standard deviation ($$\sigma$$)

A measure of dispersion.

$$\sigma = \sqrt{\frac{\sum\limits_{i=1}^n (x_i-\bar{x})^2}{n-1}}$$

Where:

* $$\bar{x}$$ = [Mean ](data-analysis.md#mean)of data
* $$x_i$$ = Each data point
* $$n$$ = Number of data points

### Standard error of the predicted y-value ($$S_{y,x}$$)

$$S_{y,x} = \sqrt{\frac{1}{n-2}\left(\sum(y-\bar y)^2-\frac{(\sum (x-\bar x)(y-\bar y))^2}{\sum (x-\bar x)^2}\right)}$$

Where:

* $$x$$ = [Mean ](data-analysis.md#mean)of x data
* $$\bar x$$ = Observed x data
* $$y$$ = Observed y data
* $$\bar y$$ = Forecast y data

### Variance

$$Variance = \sigma^2 = \frac{\sum\limits_{i=1}^n (x_i-\bar{x})^2}{n-1}$$

Where:

* $$\sigma$$= [Standard deviation](data-analysis.md#standard-deviation)
* $$\bar{x}$$ = [Mean ](data-analysis.md#mean)of data
* $$x_i$$ = Each data point
* $$n$$ = Number of data points

## Models

For all models:

* $$y$$= The dependent (or outcome) variable
* $$x$$= The independent (or predictor) variable
* $$y_0$$May be added to and model to offset in the y-axis

### Linear

$$y=a+bx$$

Where:

* $$a$$ = Intercept of the y-axis
* $$b$$ = Slope

![](<../../.gitbook/assets/model - linear (1).png>)

### Polynomials

$$y=a+bx+cx^2...+ix^n$$

Where:

* $$a$$ = Intercept of the y-axis
* $$b,c...i$$ = Coefficients, no definition
* $$n$$= Order of the polynomial

Named polynomials:

* Order = 1: [Linear](data-analysis.md#linear)
* Order = 2: Quadratic
* Order = 3: Cubic

![Polynomials of order 2, 3, 4, and 5](<../../.gitbook/assets/model - polynomials.png>)

### Exponential

$$y=ae^{kx}$$

Where:

* $$a$$ = Intercept of the y-axis
* $$k$$ = Relative increase/decrease of $$y$$ with respect to $$x$$

![](<../../.gitbook/assets/model - exp (1).png>)

### Limited Exponential

$$y=ae^{bx}+c$$

Where:

* $$a$$ = Intercept of the y-axis (offset by $$c$$)
* $$b$$ = Relative increase/decrease of $$y$$ with respect to $$x$$
* $$c$$ =  Plateau

![](<../../.gitbook/assets/model - limited exp.png>)

### Double Exponential

$$y=ae^{bx}+ce^{dx}$$

Where:

* $$a$$ =&#x20;
* $$b$$ =
* $$c$$ =
* $$d$$ =

![](<../../.gitbook/assets/model - double exp.png>)

### Power

$$y=x^a$$

Where:

* $$a$$ = Power

![](<../../.gitbook/assets/model - power (1).png>)

### Logarithmic

$$y=a\ ln(x)$$

Where:

* $$a$$ = Scalar

![](<../../.gitbook/assets/model - log (1).png>)

### Log Normal

$$y=\frac{a}{\sqrt{2\pi}cx}e^{\frac{-\left(ln\frac{x}{b}\right)^2}{2c^2}}$$

Where:

* $$a$$ = Area
* $$b$$ = Center
* $$c$$ = Log standard deviation

![](<../../.gitbook/assets/model - log normal.png>)

### Michaelis Menten

$$y = \frac{V_{max}x}{K_m+x}$$

Where:

* $$V_{max}$$= Maximum
* $$K_m$$= Michaelis constant

![](<../../.gitbook/assets/model - Michaelis Menten.png>)

### Logistic

$$y = a + \frac{b-a}{1 + e^{-d(x-c)}}$$

Where:

* $$a$$= Minimum
* $$b$$= Maximum
* $$c$$= Inflection
* $$d$$= Growth rate

![](<../../.gitbook/assets/model - logistic (1).png>)

### Gaussian

$$y=ae^{\frac{(x-b)^2}{2c^2}}$$

Where:

* $$a$$= Amplitude
* $$b$$= Position
* $$c$$= Width

![](<../../.gitbook/assets/model - Gaussian.png>)

### Lorentz

$$y=\frac{2ac}{4\pi (x-b)^2+c^2}$$

Where:

* $$a$$= Amplitude
* $$b$$= Position
* $$c$$= Width

![](<../../.gitbook/assets/model - Lorentz.png>)

[Which model should I use?](https://xkcd.com/2048/)

## Excel

### Formulas

#### Basics

* Sum
  * `=sum(range)`
  * `=sumif(range, condition)`
* Product
  * `=product(range)`
* Remainder from division
  * `=mod(number)`
* Power
  * `=power(number, exponent)`
* Square root
  * `=sqrt(number)`
* Count the number of cells containing numbers
  * `=count(range)`
  * `=countif(range, condition)`
* Random
  * `=rand()`
  * `=randbetween(lower bound, upper bound)`
* Round
  * `=round(number, decimal places)`
  * `=roundup(number, decimal places)`
  * `=rounddown(number, decimal places)`
  * `=mround(number, multiple)`
  * `=ceiling(number, multiple)`
  * `=floor(number, multiple)`
  * `=even(number)`
  * `=odd(number)`
  * `=int(number)`
* Logic
  * `=if(condition, value if true, value if false`
  * `=and(condition 1, condition 2)`
  * `=or(condition 1, condition 2)`
* Date
  * `=today()`
* Date and time
  * `=now()`

#### Linear regression

* [Slope](data-analysis.md#linear-regression)
  * `=slope(y-values, x-values)`
* [Intercept](data-analysis.md#linear-regression)
  * `=intercept(y-values, x-values)`
* Forecast for a given x
  * `=forecast(x, y-values, x-values)`
* [Coefficient of determination](data-analysis.md#coefficient-of-determination)
  * `=rsq(y-values, x-values)`
* [Standard error of the predicted y-value](data-analysis.md#standard-error-of-the-predicted-y-value)
  * `=steyx(y-values, x-values)`

#### Statistics

* [Mean](data-analysis.md#mean)
  * `=average(range)`
  * `=averageif(range, condition)`
* Median
  * `=median(range)`
* Mode
  * `=mode(range)`
* Smallest and largest in range
  * `=min(range)`
  * `=max(range)`
* $$N^{th}$$ smallest and largest in range
  * `=small(range, n)`
  * `=large(range, n)`
* Weighted average of two ranges
  * `=sumproduct(range 1, range 2)`
* [Standard Deviation](data-analysis.md#standard-deviation)
  * `=stdev(range)`
* [Relative standard deviation](data-analysis.md#relative-standard-deviation)
  * `=100 * stdev(range)/average(range)`

#### Miscellaneous

* Pi ($$\pi$$) to 15 decimal places
  * `=pi()`
* Index/match. Looks up a given value in a range and returns corresponding value from the equivalent location in a second range
  * `=index(return range, match(lookup value, lookup range, match type))`
  * match type = \[-1:less than, 0:exact, 1:greater than]

### Features

#### Solver

Used to find optimal parameters for fitting a model to a data set.

To activate: File > Options > Add-ins > Go > Solver Add-in > OK > Data tab

* Set up sheet as below
  * x = Independent variables
  * y = Observed dependent data
  * f = Predicted dependent data, should contain the formula for the relevant [model](data-analysis.md#models)
  * $$S_{res}$$= Squares of residuals
  * $$SS_{res}$$= Sum of squares of residuals
  * Parameters = Parameters for the relevant [model](data-analysis.md#models)
* Set up solver as below
  * Set objective: $$SS_{res}$$
  * To: 'Min'
  * By changing variable cells: Parameters

| x       | y       | f       | $$S_{res}$$     | $$SS_{res}$$                   | Parameters |
| ------- | ------- | ------- | --------------- | ------------------------------ | ---------- |
| $$x_1$$ | $$y_1$$ | $$f_1$$ | $$(y_1-f_1)^2$$ | $$\sum\limits_i^n(y_i-f_i)^2$$ | $$P_1$$    |
| ...     | ...     | ...     | ...             |                                | ...        |
| ...     | ...     | ...     | ...             |                                | $$P_n$$    |
| $$x_n$$ | $$y_n$$ | $$f_n$$ | $$(y_n-f_n)^2$$ |                                |            |

