#kapitel
# What is probability?
There are four kinds of probability
- Mathematical (Theory)
- Empirical (Data)
- Objective
- Subjective (Bayesian)

## Mathematical probability
For a set of possible results S. Every event in this set has a probability of occurring $P(E)$ where this real number must follow...
?
1. $P(E)\geq 0$
2. $P(E_{1}\space or \space E_{2})=P(E_{1},E_{2})=P(E_{1})+P(E_{2})$[^1]
3. $\sum P(E_{i})=1$

Mathematical probability has a hole in it in the sense that... :: the number which represents the probability holds no meaning.
<!--SR:!2023-02-23,4,272-->

## Empirical Probability
When an experiment is performed N times, and A occurs M times, then while $N \to \infty$... :: a rational number occurs, which is represented by the ratio $\frac{M}{N}$ and denoted as the probability $P(A)$.[^2]
<!--SR:!2023-02-18,4,270-->

Empirical probability unfortunately has two shortcomings
1. The probability of an event...
2. Repeatability is...
?
1. is not a true property of the experiment, but a property of the experiment against the population.
2. a must for experiments. And the experiment must be repeatable with a range of different possible outcomes and identical starting conditions.

## Objective Probability / Propensity
Objective probability states that probability is... :: an objective, observable and unchanging characteristic for a certain object. 
<!--SR:!2023-02-23,4,272-->
Objective probability is the king of discrete sets of numbers, but... :: its theory breaks down when applied to continuous sets.
<!--SR:!2023-02-23,4,272-->

## Subjective Probability[^4]
Conditional probability is... :: The probability that a is true given b is true, and is denoted with $P(A|B)$.
<!--SR:!2023-02-22,3,252-->
Bayes theorem uses $P(A|B)P(B)=P(A \text{ and } B)=P(AB)=P(B|A)P(A)$ to find the probability for $P(A|B)=$... :: $\frac{P(B|A)P(A)}{P(B)}$ (7.1)
<!--SR:!2023-02-23,4,272-->
Often we will define $P(B)$ by $\vec{A}$[^3] like this... :: $P(B)=P(B|A)P(A)+P(B|\vec{A})P(\vec{A})$ (7.2)
<!--SR:!2023-02-22,3,252-->

## Bayesian Statistics
Bayesian statistics seeks to help rectify the shortcomings of the unscientific hole in empirical probability. This is achieved by... :: substituting actual probability for an initial guess and the degree of belief in which the experimentor has.[^5]
<!--SR:!2023-02-23,4,272-->



[^1]: Given that E_1 and E_2 are mutually exclusive. Which means that they both cant happen at once. It cant both rain and not rain at the same time.
[^2]: The set of all experiments is called, the collective, ensemble or population.
[^3]: Where $\vec{A}$ denotes "not A".
[^4]: Is also known as Bayesian statistics
[^5]: This is still unscientific for continous cases.