#forelæsning 
Begyndelsesdato: 07:54   11-10-2022   Uge-41
## Dagens Emner
Specifikt handler disse emner om at differentiere funktioner af flere variable.
Jan siger at det er svært, siden der er mange typer af differentiationer.
- Retningsafledte funktioner 
- Partielt afledte funktioner
- Gradient
- Grænseværdier af funktioner med flere variabler
- Kontinuitet af funktioner med flere variabler
- $C^{1}$ funktioner[^1]
# Partielt afledte funktioner
Man "Fryser" variablerne indtil at man kun har en variabel. Derfor kan man bare differentiere den som en normal funktion.
## Definition
$f:A \rightarrow \mathbb{R}, \vec{a}\in A$ indre punkt. 
Den partielt afledte af f i retning af enhedsvektoren i er: $\vec{e}_{i}=(0,...,0,1,0,...,0)$ 
er den retningsafledte i retning $\vec{e}_{i}$.

$$\frac{\delta f}{\delta x_{i}}=f'(\vec{a};\vec{e}_{i})$$
Dette gør det meget let at regne da man blot kan differentiere den ene variabel og derefter den anden variabel.
### Eksempel
$f(x,y)=x^{2}+xy^{3}+sin(xy)$
$$\frac{df}{dx}(x,y)=2x+y^{3}+y \cos{xy}$$
$$\frac{df}{dy}(x,y)=3xy^{2}+x \cos{xy}$$


# Retningsafledte
## Definition
$f:A \subset \mathbb{R}^{n}$ hvor $\vec{a} \in A$ er et indre punkt.
Den retningsafledte, (dvs differentialkvotienten) af f i $a$, i retning $\vec{r}$ defineres ved at se på f på linjen der går gennem $\vec{a}$ i retning $\vec{r}$. 

Vi kalder parametren for $h\rightarrow \vec{a}+h \vec{r}$ og funktionen $g(h)=f(a+h \vec{r})$.
Den retningsafledte af f i $\vec{a}$ i retning $\vec{r}$ er $$f'(\vec{a};\vec{r})=g'(0)$$
Indre: $\vec{a} \in A$ er vigtigt at det er defineret som et indre tal da det medfører at g er defineret i et åbent interval omkring 0, så vi kan definere $g'(0)$.
## Anden definition
$f'(a,\vec{r})=\lim_{h \to0} \frac{f(a+h \vec{r})-f(a)}{h}=\lim_{h \to0} \frac{g(h)-g(a)}{h}=g'(0)$

# Gradienten
Man kan [[#Sætning 2.24 (fortsat)|differentiere]] to akser og så sætte dem sammen som en vektorer i ens koordinatsystem. Denne regel gælder ikke generelt, men kun en gang imellem.
## Definition
Gradienten for f i $\vec{a}$ er vektoren $\nabla f(\vec{a})=\frac{df}{dx_{1}}(\vec{a}),..., \frac{df}{dx_{n}}(\vec{a})$.

# Grænseværdier
## Definition
$f:A \to \mathbb{R},A \subset \mathbb{R}^{n}$ hvor $\vec{a}$ fortætningspunkt=akkumulationspunkt[^2]
Vi siger $\lim_{x\to \vec{a}}f(\vec{x})=L$ f har grænseværdien L for $\vec{x}$ gående mod $\vec{a}$.
Hvis der for alle $\epsilon>0$ findes et $\delta>0$ så $x \in A$ og $0<||\vec{x}-\vec{a}||<\delta$[^3] $\Rightarrow |f(\vec{x})-L|<\epsilon$

Husk: $||\vec{x}||=\sqrt{x_{1}^{2}+...+x_{n}^{2}}$.
## Regneregler
$\lim(f(\vec{x})\pm g(\vec{x}))=\lim f(\vec{x})\pm \lim g(\vec{x})$ de har alle samme grænse.
$\lim \frac{f(\vec{x})}{g(\vec{x})}= \frac{\lim f(\vec{x})}{\lim g(\vec{x})}$, hvis $\lim g(\vec{x})\neq0$.

## Sætning 2.24 (fortsat)
Hvis $h:\mathbb{R}\to \mathbb{R}$ er en funktion af en variabel.
$\lim_{\vec{x}\to\vec{a}}h(f(\vec{x}))=h(\lim_{\vec{x}\to\vec{a}})f(\vec{x})$ hvis h er kontinuert, $L=\lim_{\vec{x}\to\vec{a}}f(\vec{x})$.
Og derfor kan vi finde $\lim_{\vec{x}\to\vec{a}}x_{j}=a_{j}$, hvor $\vec{x}=(x_{1},...,x_{n})$ og $\vec{a}=(a_{1},...,a_{n})$.

### Eksempel
$\lim_{(x,y,z)\to(0,0,\pi)}sin(xy+z)=$ da sin er kontinuert $=sin(0*0+\pi)=\sin{\pi}=0$

### Eksempel
Findes $\lim_{(x,y)\to(0,0)} \frac{2xy}{x^{2}+y^{2}}$?
Vi kan dele den op i dens to variable.
$f(x,0)=\frac{0}{x^{2}}=0$ og $f(0,y)=\frac{0}{y^{2}}=0$
Vi går altså mod grænseværdierne for både x og y retningen.

# Kontinuert
En funktion er kontinuert når værdien $\vec{a}$ går mod grænseværdien $\vec{x}$.
## $C^{1}$ 
Vi siger at en funktion er $C^{1}$ når de partielt aflede er kontinuerte.
man kan skrive 
$f'(\vec{a};\vec{r})=\nabla f(\vec{a})*\vec{r}$. prik produkt.
### Definition
Hvis f er defineret på en åben mængde A (alle punkter er indre, dvs at randen ikke er en del af mængden) da er f $C^{1}$ hvis alle de partielt afledte er kontinuerte på A.
Hvis f er $C^{1}$ er f specielt kontinuert.
## Sætning 2.57
Hvis f er $C^{1}$ da er $f'(\vec{a};\vec{r})=\nabla f(\vec{a})\cdot\vec{r}$.

## Sætning 2.58 (Geometrisk fortolkning af gradient)
Hvis f er $C^{1}$ så er $\nabla f(\vec{a})$ i retningen hvor f vokser hurtigst og dens længde er den retningsafledte i den regning $f'(\vec{a};\vec{u})$ hvor u er en enhedsvektor i den retning f vokser hurtigst i.
### Bevis
$f'(\vec{a};\vec{u})=\nabla f(\vec{a})\cdot \vec{u}=||\nabla f(\vec{a})|| ||\vec{u}||\cos{\theta}$
Og kun hvis $\theta=n \pi$ så bliver det $\leq||\nabla f(\vec{a})||$

## Definition 2.32 (Kontinuitet)
f siges at være kontinuert i $\vec{a}$ hvis $\vec{a}$ er isoleret eller hvis $f(\vec{x})\rightarrow f(\vec{a})$ når $\vec{x}\rightarrow \vec{a}$.
Dvs. $\lim_{\vec{x}\to\vec{a}} f(\vec{x})=f(\vec{a})$.
Hvis f er kontinuert i alle punkter i $D_{f}$ kaldes den kontinuert.

## Sætning 2.33 (Regneregler for kontinuitet)
Hvis f,g er kontinuerte i $\vec{a}$ da er
$f+g,f*g,f-g$ kontinuerte i $\vec{a}$.
$\frac{f}{g}$ er kontinuert i $\vec{a}$, hvis $g(a)\neq0$.

## Sætning 2.34
$f_{1},...,f_{n}$ kontinuerte i $\vec{a}\in \mathbb{R}^{m}$ g er kontinuert i $(f_{1}(\vec{a}),...,f_{n}(\vec{a}))$ da er $h(x)=g(f_{1}(x),...,f_{n}(x))$ kontinuert i $\vec{a}$.



[^1]: Noget som er nemt at tjekke. Beskriver differentiabilitet for funktioner af flere variabler. Det er normalt svært at vise at en funktion af flere variabler er differentiabel.
[^2]: Dette er meget vigtigt, Referer til fodnote tre.
[^3]: Der er for alle $\delta$, et $\vec{x}$ som opfylder det.