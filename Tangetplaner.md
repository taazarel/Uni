#forelæsning 
# Spørgsmål

# Beskrivelse
Vi skal tale om [[Retningsafledte#Partielt afledte funktioner|diffrentation]], [[Retningsafledte#$C {1}$|C1]] og tangentplaner.
En hyperplan er noget som har n-1 dimensioner fra den dimension vi arbejder i. En plan i 2d er en linje fx.

# Forelæsning
## Definition(Affin funktion)
En funktion $h:\mathbb{R}^{n}\to \mathbb{R}$ kaldes affin når den er på denne form... :: $h(x_{1},...,x_{n})=a_{1}x_{1}+a_{2}x_{2}+...+a_{n}x_{n}+d \text{ hvor } a_{1},...,a_{n},d \in \mathbb{R}$ [^1]

En affin funktion af 2 variable beskrives således...
En affin funktion af 3 variable beskrives således...
?
$n=2 \text{ , } h(x,y)=ax+by+d$
$n=3 \text{ , } h(x,y,z)=ax+by+cz+d$

En affin funktion kan kaldes for en lineær funktion når $d=0$, men dette er grunden... :: $d=0$, da dette gør grafen af den lineære funktion til et underrum. Vi kan skrive $\vec{0}\in \{\vec{x}+r \vec{v}+s \vec{w}|r,s \in \mathbb{R} \}$.
Grafen for en affin funktion er... :: hyperplan.
Man kan definere en hyperplan som... :: en graf som har n-1 dimensioner fra den n dimension vi arbejder i.
### Eksempel:
$h(x,y)=2x+3y+\sqrt{7}$ er en affin funktion
### Eksempel af en affin funktion med n=1.
$h(x)=3x+2$ Dette er stadigvæk ikke en lineær funktion da $d \neq 0$

## Definition 2.61 (Tangering)
Vi har en tangering af to funktioner $f,g$ af n variabler og $\vec{a}\in D_{f}\cap D_{g}$ når... :: $$f(\vec{a})-g(\vec{a})$$ og $$\lim_{\vec{x}\to\vec{a}} \frac{f(\vec{x})-g(\vec{x})}{||\vec{x}-\vec{a}||}=0$$
Hvad kalder man det hvis funktionen f tangerer en affin funktion h i a... :: at grafen for f har en tangenthyperplan givet ved grafen af h.

## Sætning 2.62(Entydighed af tangentplan)
Entydighed af en tangenthyperplan betyder blot at... :: Der kan højst være **en** tangenthyperplan af 2 funktioner.
### Oversættelse
Vi prøver at sige dette. Hvis man har en lige linje som tangerer en funktion på et punkt, kan der kun være en lineær funktion som tangerer i dette punkt.
### Bevis
hvis $h_{1}\text{ og }h_{2}$ er to affine funktioner der begge tangerer f i $\vec{a}$ da må $h_{1}\text{ og }h_{2}$ tangerer hinanden, dvs:
$$\frac{h_{1}(\vec{x})-h_{2}(\vec{x})}{||\vec{x}-\vec{a}||}\to_{\vec{x}-\vec{a}}0$$

## Sætning 2.63
Vi kan med sikkerhed finde en affin funktion som tangerer f i $\vec{a}$ når... :: f er $C^{1}$ og $\vec{a}$ er et indre punkt i $D_{f}$.
Man definerer en affin funktion matematisk som... :: $h(\vec{x})=f(\vec{a})+\nabla f(\vec{a})\cdot (\vec{x}-\vec{a})$[^2]


[^1]: Hvis d=0 så kaldes dette for en lineær funktion
[^2]: Dette ligner meget et Taylorpolynomie når det bliver udvidet: $f(\vec{a})+ \frac{df}{dx_{1}}\vec{a}(x_{1}-a_{1})+...+ \frac{df}{dx_{n}}\vec{a}(x_{n}-a_{n})$
