#kapitel 
# §6.1 Outline of the method

Vi kan finde det mest optimale $\chi ^{2}$ ved at minimere... :: det frie udtryk når vi tager ML. Ved gauss distribution bliver det $\chi ^{2} = \sum_{j=1}^{N} \frac{(x_{j}-\hat \mu)^{2}}{\sigma^{2}}$. [^1] <!--SR:!2023-05-14,54,290-->

For at finde det mindste $\chi ^{2}$ kan vi blot... :: differentiere til estimatorene og sætte det lig nul $$\frac{d \chi ^{2}}{d\hat a}=0 \Leftrightarrow \frac{1}{\sigma^{2}}\sum_{j=1}^{N}\frac{df(x_{j}:\hat a)}{d\hat a}[y_{j} - f(x_{j}:\hat a)] = 0$$[^2]   <!--SR:!2023-04-08,18,250-->
# §6.4 The $\chi^{2}$ distribution
For at finde ud af om sandsynligheden for at $\chi^{2}$ passer på modellen kan vi... :: opstille en distribution som viser sandsynligheden $$P(\chi^{2};n)= \frac{2^{\frac{-n}{2}}}{\Gamma(\frac{n}{2})}\chi^{n-2}e^{\frac{-\chi^{2}}{2}}$$ (6.18) Hvis $\chi ^{2}$ er meget lille er vores errors nok for store. [^5] <!--SR:!2023-03-24,3,250-->


# §6.6 Linear Least Squares and Matrices

A linear Least Square describes... :: a model in which the parametres are linear. This can be written as. $$\sum_{i=1}^{N}\sum_{j=1}^{N} [y_{i}-f(x_{i}:\vec{a})]V_{ij}^{-1}[y_{j}-f(x_{j}:\vec{a})]$$$$\Rightarrow \chi ^{2} = (\vec{y'}-\vec{f'})\vec{V}^{-1}(\vec{y}-\vec{f})$$ (6.20)[^3] <!--SR:!2023-05-09,49,270-->

# §6.7 Non-linear Least Squares

For non-linear least squares we can find the answer by... :: an **iterative**[^4] approach. Given a first guess we find the gradient and look for static points. <!--SR:!2023-04-13,23,270-->


[^1]:Her bliver $\langle \chi ^{2} \rangle = N$, $V(\chi ^{2})=2N$, $\sigma_{\chi^{2}}= \sqrt{2N}$.
[^2]: Hvor data normalt skrives som $y_{j}$ og modellen $x_{j}$.
[^3]: hvor ' betyder at det er en invers vektor/matrix.
[^4]: The method is often the "Leuwenberg-Morquordt algrorithm/interpolation".
[^5]: Gennemsnittet er n, og variansen 2n