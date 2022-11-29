# Dagsplan

1. 6.1 RM
2. 6.3 RM (Sammenhæng til matricer)
3. 6.2 RM

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
### Sætning 6.11

Lad $T:\mathbb{R}^{n}\to \mathbb{R}^{m}$ være lineær, da findes 
$A \in \mathbb{M}_{m,n}$ så $T=$...
Da er præcis én A j'te søjle i A...
?
$\mu_{A}\Rightarrow T(\vec{v})=A\vec{v}$ for alle $\vec{v}\in \mathbb{R}^{n}$
som er $T(\vec{e_{j}})\in \mathbb{R}^{m}$ hvor $j=1,...,n$ 

### Sætning 6.12
Lad $T:V \to V'$ være lineær. Da findes entydig $A \in \mathbb{M}_{n,m}$ for alle $\vec{v}\in V$ Denne skrives som... :: $[T(\vec{v})]_{B}=A[\vec{v}]_{B}$ [^1]
En given søjle i $[T(\vec{v})]_{B}=A[\vec{v}]_{B}$ skrives som ... :: $[T(\vec{v}_{j})]_{B}$ 

# Messer §6.2 (Mængdelære)
$X,Y$ er mængder, vi har $f:X \to Y$ funktion. Disse mængder kaldes for ... :: $X=$ domæne/definitionsmængden. $Y=$ codomæne
## Definition
$f:X \to Y$ er injektiv[^2] hvis for alle $x_{1},x_{2}\in X,$ der findes... :: $f(x_{1})=f(x_{2})\Rightarrow x_{1}=x_{2}$ eller $x_{1}\neq x_{2}\Rightarrow f(x_{1})\neq f(x_{2})$.
Værdimængden for $f:X \to Y$ defineres som... :: $f(Y)=\{f(x)|x \in X \}\subseteq Y$.[^3]


# Fodnoter
[^1]: Hvor den venstre del er $\mathbb{R}^{m}$ og den højre er $\mathbb{R}^{n}$.
[^2]: Injektiv betyder one to one, og skrives injective på engelsk. Surjektiv betyder onto og skrives surjective på engelsk.
[^3]: Dette er billedet. Defineres også som værdimængden.