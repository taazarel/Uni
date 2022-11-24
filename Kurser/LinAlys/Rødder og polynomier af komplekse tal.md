#forelæsning 
Begyndelsesdato: Kl. 08:12  Den 22-11-2022   Uge-47
# Programmet
- n-k rødder af $z \in \mathbb{C}$. (TL 3.4)
- Polynomier (TL 1.5)

## Definition 3.5.1
lad $z \in \mathbb{C},n \in \mathbb{N}$ Da er en n-te rod af z skrevet som... :: $w^{n}=z \text{ hvor }w \in \mathbb{C}$.[^1]

## Sætning 3.5.2
lad $z \in \mathbb{C}\backslash \{ 0\},n \in \mathbb{N}$ da vil z have disse rødder... :: n forskellige n-te rødder skrevet $w_{0},...,w_{n-1}\in \mathbb{C}$.
Givet $z,w \in \mathbb{C}$ og $w^{n}=z,z=re^{i \theta }$ så bliver den bestemte rod $w_{k}=$... :: $r^{\frac{1}{n}}e^{i \frac{\theta+2\pi k}{n}}$.

Nogle smutveje til at finde rødder af et kompleks tal er
?
At udregne $w_{k}=r^{\frac{1}{n}}e^{i \frac{\theta+2\pi k}{n}},k=0,n-1$
Omregne $w_{k}$ til en reel og imaginær del. $w_{k}=r^{\frac{1}{n}}e^{\frac{i \theta }{n}}(e^{i \frac{2\pi}{n}})^{k}$ 
At bruge $w_{k}=w_{0}\cdot (e^{i \frac{2\pi}{n}})^{k}$ 

## Sætning 3.4.5 (Polynomiers løsning i det komplekse rum)
At finde løsningen til et andengradspolynomie i det komplekse talrum er lidt anderledes. Givet $az^{2}+bz+c=0, z \neq 0$ så er løsningerne... :: $z= \frac{-b\pm\sqrt{d}}{2a}$ 

Disse ting er anderledes ved $az^{2}+bz+c=0 \in \mathbb{C}$...
?
$d>0$ har vi to forskellige reelle rødder[^2]
$d=0$ har vi en reel rod
$d<0$ har vi to ikke reelle rødder.

Givet $az^{2}+bz+c=0,d=0$ så bliver $z=$... :: $\frac{-b}{2a}$.

## Definition 1.5 (Polynomier)
Et komplekst polynomie $p:\mathbb{C}\to \mathbb{C}$ bliver skrevet på formen... :: $$p(z)=a_{n}z^{n}+a_{n-1}z^{n-1}+...+a_{0}z^{0},n \in \mathbb{N} \Rightarrow \sum_{k=0}^{n}a_{k}z^{k}$$
## Definition RM (Reelle polynomier)
Et reelt polynomie $f:\mathbb{R}\to \mathbb{R}$ skrives som... :: $$f(x)=a_{n}x^{n}+...+a_{0}x^{0},n \in \mathbb{N},a_{n}\in \mathbb{R}$$
### Definition (Grad af polynomier)
Graden af et polynomie p skrives som... :: $grad(p)$ er den største $n \in \{ 0,1,...\} \text{ så }a_{n} \neq 0$.

## Regneregler med polynomier
Produktet af to polynomier $p,q:\mathbb{C}\to \mathbb{C}$ med graderne $grad(p)=n,grad(q)=m$ skrives som ... :: $p(z)q(z)=(a_{n}b_{m})z^{n+m}+(a_{n}b_{m-1}+a_{n-1}b_{m})z^{n+m-1}$ Et polynomie til graden $grad(p \cdot q)=grad(p)+grad(q)$.

### Sætning 1.5.2 (Division af polynomier med rest)
Givet $p,q \in \mathbb{C}\text{ og }q \neq 0\text{ og } k=\frac{p}{q}$ så findes polynomiet $k(z)\text{ og }r(z)$ så $p(z)=$... :: $k(z)q(z)+r(z)$ med $grad(r)<grad(q)$.

Vektorer i $\mathbb{R}^{n}$ kan skrives som:
afstand til $\vec{0},||\vec{v}||=\sqrt{\vec{v}\cdot \vec{v}}$.
Afstand fra $\vec{v}$ til $\vec{w},||\vec{v}-\vec{w}||$
Vinkel $\vec{v},\vec{w} \neq 0$ og $\theta =\cos^{-1}{\frac{\vec{v}\cdot\vec{w}}{||\vec{v}||\cdot||\vec{w}||}}$
Projektion $proj_{\vec{u}}(\vec{v})= \frac{\vec{u}\cdot\vec{v}}{\vec{u}\cdot \vec{u}}$ 
Ortogonalitet $\vec{u}\cdot \vec{v}=0$
Oversat tilet V indre produkt rum er de...
?
norm $||\vec{v}||=\sqrt{\langle \vec{v},\vec{v}\rangle }$
Afstand $\vec{v} \text{ til }\vec{w}$ $||\vec{v}-\vec{w}||$
Vinkel $\vec{u},\vec{v}\in V \backslash 0$ så er $\theta =\cos^{-1}{\frac{\langle \vec{u},\vec{v}\rangle}{||\vec{u}||||\vec{v}||}}$
Projektion $proj_\vec{u}(\vec{v})= \frac{\langle\vec{v},\vec{u}\rangle}{\langle \vec{u},\vec{u}\rangle }\vec{u}$
Ortogonalitet $\langle \vec{u},\vec{v}\rangle =0$

## Sætning 4.11 Caudiy Schwarz ulighed
Givet $\vec{u},\vec{v}\in V$ da kan vi vise en ulighed som... :: $|\langle \vec{u},\vec{v}\rangle| \leq ||\vec{u}||\cdot ||\vec{v}||$ altså $-(||\vec{u}||\cdot ||\vec{v}||)\leq \langle \vec{u},\vec{v}\rangle \leq ||\vec{v}||\cdot ||\vec{u}||$
### Korollar
For $\frac{\langle \vec{u},\vec{v}\rangle }{||\vec{u}||\cdot ||\vec{v}||}\in [-1,1]$ så er $\theta =$... :: Veldefineret.

## Sætning 4.12
V er et indre produkt rum $\vec{v},\vec{u}\in V$ og $a \in \mathbb{R}$
1. Hvis $||\vec{u}||\geq 0$ og $||\vec{u}||=0$ så er...
2. $||a \vec{u}||=...$
3. $||\vec{u}+\vec{v}||\leq ...$
?
1. $\vec{u}=\vec{0}$
2. $|\vec{a}|\cdot ||\vec{u||}$
3. $||\vec{u}||+||\vec{v}||$ Denne hedder også trekantsuligheden ![[Rødder og polynomier af komplekse tal 2022-11-24 08.33.27.excalidraw]]
### Korollar
For $f,g \in C_{[a,b]}$ så er $$\sqrt{\int_{a}^{b} (f(x)+g(x))^{2}dx}\leq ...$$ :: $$\sqrt{\int_{a}^{b} f(x)^{2}dx}+\sqrt{\int_{a}^{b} g(x)^{2}dx}$$
## Definition 4.16
Lad V være et indre produkt rum. Vektorfamilien $\vec{u_{1}},...,\vec{u_{n}}\in V$ er ortogonale hvis.... :: $\langle \vec{u_{i}},\vec{u_{j}}\rangle =0$ for $i \neq j$ og $\langle \vec{u_{i}},\vec{u_{j}}\rangle =1$ for $i=j$.[^3]
Vi kan skrive skalaren $r_{i}=...$ :: $\frac{\langle \vec{u_{i}},\vec{v}\rangle}{\langle \vec{u_{i}},\vec{u_{i}}\rangle }= \text{ hvis ortonormal } = \langle \vec{u_{i}},\vec{v}\rangle$.

## Sætning 4.17
Hvis $\vec{u_{1}},...,\vec{u_{n}}\in V \backslash \{\vec{0} \}$ er ortogonale medfører det at familien er.... :: Lineært uafhængige. Men ortogonalitet er lettere at tjekke.
### Korollar "Ortonormal basis" (ONB)
$\vec{e_{1}},...,\vec{e_{n}}\in \mathbb{R}^{n}$ med prikprodukter. Hvis V har en endelig $dim \{ V\}$ så vil ... :: vi finde en basis $\vec{u_{1}},...,\vec{u_{n}}\in V$ gennem en Gram Schmidt Proces.

## Sætning 4.20 (Konstruktion af ONB)
Givet $\vec{u_{1}},...,\vec{u_{n}}\in V$ er en basis, konstruerer vi ONB $\vec{e_{1}},...,\vec{e_{n}}\in V$ og kan definere... :: $\vec{e_{1}}= \frac{1}{||\vec{u_{1}}||}\vec{u_{1}}$ og $v_{2}=\vec{u_{2}}-\langle \vec{u_{2}},\vec{e_{1}}\rangle \vec{e_{1}}$ så kan vi definere $\vec{e_{2}}= \frac{1}{||\vec{v}||}\vec{v_{2}}$.
De generelle $\vec{v_{k}},\vec{e_{k}}$ kan skrives som... :: $\vec{v_{k}}=\vec{u_{k}}-\langle \vec{u_{k}},\vec{u_{1}}\rangle \vec{e_{1}}-...-\langle \vec{u_{k}},\vec{e_{k-1}}\rangle \vec{e_{k-1}}$. og $e_{k}= \frac{1}{||\vec{v_{k}}||}\vec{v_{k}}$. $v_{k}$ kan omdefineres til $$\vec{v_{k}}=\vec{u_{k}}-\sum_{j=1}^{k-1}\langle \vec{u_{k}},\vec{e_{j}}\rangle \vec{e_{j}}$$


## Kig på senere
### Eksempel 3.4.3 
For at se hvordan man finder en rod.
### Eksempel 1.5.1
For at se hvordan man dividerer polynomier
### Eksempel på side 181
For at se konstruktion af en ONB
# Fodnoter
[^1]: Der kan både være flere en en rod, eller ingen gyldige rødder. Altså er rødderne ikke entydige.
[^2]: Diskriminanten er stadigvæk $d=b^{2}-4ac$
[^3]: Messer $S \subseteq V$ er ortogonal.