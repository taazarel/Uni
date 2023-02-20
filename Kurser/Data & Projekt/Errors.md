#kapitel 
# 4.1 Why errors are Gaussian
## The central limit theorem
Givet at summen X af N uafhængige variabler hver taget fra en distribution med gennemsnit $\mu_{i}$ og varians $V_{i}$ har distributionen for X
1. Summen af alle middelværdierne er det samme som... 
2. Variansen er...
3. Bliver...
?
middelværdien af hele summen. $E(x)= E(\sum x_{i})=\sum E(x_{i})=\sum \mu_{i}$.
$V(x)=\sum V_{i}=\sum \sigma^{2}$
gaussian når $N \to \infty$.

# 4.2 Working with errors
## Repeated measurements
Den samme ting måles flere gange. Så kan vi bruge CLT som vi forenkler til at alle $\mu_{i}=\mu$ og $\sigma_{i}=\sigma$. Så finder vi
Gennemsnittet bliver...
Variansen bliver...
?
$\vec{x}= \frac{X}{N} \Rightarrow E(\vec{x})=\mu$.[^1] (4.5)
$V(\vec{x})=\frac{1}{N^{2}}\sum V_{i}= \frac{\sigma^{2}}{N}$. (4.6)[^2]

## Averaging Weighted Measurements
The generalised weight given to a result is proportional to the inverse square of the resolution... :: $\vec{x}=\frac{\sum\frac{x_{i}}{\sigma_{i}^{2}}}{\sum \frac{1}{\sigma_{i}^{2}}}$.
The variance becomes this when weighted... :: $V(\vec{x})= \frac{1}{\sum \frac{1}{\sigma_{i}^{2}}}$.

# 4.3 Combination of Errors
## One variable
Given $f(x)=ax+b$ is linear and of one variable, then
1. $E(f)=...$
2. $V(f)=...$
3. $V(f)\approx...$
?
$aE(x)+b$
$a^{2}V(x)$
$\left(\frac{df}{dx}\right)^{2}V(x)$

## Two or more variables
## The law of combination of errors
If $f$ is a function of more than one variable, and is linear $f(x,y)=ax+by+c$. Given the independency of these variables, then the error becomes a combination of the variables written as... :: $$V(f)= \left(\frac{df}{dx}\right)^{2}V(x)+\left(\frac{df}{dy}\right)^{2}V(y)$$[^3]


[^1]: Dette er altså gennemsnittet af gennemsnittet.
[^2]: Her er $\sigma_{x}= \frac{1}{\sqrt{N}}\sigma$
[^3]: Ergo kan vi finde standardafvigelsen ved at tage kvadratroden, og derved har vi obhobningsloven