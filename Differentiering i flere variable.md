#kapitel 
## Partielle afledte
En funktion er partielt afledt når... :: den er differentiabel i x-retningen af denne variabel. $$\frac{f(x,a_{2})-f(a_{1},a_{2})}{x-a_{1}}\to c \text{ for }x \to a_{1}$$
## Retningsafledte
En funktion er retningsafledt når... :: den er differentiabel i v's retning i  punkt a, hvis funktionen er differentiabel i t=0. [^1]$$\frac{f(\vec{a}+t \vec{v})-f(\vec{a})}{t}\to c \text{ for }t \to 0$$
## Gradient
Gradienten for en funktion f defineres som... :: En vektor $\vec{c}\in \mathbb{R}^{k}$ som opfylder i grænseovergangen $\Delta x \to 0$: $\Delta f= \vec{c}\cdot \Delta \vec{x} + \epsilon (\Delta \vec{x})||\Delta \vec{x}||$  Noter at vi ofte skriver $\vec{c}=\nabla f(\vec{a})$

## $C^{1}$ betingelsen
Givet er $f:\Omega \to \mathbb{R}$ og $\vec{a}\in \Omega$. f er c1 hvis... :: $x \to \nabla f(x)$ er kontinuert og har partielt afledte i alle punkter i alle retninger i domænet $\Omega$. Så er f differentiabel i $\vec{a}$, og er $C^{1}$.

## Definition for differentiabilitet i dimension $k \to m$
Lad $\Omega \subset \mathbb{R}^{k}$ være en åben mængde . Lad $f:\Omega \to \mathbb{R}^{m}$ være en afbildning og $\vec{a} \in \Omega$. Så vil f være differentiabel i $\vec{a}$ med funktionalmatrix C hvis... :: $\Delta f = f(\vec{a}+\Delta \vec{x})-f(\vec{a})= C \Delta \vec{x}+ \epsilon (\Delta \vec{x})||\Delta \vec{x}||$ er sandt.

Funktionalmatricen skrives som... :: $$Df(\vec{a})= \left[
\begin{array}{ccc}
\frac{\delta f_{1}}{\delta x_{1}} & ... & \frac{\delta f_{m}}{\delta x_{1}} \\ 
\vdots & ... & \vdots \\ 
\frac{\delta f_{1}}{\delta x_{k}} & ... & \frac{\delta f_{m}}{\delta x_{k}}
\end{array}
\right]$$
## Den generaliserede kæderegel
Den sammensatte afbilding $g \circ f$ kan skrives gennem funktionalmatricer således... :: $D(g\circ f)(\vec{a})= Dg(f(\vec{a}))Df(\vec{a})$[^2]



[^1]: Dette er hvor den partielle afledte kommer fra. Her insisterer vi blot på en retning (vektoren v) fra start.
[^2]: Det er meget vigtigt at man husker den korrekte rekkæfølge i produktet. Disse er jo matricer, hvilket betyder at vores kommutative regel ikke gælder.