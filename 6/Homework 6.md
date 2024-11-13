___
## Theorem of Calculus, Density and Cumulative Distribution Functions

### The Fundamental Theorem of Calculus
The **Fundamental Theorem of Calculus (FTC)** serves as a bridge between differentiation and integration, providing an essential foundation for understanding the connection between density functions and cumulative distribution functions (CDFs) in probability.

The FTC is comprised of two primary parts:

###### 1

For a continuous, real-valued function $f$ over an interval $[a, b]$, if $F(x)$ is defined as:

$$
F(x) = \int_{a}^{x} f(t) \, dt
$$

then $F$ is continuous over $[a, b]$, differentiable within $(a, b)$, and satisfies:

$$
F'(x) = f(x).
$$

In simpler terms, the derivative of the integral of $f$ from $a$ to $x$ yields the original function $f(x)$.

###### 2

For an antiderivative $F$ of $f$ over $[a, b]$, where $F'(x) = f(x)$, we have:

$$
\int_{a}^{b} f(x) \, dx = F(b) - F(a).
$$

### Connection to Density and Cumulative Distribution Functions

In probability, two closely related concepts often arise:

- **Probability Density Function (PDF)**: for a continuous random variable $X$, the PDF $f(x)$ indicates the probability density at a specific point $x$.
- **Cumulative Distribution Function (CDF)**: the CDF $F(x)$ represents the probability that $X$ is less than or equal to $x$:  
  $$
  F(x) = P(X \leq x) = \int_{-\infty}^{x} f(t) \, dt.
  $$

The CDF $F(x)$ can be viewed as the integral of the PDF $f(x)$ from $-\infty$ to $x$.
If we define $F(x)$ as:

$$
F(x) = \int_{-\infty}^{x} f(t) \, dt,
$$

then $F$ is differentiable, with its derivative equal to the PDF $f(x)$. Therefore:

$$
F'(x) = f(x).
$$

This illustrates that the PDF $f(x)$ is the derivative of the CDF $F(x)$. This core relationship enables us to transition between the PDF and CDF representations in probability:

1. **From PDF to CDF**: integrate the PDF over $(-\infty, x]$:  
   $$
   F(x) = \int_{-\infty}^{x} f(t) \, dt.
   $$
   
2. **From CDF to PDF**: differentiate the CDF with respect to $x$:  
   $$
   f(x) = \frac{d}{dx} F(x).
   $$

## Comparison of Empirical and Theoretical Mean and Variance

The empirical mean and variance, calculated from sample data, serve as practical estimations of the theoretical mean and variance. They help describe sample traits and facilitate population-level inferences. Here are the differences:

1. **Empirical vs. Theoretical Mean**
   - **Theoretical Mean**: For uniformly distributed random values between 0 and 1, the theoretical mean is 0.5, since every value in this range has equal likelihood.
   - **Empirical Mean**: The empirical mean of generated random values approaches the theoretical 0.5 with large sample sizes. In smaller samples, however, random fluctuations often cause the empirical mean to deviate from the theoretical mean.

2. **Empirical vs. Theoretical Variance**
   - **Theoretical Variance**: For a uniform distribution on $[0,1]$, the theoretical variance is 0.0833 due to the even spread around a mean of 0.5.
   - **Empirical Variance**: As sample size grows, the calculated variance converges to 0.0833. Smaller samples may show significant variance deviations from the theoretical value due to random sample fluctuations.

### Impact of Sample Size

With larger samples, both the empirical mean and variance tend to align with their theoretical values, as predicted by the law of large numbers. In effect, greater sample sizes bring empirical values closer to theoretical expectations:

- **Mean**: Tends toward 0.5 with reduced average error.
- **Variance**: Approaches 0.0833, diminishing the effect of sample fluctuations.

Assessing empirical mean and variance against theoretical values reveals how closely a random sample mirrors an ideal uniform distribution. It also gauges a simulation's accuracy based on sample size.
