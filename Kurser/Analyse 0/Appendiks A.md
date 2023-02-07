#formler
# Formelsamling
## Algebraiske formler
$\sqrt{x}-\sqrt{y}= \frac{x-y}{\sqrt{x}+\sqrt{y}}$
### Kvadratsætninger (A.1)[^1]
$(a+b)^{2}= a^{2}+b^{2}+2ab$
$(a-b)^{2}= a^{2}+b^{2}-2ab$
$(a+b)(a-b)= a^{2}-b^{2}$

## Trigonometriske formler
$\gamma (x)=(\cos{x},\sin{x})$ (A.10)
$$Q_{x}=\left[
\begin{array}{cc}
\cos{x} & -\sin{x} \\ 
\sin{x} & \cos{x}
\end{array}
\right] $$ (A.14)[^2]

$\gamma (x + y)=Q_{x}\cdot \gamma (y)$ (A.16)[^3]

### Additionsformler[^4]
$\cos{x+y}= \cos{x}\cos{y}-\sin{x}\sin{y}$
$\sin{x+y}=\sin{x}\cos{y}+\cos{x}\sin{y}$

#### Fordoblingsformlerne[^5]
$\cos{2x}=\cos^{2}{x}-\sin^{2}{x}$
$\sin{2x}=2\cos{x}\sin{x}$

$|\sin{x}|\leq |x|$ (A.20)

## Logaritme & Eksponentiale funktioner
$f(xy)=f(x)+f(y) \text{ for alle }x,y >0$ (A.25) (Logaritmens funktionalligning)

Herfra kan vi udlede $f(1)=0$ (A.26) og $f(\frac{x}{y})=f(x)-log(y)$ (A.27)
samt $f(x^{n})=n \cdot f(x)$ (A.28)

Der er kun én funktion som opfylder både logaritmensfunktionalligning og $f(x)\leq x-1 \text{ for alle }x >0$. Denne kalder vi $log(x)$ og det er den naturlige logaritme.

$log(x)\geq \frac{x-1}{x}\text{ givet }x>0$. (A.31)

Den naturlige logaritme har en invers som vi kalder den eksponentialfunktionen. $exp(a+b)=exp(a)exp(b)\text{ for }a,b \in \mathbb{R}$(A.33)

[^1]: Kvadratsætninger er strengt voksende
[^2]: Q er en ortonormal matrix og dens determinant er 1. Dette betyder at Q er en rotation, som starter i (1,0)
[^3]: Dette er altså en rotation som først drejer med x, og derefter med y.
[^4]: Disse bliver direkte afledt fra A.16.
[^5]: Findes gennem additionsformlerne