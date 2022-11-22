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


## Kig på senere
### Eksempel 3.4.3 
For at se hvordan man finder en rod.
### Eksempel 1.5.1
For at se hvordan man dividerer polynomier
# Fodnoter
[^1]: Der kan både være flere en en rod, eller ingen gyldige rødder. Altså er rødderne ikke entydige.
[^2]: Diskriminanten er stadigvæk $d=b^{2}-4ac$