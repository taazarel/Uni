#kapitel 
# §5.1 Properties of Estimators
A good Estimator has these properties
- Consistency
- Bias
- Efficiency
Which are explained as...
?
- Estimators are consistent when $\lim_{n \to \infty} â = a$
- If its expectation value is equal to the true value $\langle â \rangle = a$
- Lastly. An estimator is efficient when its variance is small. This just means that we should pick the model which gives the smallest variance.
# §5.2 Some basic estimators
## §5.2.1 Estimating the Mean
To estimate the mean we... :: use the Central limit theorem ([[Errors#The central limit theorem|CLT]])[^1]
<!--SR:!2023-03-03,3,250-->

## §5.2.2 Estimating the Variance
The variance can be shown as... :: $\hat V(x) = s^{2} = \frac{1}{N-1} \sum (x_{i}-\vec{x})^{2}$ (5.14) this is the unbiased and consistent version used for instances where we do not know the true $\mu$. Otherwise use $\hat V(x) = \frac{1}{N} \sum (x_{i}-\mu )^{2}$  
<!--SR:!2023-03-04,4,270-->

## §5.2.3 Estimating $\sigma$.
Estimating $\sigma$ has two useful answers, where the error of the estimate is... :: $\sigma_{\sigma} = \frac{\sigma}{\sqrt{2N}}$ (5.23) when we know $\mu$. And $\sigma_{s}= \frac{\sigma}{\sqrt{2(N -1)}}$ (5.24) as an extrapolation of (5.14)
<!--SR:!2023-03-04,4,274-->
Estimating $\sigma$ gives us two answers, one for when we know the model, and one where we do not. These are written as... :: $\hat \sigma = \sqrt{\hat V(x)}$ for known theory and $\hat\sigma = s$ for equation (5.14).
<!--SR:!2023-03-04,4,274-->

# §5.3 Maximum likelihood
For a data sample, the maximum likelihood for an estimator is... :: the maximum for equation (5.1) which is $L(x_{1},...,x_{n}) = \Pi P(x_{i}, a)$.[^2] This value is called ML.
<!--SR:!2023-03-04,4,270-->

[^1]: Remember the variance of this mean. This mean is consistent and unbiased.
[^2]: It is usually easier to find the maximum of the log of L.