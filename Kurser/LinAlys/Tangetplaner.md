#forelæsning 
# Spørgsmål

# Beskrivelse
Vi skal tale om [[Retningsafledte#Partielt afledte funktioner|diffrentation]], [[Retningsafledte#$C {1}$|C1]] og tangentplaner.
En hyperplan er noget som har n-1 dimensioner fra den dimension vi arbejder i. En plan i 2d er en linje fx.

# Forelæsning
## Definition(Affin funktion)
En funktion $h:\mathbb{R}^{n}\to \mathbb{R}$ kaldes affin når den er på denne form... :: $h(x_{1},...,x_{n})=a_{1}x_{1}+a_{2}x_{2}+...+a_{n}x_{n}+d \text{ hvor } a_{1},...,a_{n},d \in \mathbb{R}$ [^1]
<!--SR:!2022-11-25,18,270-->

En affin funktion af 2 variable beskrives således...
En affin funktion af 3 variable beskrives således...
?
$n=2 \text{ , } h(x,y)=ax+by+d$
$n=3 \text{ , } h(x,y,z)=ax+by+cz+d$
<!--SR:!2022-11-27,20,290-->

En affin funktion kan kaldes for en lineær funktion når $d=0$, men dette er grunden... :: $d=0$, da dette gør grafen af den lineære funktion til et underrum. Vi kan skrive $\vec{0}\in \{\vec{x}+r \vec{v}+s \vec{w}|r,s \in \mathbb{R} \}$.
<!--SR:!2022-11-26,19,290-->
Grafen for en affin funktion er... :: hyperplan.
<!--SR:!2022-12-15,30,270-->
Man kan definere en hyperplan som... :: en graf som har n-1 dimensioner fra den n dimension vi arbejder i.
<!--SR:!2022-11-27,20,290-->
### Eksempel:
$h(x,y)=2x+3y+\sqrt{7}$ er en affin funktion
### Eksempel af en affin funktion med n=1.
$h(x)=3x+2$ Dette er stadigvæk ikke en lineær funktion da $d \neq 0$

## Definition 2.61 (Tangering)
Vi har en tangering af to funktioner $f,g$ af n variabler og $\vec{a}\in D_{f}\cap D_{g}$ når... :: $$f(\vec{a})-g(\vec{a})$$ og $$\lim_{\vec{x}\to\vec{a}} \frac{f(\vec{x})-g(\vec{x})}{||\vec{x}-\vec{a}||}=0$$
<!--SR:!2022-11-23,16,270-->
Hvad kalder man det hvis funktionen f tangerer en affin funktion h i a... :: at grafen for f har en tangenthyperplan givet ved grafen af h.
<!--SR:!2022-11-15,8,230-->

## Sætning 2.62(Entydighed af tangentplan)
Entydighed af en tangenthyperplan betyder blot at... :: Der kan højst være **en** tangenthyperplan af 2 funktioner.
<!--SR:!2022-11-26,19,290-->
### Oversættelse
Vi prøver at sige dette. Hvis man har en lige linje som tangerer en funktion på et punkt, kan der kun være en lineær funktion som tangerer i dette punkt.
### Bevis
hvis $h_{1}\text{ og }h_{2}$ er to affine funktioner der begge tangerer f i $\vec{a}$ da må $h_{1}\text{ og }h_{2}$ tangerer hinanden, dvs:
$$\frac{h_{1}(\vec{x})-h_{2}(\vec{x})}{||\vec{x}-\vec{a}||}\to_{\vec{x}-\vec{a}}0$$

## Sætning 2.63
Vi kan med sikkerhed finde en affin funktion som tangerer f i $\vec{a}$ når... :: f er $C^{1}$ og $\vec{a}$ er et indre punkt i $D_{f}$.
<!--SR:!2022-11-28,21,290-->
Man definerer en tangenthyperplan h som en affin funktion matematisk således... :: $h(\vec{x})=f(\vec{a})+\nabla f(\vec{a})\cdot (\vec{x}-\vec{a})$[^2]
<!--SR:!2022-11-25,18,290-->

## Definition 2.67(Differentiabilitet af funktioner af flere variabler)
En funktion f er diffrentiabel i et indre punkt $\vec{a}$ i $D_{f}$ hvis... :: der findes en affin funktion der tangerer f i det punkt.
<!--SR:!2022-11-15,4,190-->
En 
funktion $C^{1}$ medfører at... :: Funktionen er differentiabel.
<!--SR:!2022-11-24,17,290-->
Differentiabilitet af en funktion medfører at... :: Funktionen har en partielt afledt i $\vec{a}$.
<!--SR:!2022-11-21,14,270-->

## Sætning 2.70(Kædereglen af funktioner af flere variabler)

Givet er $f(u_{1},...,u_{m})$ er $C^{1}$ og $g_{1}(x_{1},...,x_{n}),g_{2}(x_{1},...,x_{n}),...,g_{m}(x_{1},...,x_{n}) \text{ er alle }C^{1}$.
Hvis vi indsætter g funktionerne på u pladserne i f, så er følgende sandt
Og differentiationen af k kan skrives således:
?
$k(x_{1},...,x_{n})=f(g_{1}(x_{1},...,x_{n}),...,g_{m}(x_{1},...,x_{n}))$ er derved $C^{1}$.
$$\frac{dk}{dx_{j}}(\vec{a})= \frac{df}{du_{1}}(\vec{b}) \frac{dg_{1}}{dx_{j}}(\vec{a})+...+ \frac{df}{du_{m}}\vec{b} \frac{dg_{m}}{dx_{j}}(\vec{a})$$
Hvor $\vec{a}=(a_1,...,a_{n})\in \mathbb{R}^{n}$ og $\vec{b}=g_{1}(\vec{a}),g_{2}(\vec{a}),...,g_{m}(\vec{a})\in \mathbb{R}^{m}$.
<!--SR:!2022-11-25,18,270-->

## Tangenten for [[Partiel integration#Def 1.5 (Niveaukurve)|niveaukurven]].
Princip: Tangenten til niveaukurven er niveaukurven til den tangerende affine funktion.

## Definition 2.72 (Tangent til niveaukurven)
Givet er en $C^{1}$ funktion og punktet $\vec{a}\in D_{f}$. Så vil tangenten til niveaukurven i $\vec{a}$ være... :: $f(\vec{a})+\nabla f(\vec{a})\cdot (\vec{x}-\vec{a})=f(\vec{a})$.[^3]
<!--SR:!2022-11-28,17,275-->


[^1]: Hvis d=0 så kaldes dette for en lineær funktion
[^2]: Dette ligner meget et Taylorpolynomie når det bliver udvidet: $f(\vec{a})+ \frac{df}{dx_{1}}\vec{a}(x_{1}-a_{1})+...+ \frac{df}{dx_{n}}\vec{a}(x_{n}-a_{n})$
[^3]: Ergo det samme som niveaukurven af tangenten til f.