# Dagsplan

Tirsdag
1. 6.1 RM
2. 6.3 RM (Sammenhæng til matricer)
3. 6.2 RM
Torsdag
1. 6.5 RM
2. 6.6 RM
3. 6.7 RM
# Messer §6.1
## Definition 6.1

Givet er V og W vektorrum og funktionen $T:V \to W$ er lineær. 
Hvis for alle $\vec{v},\vec{w},\in V,r \in \mathbb{R}$ Så kan vi definere disse:
$T(\vec{v}+\vec{w})=$...
$T(r \vec{v})=$...
?
$T(\vec{v})+T(\vec{w})$ Additiv lov
$rT(\vec{v})$ Homogen lov

#### Eksempel
$A \in \mathbb{M}_{m,n}$ og $\mu _{A}:\mathbb{R}^{n}\to \mathbb{R}^{m}$ $\mu_{A}(\vec{v})=A \vec{v}$. Givet at $A(\vec{v}+\vec{w})=A\vec{v}+A\vec{w}$ og $A(r \vec{v})=r A\vec{v}$ så må $\mu_{A}$ være... :: $\mu_{A}$ er lineær.

### Sætning 6.2

Lad $T:V \to W$ være lineær. Da er de tre aksiomer:
Om nulvektoren...
Negativ vektor...
Og en familie af skalarer...
?
$T(\vec{0})=\vec{0}$ (i)
$T(-\vec{v})=-T(\vec{v})$ (ii)
$T(r_{1}\vec{v_{1}}+...+r_{n}\vec{v_{n}})=r_{1}T(\vec{v_{1}})+...+r_{n}T(\vec{v_{n}})$. (iii)

### Sætning 6.3
Lad $T,T':V \to W$ være lineær, og lad $S=\{\vec{v_{1}},...,\vec{v_{n}} \}\in V$ være udspændende. Hvis $T(\vec{v_{i}})=T'(\vec{v_{i}})$ for alle i, så er $T=$... :: $T'$ Altså har entydighed for disse funktioner.

# Messer §6.3 (Sammenhæng af lineære afbildninger og matricer)
### Sætning 6.11 (Specialtilfælde af 6.12)

Lad $T:\mathbb{R}^{n}\to \mathbb{R}^{m}$ være lineær, da findes 
$A \in \mathbb{M}_{m,n}$ så $T=$...
Da er præcis én A j'te søjle i A...
?
$\mu_{A}\Rightarrow T(\vec{v})=A\vec{v}$ for alle $\vec{v}\in \mathbb{R}^{n}$
som er $T(\vec{e_{j}})\in \mathbb{R}^{m}$ hvor $j=1,...,n$ 

### Sætning 6.12
Lad $T:V \to V'$ være lineær, Givet er to baser $B,B'$. Da findes entydig $A \in \mathbb{M}_{n,m}$ for alle $\vec{v}\in V$ Denne skrives som... :: $[T(\vec{v})]_{B'}=A[\vec{v}]_{B}$ [^1]
En given søjle i matricen $A$ skrives som... :: $[T(\vec{u}_{j})]_{B'}$ 

# Messer §6.2 (Mængdelære)
$X,Y$ er mængder, vi har $f:X \to Y$ funktion. Disse mængder kaldes for ... :: $X=$ domæne/definitionsmængden. $Y=$ codomæne
## Definition
$f:X \to Y$ er injektiv[^2] hvis for alle $x_{1},x_{2}\in X,$ der findes... :: $f(x_{1})=f(x_{2})\Rightarrow x_{1}=x_{2}$ eller $x_{1}\neq x_{2}\Rightarrow f(x_{1})\neq f(x_{2})$.
Værdimængden for $f:X \to Y$ defineres som... :: $f(Y)=\{f(x)|x \in X \}\subseteq Y$.[^3]
# Messer §6.5 (Basis-skift)
#### Specialtilfælde af 6.12
Givet $V=V',T=id_{V}:V \to V$ givet to baser B og B', så er $T(\vec{v})=...$ :: $\vec{v}$

### Sætning 6.16 
Givet er to baser $B,B'$ for $V$. Da findes præcis én $P \in \mathbb{M}_{n,n}$ så for alle $\vec{v}\in V$ hvad er den j'te søjle og $[\vec{v}]_{B}=...$::$P \cdot [\vec{v}]_{B'}$ og den bestemte søjle er $[\vec{u_{j}}']_{B}$

## Basisskift for lin. afbildning.
Lad $T:V \to V$ være en lineær afbildning[^4] Nu kan vi vælge $B=B':A \in \mathbb{M}_{n,n}$ matricen for T i forhold til B bliver så $[T(\vec{v})]_{B}=A[\vec{v}]_{B}$ for alle $\vec{v}\in V$. 
Givet en anden basis B' får $A' \in \mathbb{M}_{n,n}$ matricen for T relativ til B' $[T(\vec{v})]_{B'}=A'[\vec{v}]_{B'}$ 
Basisskift-matricen fra $B'$ til $B$ givet $P \in \mathbb{M}_{n,n}:[\vec{v}]_{B}=P[\vec{v}]_{B'}$
### Sætning 6.19
Da kan A' findes ved...
?
$A'=D^{-1}AP$

# Messer §6.6 (Kerne og Billede)

## Definition 6.20
Lad lineær $T:V \to W$ hvor $V,W$ er vektorrum. 
Definer $ker(T)=...$
Definer $im(T)=...$
?
$\{\vec{v}\in V|T(\vec{v})=\vec{0} \}\subseteq V$
$\{\vec{w}\in W|\vec{w}=T(\vec{v}) \text{ for et }\vec{v}\in V \}\subseteq W$[^5]

## Definition 6.27
Lad $T:V \to W$ være lineær og $im(T)$ er endelig-dimensionalt, så er $rank(T)=...$::$dim(im(T))$.
Lad $T:V \to W$ være lineær og $ker(T)$ er endelig-dimensionalt, så er $mullity(T)=...$::$dim(ker(T))$
#### Sammenhæng med surjektivitet 
Hvis W er endelig-dimensionalt så er $T:V \to W$ surjektiv og $im(T)=$... :: $W$ Da der vil være en værdi på alle W
### Sætning 6.30
Lad T være en operator. T er injektiv hvis... :: $ker(T)=\{\vec{0} \} \Leftrightarrow dim(ker(T))=0$ 
### Sætning 6.28 (Dimensionsformlen)
Lad T være en operator[^6] og V har end. dim. Da har $im(T)$... :: endelig dimension. Da $dim(V)=rang(T)+dim(ker(T))$
#### Korollar
Givet $dim(V)=rang(T)+dim(ker(T))$ så er $rang(T)\leq ...$:: $dim(V),dim(W)$


# Fodnoter
[^1]: Hvor den venstre del er $\mathbb{R}^{m}$ og den højre er $\mathbb{R}^{n}$. Basen er $B=[\vec{u_{1}},...,\vec{u_{n}}]$, altså basen for V. Ser således ud for V': $B'=[\vec{u_{1}}',...,\vec{u_{m}}']$.
[^2]: Injektiv betyder one to one, og skrives injective på engelsk. Surjektiv betyder onto og skrives surjective på engelsk.
[^3]: Dette er billedet. Defineres også som værdimængden.
[^4]: Kaldes også en operator
[^5]: Både kernen og billede er altså underrum.
[^6]: T er defineret på V til W.