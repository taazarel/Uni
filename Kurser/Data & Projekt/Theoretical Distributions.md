#kapitel 
# General Properties of distributions
## A simple distribution
The outcome of $P(A|B)=...$::$P(A)P(B)$ given mutual exclusivity.
If given a set of probabilities $P(r)$ which are defined by the outcome r we have... :: a probability distribution. 
<!--SR:!2023-02-15,1,230-->

## The law of large numbers
Small sample sizes in statistics leave much room for error. Thus if we wish to diminish this error we... :: increase the sample size. Since the law of large numbers states that when $N \to \infty$ then $\frac{M}{N}=P$.

## Expectation values
We can compute the expected result of a probability distribution... :: $$E(r)=\sum_{r}rP(r)$$(3.1)[^1] Any function of r (f(r)) has a expectation value defined in the same way (3.2)

As $N \to \infty$ then the mean... :: approaches the expected value.

## Probability Density Distributions (KDE)
When working with continuous sets we can not set a specific size for measurements. However, this is fixed by... :: denoting the probability of an outcome finding itself inside a given range.

The probability of a result between a and b is... :: $$\int_{a}^{b}P(x)dx $$
# The Binomial Distribution
The binomial distribution is very rigid in its construction. It has these properties...
?
1. It operates on (True or False) or (Successes and Failures).
2. It describes a given number of trials/experiments. It is therefore a discrete distribution.
3. It denotes success with p, failure with $(1-p)$ or q and amount of trials as n. The amount of successes is denoted r whilst the amount of failures is $(n-r)$.

The binomial probability distribution is written as the probability of r successes out of n trials, with the probability of p for success... :: $P(r;p,n)=p^{r}(1-p)^{n-r} \frac{n!}{r!(n-r)!}$ (3.6)

We have a few meaningful properties of the binomial...
1. The mean of successes is...
2. The variance is given by...
3. The standard deviation is...
?
1. $E(r)=np$ (3.8)
2. $V(r)=np(1-p)$ (3.9)
3. $\sigma = \sqrt{np(1-p)}$ (3.10)

# Poisson Distribution
For an interval, an average expected amount of values to occur is denoted $\lambda$. If we were to dissect this interval into indices so small that only one could occur at each slice, then use the binomial distribution we would find the probability... :: $P(r;\lambda )= \frac{e^{-\lambda}\lambda^{r}}{r!}$ (3.11) which is the probability of obtaining r events given the expected value $E(r)=\lambda$.[^2]

# Normalfordeling / Gaussian Distribution
Normalfordelingen or "The gaussian" has a range of useful features. Including...
?
Its curve being centred on  $\mu$ the average.
Its width is proportional to $\sigma$.
The area under the distribution is 1.
The formula is written as$$P(r)= e^{\frac{-(x-\mu)^{2}}{2\sigma^{2}}} \frac{1}{\sigma \sqrt{2 \pi }}$$
# Breit-wigner / Cauchy / Lorentz Distribution
This distribution is used for particles in physics and is written as... :: $$F(m;M, \Gamma )= \frac{1}{2\pi } \frac{\Gamma}{(m-M)^{2}+  (\frac{\Gamma }{2})^{2}}$$

[^1]: Where E(r) is the expectation value. Also sometimes written as $\langle r \rangle$ or $\mu$. r is the result and P(r) is the probability for the result.
[^2]: The variance is also $V(r)=\lambda$ and therefore the deviation is $\sigma = \sqrt{\lambda }$.