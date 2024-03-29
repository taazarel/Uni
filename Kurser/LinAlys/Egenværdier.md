# §8 i Messer
- Egenværdier
- Egenvektorer
- Egenrum
## Definition 8.1 (Egenvektor)
Lad $T:V \to V$ være en lineær operator. En egenværdi for T er et $\lambda \in \mathbb{R}$ så der findes... :: $\vec{v}\in V \backslash \{\vec{0} \}$, med $T(\vec{v})=\lambda \vec{v}$. Da er $\vec{v}$ en egenvektor hørende til $\lambda$, som er egenværdien.[^1]
<!--SR:!2023-01-15,3,250-->

### Specialtilfælde
Givet $V=\mathbb{R}^{n}$ så kan egenvektoren defineres som... :: $A \vec{v}=\lambda \vec{v}\Rightarrow A \vec{v}=\lambda I \vec{v}\Rightarrow A \vec{v}-\lambda I \vec{v}=\vec{0}\Rightarrow (A-\lambda I)\vec{v}=\vec{0}$.
<!--SR:!2023-01-17,4,276-->

Egenvektorer og egenværdier kan beskrives intuitivt som... :: alle vektorer som bliver på deres eget span efter en transformation. De bliver blot skaleret som var der brugt en skalar, vi kalder denne skalar for egenværdien og betegner den $\lambda$.
<!--SR:!2023-01-16,4,272-->

## Sætning 8.2 (Egenværdi)
$\lambda \in \mathbb{R}$ er en egenværdi for $A \in \mathbb{M}_{n,n}\Leftrightarrow$ :: $det(A-\lambda I)=0$.
<!--SR:!2023-01-16,4,272-->

## Sætning på side 335
For $A \in \mathbb{M}_{n,n}$ er $p:\mathbb{R}\to \mathbb{R}$, polynomiet $p(\lambda )=det(A-\lambda I)$ et polynomium af grad n. Og er skrevet som... :: $p(\lambda )=\lambda ^{n}+c_{n-1}\lambda ^{n-1}+...+c_{0}$.
<!--SR:!2023-01-16,4,270-->

## §8.2 At finde egenværdier for en operator
V har end. dim. Vælg så en ordnet basis $B=[\vec{v_{1}},...,\vec{v_{n}}]$ lad $A \in \mathbb{M}_{n,n}$ være matricen for T, referende til B. Vi kan herved skrive $[T(\vec{v})]_{B}=A [\vec{v}]_{B}$ for alle $\vec{v}\in V$. Vi finder egenværdierne ved... :: $p(\lambda )=det(\lambda I-A)=\lambda ^{n}+c_{n-1 }\lambda ^{n-1}+...+c_{0}$  Så er rødderne egenværdierne.
<!--SR:!2023-01-17,4,276-->

## Definition 8.4
$A,A' \in \mathbb{M}_{n,n}$ similære hvis $A'=P^{-1}AP$. Så er $det(A'-\lambda I)=...$:: $det(A-\lambda I)$.
<!--SR:!2023-01-16,3,256-->

## Definition 8.9
V har end. dim. $T:V \to V$ er lineær. Så er det karakteristiske polynomie for T... :: $=det(\lambda I-A)=(-1)^{n}det(A-\lambda I)$.
<!--SR:!2023-01-15,3,250-->

## Sætning 8.8
Similære matricer har samme... :: karakteristiske polynomier/Determinanter af $det(A-\lambda I)=det(A'-\lambda I)$.
<!--SR:!2023-01-16,4,272-->

## Sætning 8.7 (Om sporet/track af matricer)
For alle $A,B \in \mathbb{M}_{n,n}$
1. $tr(A+B)=...$
2. $tr(rA)=...$
3. $tr(AB)=...$
4. $tr(P^{-1}AP)=...$
?
1. $tr(A)+tr(B)$
2. $r \cdot tr(A)$
3. $tr(BA)$
4. $tr(A)$
<!--SR:!2023-01-17,4,276-->

# Messer §8.3+8.4 (Diagonalisering)
## Sætning 8.13
Givet $B=[\vec{u_{1}},...,\vec{u_{n}}]$, vil en ordnet basis baseret på egenvektorer findes hvis $T(\vec{u_{i}})=\lambda_{i}\vec{u_{i}}$ opgør en række i matricen bliver den diagonaliserede basis... :: $$A=\left[\begin{array}{cccc}\lambda_{1} & 0 & ... & 0 \\ 0 & \lambda_{2} & ... &0 \\ \vdots & \vdots & \vdots & \vdots \\ 0 & 0 & ... & \lambda_{n}\end{array}\right] $$hvor $A \in \mathbb{M}_{n,n}$ er den diagonaliserede basis.
<!--SR:!2023-01-16,3,256-->
### Konsekvens af diagonaliserbar base
Givet en ordnet basis $B=[u_{1},...,u_{n}]$ en lineær transformation $T:V \to V$ og $T(\vec{u_{i}})=\lambda_{i}\vec{u_{i}}$. Bliver det karakteristikske polynomie $det(\lambda I-A)=...$:: $$\left[
\begin{array}{cccc}
\lambda -\lambda_{1} & 0 & ... & 0 \\ 
0 & \lambda -\lambda_{2} & ... & 0 \\ 
\vdots & \vdots & \vdots & \vdots \\ 
0 & ... & 0 & \lambda - \lambda_{n}
\end{array}
\right] =(\lambda -\lambda_{1})...(\lambda -\lambda_{n})$$Her er alle rødder reelle og $dim(V)=n$.

### Multiplicitet
Multiplicitet af rødder er blot hvor mange gange de opstår i det karakteristiske polynomie. Så givet $p(\lambda )=(\lambda -k)^{n}$ vil lambda have en rod som er k med en multiplicitet på... :: n da denne rod er gentaget n gange i dens potensgrad.
<!--SR:!2023-01-16,4,272-->

### Egenrum
Egenrummet som hører til egenværdien $\lambda$ er defineret som... :: $E_{T}(\lambda)=span \{\vec{u_{i}}|\lambda_{i}=\lambda  \}$
<!--SR:!2023-01-15,3,252-->
Hvis $V=\mathbb{R}^{n}$ og $T(\vec{v})=A \vec{v}$ findes $E_{A}(\lambda_{j})=ker(\lambda_{j}I-A)$ ved at... :: Rækkereducere $(\lambda_{j}-A)$, og så tage dimensionen, eller antallet af nulrækker.
<!--SR:!2023-01-14,1,236-->

## Sætning 8.14
Lad $T:V \to V$ have endelig dimension. $\lambda_{1},...,\lambda_{k} \in \mathbb{R}$. Forskellige egenværdier for $T,\vec{u_{1}},...,\vec{u_{k}}\in V$ tilhørende egenvektorerne $T(\vec{u_{i}})=\lambda_{i}\vec{u_{i}}$. Da vil basen bestående af $B=[\vec{u_{1}},...,\vec{u_{k}}]$ være... :: lineært uafhængig.
<!--SR:!2023-01-15,3,252-->

## Sætning 8.16
Hvis $dim(V)=n$ og $T:V \to V$ har n'te forskellig egenværdier så... :: er T diagonaliserbar.[^2]
<!--SR:!2023-01-14,1,236-->

## Sætning 8.15
For at finde en basis for egenværdier skal vi først finde for egenrum. Givet $T:V \to V$ har egenværdierne $\lambda_{1},...,\lambda_{k}$ vil T være diagonaliserbar hvis og kun hvis $dim(V)=...$ :: $dim(E_{T}(\lambda_{1})+...+dim(E_{T}(\lambda_{k})))$.
<!--SR:!2023-01-15,3,252-->

## Praksis Diagonalisering
Der er en række trin til at lave en diagonaliseret basis.
De er...
?
- Find alle forskellige egenværdier
- For hver egenværdi $\lambda_{i}$ skal man beregne $dim(E_{T}(\lambda_{i}))$.
- Hvis færre end n vektorer kan findes er matricen ikke diagonaliserbar. Hvis man finder n baser bruger man dem som søjler i P matrix. Som man så kan bruge sammen med A matricen(transformationen) til at finde A'.
- A' vil blive en diagonal matrice som har dens diagonale indgange som egenværdierne
Hvis $dim(E_{T}\lambda_{i})=$ multiplicitet af $\lambda_{i}$ som rod i det karakteristiske polynomie. Og alle rødder er reelle er $dim(V)=grad(p(\lambda ))=\sum_{i=1}^{k} \text{ multiplicitet af }\lambda_{i}=\sum_{i=1}^{k}dim(E_{T}(\lambda_{i}))$.
# §8.4 Symmetriske matricer & Operatorer
## Definition af symmetriske matricer
En matrice givet ved $A \in \mathbb{M}_{n,n}$ er symmetrisk hvis $A=A^{t}$.
## Definition af symmetriske operatorer
Givet operatoren $T:V \to V$ lineær, og V er et indre produkt rum. Vil T være symmetrisk hvis... :: $\langle T(\vec{v}),\vec{w}\rangle =\langle \vec{v},T(\vec{w})\rangle$ for alle $\vec{v},\vec{w}\in V$
<!--SR:!2023-01-15,2,232-->
## Sætning 8.21
Givet $T:V \to V$ symmetrisk, V indre produkt rum, $B=[\vec{u_{1}},...,\vec{u_{n}}]$ ortonormal basis og $A \in \mathbb{M}_{n,n}$ er matricen for T relativ til B. Da vil... :: $A^{t}=A$. Altså da Operatoren er symmetrisk kan vi definere den som en symmetrisk matrix.
<!--SR:!2023-01-16,4,272-->
## Sætning 8.23
Givet $A \in \mathbb{M}_{n,n}$ er symmetrisk Da er alle rødder... :: i det karakteristiske polynomium reelle.
<!--SR:!2023-01-16,3,256-->
### Konsekvens
Givet V er et indre produkt rum, T er symmetrisk på V så er alle rødder... :: i det karakteristiske polynomium for T reelle.
<!--SR:!2023-01-17,4,276-->

## Sætning 8.24 (Spektralsætningen)
Lad V være et end. dim. indre produkt rum. T er symmetrisk på V. Da findes en... :: Ortonormal basis B bestående af [[Egenværdier#Definition 8.1 (Egenvektor)|Egenvektorer]].
<!--SR:!2023-01-15,3,250-->

# Fodnoter
[^1]: Kan også skrives som $A \vec{v}=\lambda \vec{v}\Rightarrow (A-\lambda I)\vec{v}=\vec{0}$ givet $V = \mathbb{R}^{n}$.
[^2]: Vi antager her at egenværdierne er reelle og forskellige fra hinanden.