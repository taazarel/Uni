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

# §5.2.1 Estimating the Mean
To estimate the mean we... :: use the Central limit theorem ([[Errors#The central limit theorem|CLT]])[^1]

# §5.2.2 Estimating the Variance
The variance can be shown as... :: $\hat V(x) = s^{2} = \frac{1}{N-1} \sum (x_{i}-\vec{x})^{2}$ (5.14) this is the unbiased and consistent version used for instances where we do not know the true $\mu$. Otherwise use $\hat V(x) = \frac{1}{N} \sum (x_{i}-\mu )^{2}$  

# §5.2.3 Estimating $\sigma$.
Estimating $\sigma$ has two useful answers... :: $\sigma_{\sigma} = \frac{\sigma}{\sqrt{2N}}$ (5.23) when we know $\mu$. And $\sigma_{s}= \frac{\sigma}{\sqrt{2(N -1)}}$ (5.24) as an extrapolation of (5.14)


[^1]: Remember the variance of this mean. This mean is consistent and unbiased.