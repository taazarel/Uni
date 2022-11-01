#forelæsning 
# Spørgsmål

# Beskrivelse
Vi skal tale om [[Retningsafledte#Partielt afledte funktioner|diffrentation]], [[Retningsafledte#$C {1}$|C1]] og tangentplaner.
En hyperplan er noget som har n-1 dimensioner fra den dimension vi arbejder i. En plan i 2d er en linje fx.
En hyperplan beskrives som... :: en graf som har n-1 dimensioner fra den n dimension vi arbejder i.

# Forelæsning
## Definition(Affin funktion)
En funktion $h:\mathbb{R}^{n}\to \mathbb{R}$ kaldes affin når den er på denne form... :: $h(x_{1},...,x_{n})=a_{1}x_{1}+a_{2}x_{2}+...+a_{n}x_{n}+d \text{ hvor } a_{1},...,a_{n},d \in \mathbb{R}$ [^1]

En affin funktion af 2 variable beskrives således...
En affin funktion af 3 variable beskrives således...
?
$n=2 \text{ , } h(x,y)=ax+by+d$
$n=3 \text{ , } h(x,y,z)=ax+by+cz+d$

En affin funktion kan kaldes for en lineær funktion når $d=0$, men dette er grunden... :: $d=0$, da dette gør grafen af den lineære funktion til et underrum. Vi kan skrive $\vec{0}\in \{\vec{x}+r \vec{v}+s \vec{w}|r \}$
Grafen for en affin funktion er... :: hyperplan.
### Eksempel:
$h(x,y)=2x+3y+\sqrt{7}$ er en affin funktion
### Eksempel af en affin funktion med n=1.
$h(x)=3x+2$ Dette er stadigvæk ikke en lineær funktion da $d \neq 0$

## Definition 2.61 (Tangering)
Vi har en tangering af to funktioner $f,g$ af n variabler og $\vec{a}\in D_{f}\cap D_{g}$ når... :: $$f(\vec{a})-g(\vec{a})$$ og $$\lim_{\vec{x}\to\vec{a}} \frac{f(\vec{x})-g(\vec{x})}{||\vec{x}-\vec{a}||}=0$$



[^1]: Hvis d=0 så kaldes dette for en lineær funktion