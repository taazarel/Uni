# 9.1
Lad $T_{1}:\mathbb{P}_{3}\to \mathbb{P}_{3}$ være givet ved $T_{1}(p)=p(1)$.
## (a) 
Vis at $T_{1}$ er lineær

Givet at $p,q \in \mathbb{P}_{3}$ og $r \in \mathbb{R}$.
$T_{1}(p+q)=(p+q)(1)=p(1)+q(1)=T_{1}(p)+T_{1}(q)$.
$T_{1}(rp)=(rp)(1)=r(p(1))=rT_{1}(p)$.

## (b)
Hvad er matricen for $T_{1}$ relativ til den ordnede basis $B=[1,x,x^{2},x^{3}]$ for $\mathbb{P}_{3}$ og basen $B'=[1]$ for $\mathbb{R}$.
$$A=\left[[T_{1}(\vec{u_{1}})]_{B'}\space[T_{1}(\vec{u_{2}})]_{B'}\space [T_{1}(\vec{u_{3}})]_{B'}\space [T_{1}(\vec{u_{4}})]_{B'}\right]=\left[
\begin{array}{}1  & 1 & 1 & 1
\end{array}
\right]$$

## (c)
Lad nu a være et vilkårligt reelt tal og definer $T_{a}(p)=p(a)$. Find matricen for $T_{a}$ relativ til de samme baser som i (b)

$$A=\left[[T_{1}(\vec{u_{1}})]_{B'}\space[T_{1}(\vec{u_{2}})]_{B'}\space [T_{1}(\vec{u_{3}})]_{B'}\space [T_{1}(\vec{u_{4}})]_{B'}\right]=\left[
\begin{array}{}1 & a & a^{2} & a^{3}
\end{array}
\right]$$

# 9.2
Lad $B=[1,x,x^{2},x^{3}]$. Det må bruges uden bevis at B er en basis for $\mathbb{P}_{3}$.
## (a)
Vis at $B_{a}=[1,x-a,(x-a)^{2},(x-a)^{3}]$ er en basis for $\mathbb{P}_{3}$ for ethvert $a \in \mathbb{R}$.

$(x-a)^{2}=(x-a)(x-a)=x^{2}+a^{2}-2ax$$(x-a)^{3}=(x^{2}+a^{2}-2ax)(x-a)=x^{3}+a^{2}x-2ax^{2}-a^{3}-ax^{2}+2a^{2}x$$(x-a)^{3}=x^{3}-a^{3}+3(-ax^{2}+a^{2}x)$
$B_{a}$ har altså både anden og tredje grads led. Dette gør det muligt at danne en given vektor gennem lineærkombination.

## (b)
Find en formel for basisskiftmatricen for at skrifte fra $B_{a}$ til $B$.

$P=\left[[\vec{u}_{1}']_{B},[\vec{u}_{2}']_{B},[\vec{u_{3}}']_{B},[\vec{u_{4}}']_{B}\right]=\left[\begin{array}{}1 & -a & a^2  & -a^3 \\ 0 & 1 & -2a & 3a^2 \\ 0 & 0 & 1 & -3a \\ 0 & 0 & 0 & 1\end{array}\right]$

# 9.3
For $A,B \in \mathbb{M}_{2,2}$ defineres kommutatoren $$[A,B]=AB-BA \in \mathbb{M}_{2,2}$$ I denne opgave vil vi også skrive $K_{B}(A)=[A,B]$ når vi tænker på B som fastholdt og $A\rightarrow K_{B}(A)$ som afbildning $\mathbb{M}_{2,2}\to \mathbb{M}_{2,2}$. 
## (a)
Vis at $K_{B}:\mathbb{M}_{2,2}\to \mathbb{M}_{2,2}$ er lineær for ethvert $B \in \mathbb{M}_{2,2}$.

Lad $A,B \in \mathbb{M}_{2,2}$ og $r \in \mathbb{R}$.
$K_{B}(A+C)=[A+C,B]=(A+C)B-B(A+C)=AB-BA+CB-BC$$=(AB-BA)+(CB-BC)=[A,B]+[C,B]=K_{B}(A)+K_{B}(C)$
Den additive lov er altså god nok.
Nu kan vi tjekke den homogene lov.$K_{B}(rA)=[rA,B]=rAB-BrA=r(AB)-r(BA)$
$=r(AB-BA)=r[A,B]=r(K_{B}(A))$

Siden vi valgte en arbitrer matrice og skalarkoefficient så må dette gælde for ethvert $B \in \mathbb{M}_{2,2}$.
## (b)
Beskriv $ker(K_{B})$ når $B=\left[ \begin{array}{cc}a & 0 \\ 0 & b\end{array}\right]$ for $a,b \in \mathbb{R}$. (Vink: svaret afhænger af om $a=b$ eller $a \neq b$.)

$ker(K_{B})=\{A,B \in \mathbb{M}_{2,2}|K_{B}(A)=\left[\begin{array}{}0 & 0 \\ 0 & 0\end{array}\right] \}\subseteq \mathbb{M}_{2,2}$
Hvor $A=\left[\begin{array}{}c_{11} & c_{12} \\ c_{21} & c_{22}\end{array}\right]$

### Hvis $a=b$
$AB-BA=\left[\begin{array}{}ac_{11} & bc_{12} \\ ac_{21} & bc_{22}\end{array}\right]=\left[\begin{array}{}0 & 0 \\ 0 & 0\end{array}\right]$ hvis $a=b=0$

### Hvis $a \neq b$
$AB-BA=\left[\begin{array}{}ac_{11} & bc_{12} \\ ac_{21} & bc_{22}\end{array}\right] \neq \left[\begin{array}{}0 & 0 \\ 0 & 0\end{array}\right]$ da $a \neq b = 0$ medmindre $A=\left[\begin{array}{}0 & 0 \\ 0 & 0\end{array}\right]$

Vi kan herfra konkludere at $a=b$ da vores kerne kun kan defineres derved.

## (c)
Vis at $B \in ker(K_{B})$ for ethvert $B \in \mathbb{M}_{2,2}$, og brug dimensionsformlen til at konkludere at $K_{B}$ ikke er surjektiv.

$K_{B}(B)=[B,B]=BB-BB=\left[\begin{array}{}0 & 0 \\ 0 & 0\end{array}\right]$
Dette opfylder definitionen for $ker(K_{B})$.

$dim(\mathbb{M}_{2,2})=2 \times 2$
$rang(K_{B})\leq 2$

Da rang af operatoren og dimensionen af codomænet ikke er det samme kan vi konkludere at $K_{B}$ ikke er surjektiv gennem dimensionsformlen. Den er heller ikke injektiv da vores domæne og codomæne er ens.
