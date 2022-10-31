# Delopgave 1
## a
Afgør om polynomierne 
$p_{1}(x)=x^{2}-1,p_{2}(x)=2x^{2}+x,p_{3}(x)=x+1$
er lineært uafhængige i funktionsrummet $\mathbb{F}_{\mathbb{R}}$.
Hvis disse polynomier er lineært uafhængige i $\mathbb{F}_{\mathbb{R}}$, så ville de ingen frie variable have i en række-echelon form, med en vilkårlig polynomie i $\mathbb{F}_{\mathbb{R}}$.
altså:
$r_{1}(x^{2}-1)+r_{2}(2x^{2}+x)+r_{3}(x+1)=ax^{2}+bx+c$, hvor $r_{1},r_{2},r_{3}\in \mathbb{R}$. 
Hvilket vi kan omskrive til tre ligninger med tre ubekendte.
$$
\begin{array}{c}
r_{1}+r_{2}=a \\ r_{2}+r_{3}=b \\ -r_{1}+r_{3}=c
\end{array}
$$
Og derefter skrive som en koefficientsmatrix.
$$\left[
\begin{array}{ccc|c}
1 & 2 & 0 & a \\ 0 & 1 & 1 & b \\ -1 & 0 & 1 & c
\end{array}
\right]\to
\left[
\begin{array}{ccc|c}
1 & 2 & 0 & a \\ 0 & 1 & 1 & b \\ 0 & 0 & -1 & c+a-2b
\end{array}
\right]\to
\left[
\begin{array}{ccc|c}
1 & 2 & 0 & a \\ 0 & 1 & 0 & b+c+a-2b \\ 0 & 0 & 1 & 2b-a-c
\end{array}
\right]$$
$$\to
\left[
\begin{array}{ccc|c}
1 & 0 & 0 & a-2(b+c+a-2b) \\ 0 & 1 & 0 & b+c+a-2b \\ 0 & 0 & 1 & 2b-a-c
\end{array}
\right]\to
\left[
\begin{array}{ccc|c}
1 & 0 & 0 & 2b-a-2c \\ 0 & 1 & 0 & a+c-b \\ 0 & 0 & 1 & 2b-a-c
\end{array}
\right]$$
Vi kan herved se at:
- Der er ingen frie variabler da:
	- $r_{1}=2b-a-2c$
	- $r_{2}=a+c-b$
	- $r_{3}=2b-a-c$
- Derfor må polynomierne være lineært uafhængige i funktionsrummet $\mathbb{F}_{\mathbb{R}}$. 
## b
Vis, at det underrum i $\mathbb{F}_{\mathbb{R}}$, der udspændes af polynomierne i (a) udgøres af alle polynomier af grad højst 2 dvs. af $\mathbb{P}_{2}$ 

Vi kalder $span(p_{1},p_{2},p_{3})=V$. Vi skal herved vise at mængden $V=\mathbb{P}_{2}$, hvor $V,\mathbb{P}_{2} \subseteq \mathbb{F}_{\mathbb{R}}$.
Nu kan vi finde et vilkårligt polynomie af højst 2 grad, dvs. 2 grad: $ax^{2}+bx+c \in \mathbb{P}_{2}$. Hvis det er sandt at V udspænder hele $\mathbb{P}_{2}$ så må der findes $r_{1},r_{2},r_{3} \in \mathbb{R}$ som gør 
$r_{1}(p_{1})+r_{2}(p_{2})+r_{3}(p_{3})=ax^{2}+bx+c$, et sandt udtryk.

Men dette har vi jo netop bevist i (a). Så hermed kan vi se at underrummet som V spanner i $\mathbb{F}_{\mathbb{R}}$ er det samme som alle polynomier af 2 grad, dvs. $V=\mathbb{P}_{2}$.

# Delopgave 2
## a
*Betragt kraftfelterne, afgør om de er konservative og bestem i givet fald en tilhørende potentialfunktion.*

$F_{1}(x,y)=(y,x),F_{2}(x,y)=(-y,x)$
Gradienten til en funktion er givet ved $\nabla V=(\frac{d}{dx}V(x,y), \frac{d}{dy}V(x,y))$. hvis vi kan finde en funktion for denne gradient som giver $F(x,y)=-\nabla V$ så er kraftfeltet konservativt.
For $F_{1}$ kan vi vise dette da en funktion findes som gør dette muligt, nemlig: $V=-xy$
$-\nabla V=(\frac{d}{dx}(-xy), \frac{d}{dy}(-xy))=-(-y,-x)=(y,x)=F_{1}(x,y)$ 
Derfor er $F_{1}$ konservativ.

Vi kan til gengæld ikke finde en fælles stamfunktion for $F_{2}$ som gælder. Da vi har: $F_{2}(x,y)=(-y,x)$
$\int_{}^{}-y dx=-xy+c(y)$ Hvor c er en konstant som kunne være afhængig af y.
$\int_{}^{}xdy=xy+c(x)$ hvor c er en konstant som kunne være afhængig af x.
Her kan vi se at stamfunktionen for den delvist afledte af x, kan ikke være det samme som stamfunktionen for den delvist afledte af y. 
Vi har altså 
$F_{2}(x,y)=(-y,x)\neq -\nabla V$
Og denne er ikke et konservativ kraftfelt.
## b
Lad os først finde de delvist afledte af x,y, og z.
$\frac{dV}{dx}=y+z$, $\frac{dV}{dy}=x+z$, $\frac{dV}{dz}=2az+y+x$.
Herefter kan vi indsætte dette i en gradient.

$-\nabla V=-(y+z,x+z,2az+y+x)=\vec{0}$ 
Så dette må betyde at alle led skal være lig med nul.
Vi kan derfor finde at.
$a= -(\frac{x+y}{2z})$
Og vi kan benytte de andre to koordinater til at finde:
$x=-z$
$y=-z$
Derfor må: $a=-\left(\frac{-2z}{2z}\right)= 1$
Vi finder at $a=1$ har præcist 1 ligevægtspunkt.
# Delopgave 3
## a
Vi skal finde $T_{2}E(v)$ hvor: $E(v)= \frac{mc^{2}}{\sqrt{1- \frac{v^{2}}{c^{2}}}}$.
Vi kan starte med at differentiere $E(v)$ først 1 gang og så differentiere resultatet igen.
For at spare på pladsen viser jeg blot metoden ikke udregningen.
$\frac{dE(v)}{dv}=f'(g(h(v)))\cdot g'(h(v))\cdot h'(v)= \frac{mv}{\left(1-\frac{v^{2}}{c^{2}}\right)^{\frac{3}{2}}}\Rightarrow E'(v)$ 
Hvor $f(v)=\frac{mc^{2}}{g(v)}$, $g(v)=\sqrt{h(v)}$ og $h(v)=1- \frac{v^{2}}{c^{2}}$   
For det første led, og derefter kan vi finde det andet led til at være:
$\frac{dE'v}{dv}=f'(v)\cdot g(h(j(v))) + f(v)\cdot g'(h(j(v)))\cdot h'(j(v))\cdot j'(v)\Rightarrow mc^{2}\frac{c^{2}+2v^{2}}{(c^{2}-v^{2})^{2}\sqrt{1- \frac{v^{2}}{c^{2}}}} \Rightarrow E''(v)$  
Hvor $f(v)=mv$, $g(v)=\frac{1}{h(v)}$, $h(v)=(j(v))^{\frac{3}{2}}$  og $j(v)=1- \frac{v^{2}}{c^{2}}$ .
Nu kan vi samle dette til taylorpolynomiet ved v=0.
$$T_{2}E(v)=mc^{2}+ \frac{0}{1!}(v-0)^{1}+ \frac{m}{2!}(v-0)^{2}\Rightarrow mc^{2}+ \frac{mv^{2}}{2}$$
Vi kan herved se at enheden for dette polynomium er $\frac{m^{2}}{s^{2}}kg$ eller også skrevet som $J$ . Dette passer altså perfekt med newtons kinetiske energi.

## b
For at gøre det let for os selv bruger vi bare forslaget i opgaven, dvs. $m=1, c=300$.
Vi benytter os af Python til at finde taylorpolynomierne af 4 og 10 grad.
$E(0)=mc^{2}=1kg300 \frac{m}{s}^{2}=90000*10^{-6} \frac{m^{2}}{s^{2}}kg$   
$T_{2}E(v)=mc^{2}+ \frac{mv^{2}}{2}=90000+ \frac{v^{2}}{2} \frac{m^{2}}{s^{2}}kg*10^{-6}$ 
$T_{4}E(v)=mc^{2}+ \frac{mv^{2}}{2}+ \frac{mv^{4}}{240000}=90000+ \frac{v^{2}}{2}+ \frac{v^{4}}{240000} \frac{m^{2}}{s^{2}}kg*10^{-6}$
Lad os forkorte det længste led til resultatet.
$T_{10}E(v)=90000+ \frac{v^{2}}{2}+ \frac{v^{4}}{240000}+ \frac{v^{6}}{25920000000}+ \frac{7v^{8}}{18662400000000000}+ \frac{7v^{10}}{1866240000000000000000} \frac{m^{2}}{s^{2}}kg*10^{-6}$

Vi kan se at alle disse polynomier og også $E(v)$ selv skærer ved $90000 J$, så vi vælger dette til vores graf. Vi finder også at 400 til begge sider passer godt da vi satte $c=300$ i programmet.

![[Pointopgave 6.3.b 2.png]]

Ud fra denne figur kan vi se at vi kunne benytte $T_{2}E(v)$ ca. op til $180 \frac{m^{2}}{s^{2}}*10^{-6}$.
Og $T_{10}E(v)$ ser ud til at følge meget nærmere på $E(v)$ så den kan vi godt bruge i vores interval fra (-200,200) og jeg vurderer at den er en god approksimation.
(Jeg forøgede intervallet for at se om $T_{10}E(v)$ fulgtes med $E(v)$, og det gør den, til gengæld ser grafen ikke godt ud, så jeg valgte dette interval)
