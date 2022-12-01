# 9.1
Lad $T_{1}:\mathbb{P}_{3}\to \mathbb{P}_{3}$ være givet ved $T_{1}(p)=p(1)$.
## (a) 
Vis at $T_{1}$ er lineær

Givet at $p,q \in \mathbb{P}_{3}$ og $r \in \mathbb{R}$.
$T_{1}(p+q)=p(1)+q(1)=T_{1}(p)+T_{1}(q)$.
$T_{1}(rp)=rp(1)=rT_{1}(p)$.

## (b)
Hvad er matricen for $T_{1}$ relativ til den ordnede basis $B=[1,x,x^{2},x^{3}]$ for $\mathbb{P}_{3}$ og basen $B'=[1]$ for $\mathbb{R}$.



## (c)
Lad nu a være et vilkårligt reelt tal og definer $T_{a}(p)=p(a)$. Find matricen for $T_{a}$ relativ til de samme baser som i (b)


# 9.2
Lad $B=[1,x,x^{2},x^{3}]$. Det må bruges uden bevis at B er en basis for $\mathbb{P}_{3}$.
## (a)
Vis at $B_{a}=[1,x-a,(x-a)^{2},(x-a)^{3}]$ er en basis for $\mathbb{P}_{3}$ for ethvert $a \in \mathbb{R}$.

## (b)
Find en formel for basisskiftmatricen for at skrifte fra $B_{a}$ til $B$.

# 9.3
For $A,B \in \mathbb{M}_{2,2}$ defineres kommutatoren $$[A,B]=AB-BA \in \mathbb{M}_{2,2}$$ I denne opgave vil vi også skrive $K_{B}(A)=[A,B]$ når vi tænker på B som fastholdt og $A\rightarrow K_{B}(A)$ som afbildning $\mathbb{M}_{2,2}\to \mathbb{M}_{2,2}$. 
## (a)
Vis at $K_{B}:\mathbb{M}_{2,2}\to \mathbb{M}_{2,2}$ er lineær for ethvert $B \in \mathbb{M}_{2,2}$.

## (b)
Beskriv $ker(K_{B})$ når $B=\left[ \begin{array}{cc}a & 0 \\ 0 & b\end{array}\right]$ for $a,b \in \mathbb{R}$. (Vink: svaret afhænger af om $a=b$ eller $a \neq b$.)

## (c)
Vis at $B \in ker(K_{B})$ for ethvert $B \in \mathbb{M}_{2,2}$, og brug dimensionsformlen til at konkludere at $K_{B}$ ikke er surjektiv.