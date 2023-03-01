#kapitel 
# §6.1 Outline of the method

Vi kan finde det mest optimale $\chi ^{2}$ ved at minimere... :: det frie udtryk når vi tager ML. Ved gauss distribution bliver det $\chi ^{2} = \sum_{j=1}^{N} \frac{(x_{j}-\hat \mu)^{2}}{\sigma^{2}}$. [^1]

For at finde det mindste $\chi ^{2}$ kan vi blot... :: differentiere til estimatorene og sætte det lig nul $$\frac{d \chi ^{2}}{d\hat a}=0 \Leftrightarrow \frac{1}{\sigma^{2}}\sum_{j=1}^{N}\frac{df(x_{j}:\hat a)}{d\hat a}[y_{j} - f(x_{j}:\hat a)] = 0$$[^2]  

# §6.6 Linear Least Squares and Matrices

$$\sum_{i=1}^{N}\sum_{j=1}^{N} [y_{i}-f(x_{i})]$$

# §6.7 Non-linear Least Squares

[^1]:Her bliver $\langle \chi ^{2} \rangle = N$, $V(\chi ^{2})=2N$, $\sigma_{\chi^{2}}= \sqrt{2N}$.
[^2]: Hvor data normalt skrives som $y_{j}$ og modellen $x_{j}$.