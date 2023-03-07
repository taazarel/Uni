#aflevering 
# Opgave 1


# Opgave 2
$$\sinh(x)' = f'(x) + g'(x) = \left(\frac{e^{x}}{2}\right)' + \left(\frac{-e^{-x}}{2}\right)' = \frac{e^{x}}{2} - \frac{e^{-x}}{2}(-1)$$
$$= \frac{e^{x}+e^{-x}}{2}=\cosh(x)$$
Vi kan også gøre dette for vores $\cosh(x)$.
$$\cosh(x)' = \left(\frac{e^{x}}{2}\right)' + \left(\frac{e^{-x}}{2}\right)' = \frac{e^{x}-e^{-x}}{2} =\sinh(x)$$
Da vi har brugt differentialerne af funktioner som vi kender. Kan vi konkludere at dette må virke for alle $x \in \mathbb{R}$.

For $\tanh(x)'$ bruger vi både produkt og kædereglen.
$$\tanh(x)' = \sinh(x)' \frac{1}{\cosh(x)} + \sinh(x) \left(\frac{1}{\cosh(x)}\right)'$$
$$= \frac{\cosh(x)}{\cosh(x)} + \sinh(x) (-1)\left(\frac{1}{\cosh^{2}(x)}\right)\sinh(x)$$
$$=1 - \frac{\sinh^{2}(x)}{\cosh^{2}(x)} = 1 - \tanh^{2}(x)$$
Vi kan også skrive
$$\frac{\cosh^{2}(x)-\sinh^{2}(x)}{\cosh^{2}(x)} $$
Vi ved at $\cosh^2(x)-\sinh^2(x)=1$ så derfor bliver udtrykket
$$\frac{1}{\cosh^{2}(x)}$$
# Opgave 3


# Opgave 4
## a
$\tan(x)= \frac{\sin{x}}{\cos{x}}$ for $|x|< \frac{\pi}{2}$.

Vi skal bruge både kæde og produktreglerne. $$\tan'{x}=\sin'{x} \frac{1}{\cos{x}}+ \sin{x}\left(\frac{1}{\cos{x}}\right)' = \frac{\cos{x}}{\cos{x}}+ \sin{x}\left(\frac{-1}{\cos^{2}{x}}\right)(-\sin{x})$$
$$= 1+ \frac{\sin^{2}{x}}{\cos^{2}{x}}=1+ \left(\frac{\sin{x}}{\cos{x}}\right)^{2}=1 + \tan^{2}{x}$$
Lad os gøre dette igen for $\tan'{x}$.
$$\tan''{x}=\left(1+ \tan^{2}{x}\right)' = \left(\left(\tan{x}\right)^{2}\right)'=2 \tan{x}(1+ \tan^{2}{x})=2 \tan{x}+ 2\tan^{3}{x}$$

Dette dur så længe at tan(x) er kontinuert, hvilket gælder for $x \in (0,\pi )$.
## b
$$\tan'{x}=Q_{1}(\tan{x})=1+ \tan^{2}{x}$$
$$\tan''{x}=Q_{2}(\tan{x})=2\tan{x}+2\tan^{3}{x}=2\tan{x}(1+\tan^{2}{x})$$
Hvis vi differentierer $Q_{1}(\tan{x})=1+ \tan^{2}{x}=(1+y^{2})\Rightarrow (1+y^{2})' = 0 + 2y = 2\tan{x}$.
Nu finder vi at dette er det samme som hvad står udenfor parantesen i $Q_{2}(\tan{x})$. Her finder vi at sammenhængen mellem $Q_{1}$ og $Q_{2}$ er $Q_{2}(\tan{x})=(Q_{1}(\tan{x}))'(1+\tan^{2}{x})$.

Til sidst kan vi bevise dette forhold mere generelt gennem induktion.

## c
Brug sammenhængen fundet fra (4.b) til at opskrive taylor polynomiet for 5 grad og omkring punktet 0.
$$P_{5}(tan(x))=\tan{x}+ \frac{Q_{1}(\tan{x})}{1!}x + \frac{Q_{2}(\tan{x})}{2!}x^{2} + \frac{Q_{3}(\tan{x})}{3!}x^{3}+ \frac{Q_{4}(\tan{x})}{4!}x^{4}+ \frac{Q_{5}(\tan{x})}{5!}x^{5}$$
$$Q_{1}(x)=1+x^{2}$$
$$Q_{2}(x)=2x(1+x^{2}) = 2x+ 2x^{3}$$
$$Q_{3}(x)=(2+6x^{2})(1+x^{2})=2+2x^{2}+6x^{2}+6x^{4}$$
$$Q_{4}(x)=(16x + 24x^{3})(1+x^{2})=16x+24x^{3}+16x^{3}+24x^{5}$$
$$Q_{5}=(16+120x^{2}+140x^{4})(1+x^{2})=16+136x^{2}+260x^{4}+140x^{6}
$$$$=16+136x^{2}+260x^{4}+140x^{6}$$
$$P_{5}(\tan{x})=\tan{x}+\frac{1+\tan^{2}{x}}{1!} x+\frac{2\tan{x}+2\tan^{3}{x}}{2!} x^{2}+\frac{2+8\tan^{2}{x}+6\tan^{4}{x}}{3!} x^{3}$$
$$+\frac{16\tan{x}+40\tan^{3}{x}+24\tan^{5}{x}}{4!} x^{4}+\frac{16+136\tan^{2}{x}+260\tan^{4}{x}+140\tan^{6}{x}}{5!} x^{5}$$

## d


# Opgave 5
