# §8 i Messer
- Egenværdier
- Egenvektorer
- Egenrum
## Definition 8.1 (Egenvektor)
Lad $T:V \to V$ være en lineær operator. En egenværdi for T er et $\lambda \in \mathbb{R}$ så der findes... :: $\vec{v}\in V \backslash \{\vec{0} \}$, med $T(\vec{v})=\lambda \vec{v}$. Da er $\vec{v}$ en egenvektor hørende til $\lambda$, som er egenværdien.[^1]

### Specialtilfælde
Givet $V=\mathbb{R}^{n}$ så kan egenvektoren defineres som... :: $A \vec{v}=\lambda \vec{v}\Rightarrow A \vec{v}=\lambda I \vec{v}\Rightarrow A \vec{v}-\lambda I \vec{v}=\vec{0}\Rightarrow (A-\lambda I)\vec{v}=\vec{0}$.

Egenvektorer og egenværdier kan beskrives intuitivt som... :: alle vektorer som bliver på deres eget span efter en transformation. De bliver blot skaleret som var der brugt en skalar, vi kalder denne skalar for egenværdien og betegner den $\lambda$.

## Sætning 8.2 (Egenværdi)
$\lambda \in \mathbb{R}$ er en egenværdi for $A \in \mathbb{M}_{n,n}\Leftrightarrow$ :: $det(A-\lambda I)=0$.

## Sætning på side 335
For $A \in \mathbb{M}_{n,n}$ er $p:\mathbb{R}\to \mathbb{R}$, polynomiet $p(\lambda )=det(A-\lambda I)$ et polynomium af grad n. Og er skrevet som... :: $p(\lambda )=\lambda ^{n}+c_{n-1}\lambda ^{n-1}+...+c_{0}$.

## §8.2 At finde egenværdier for en operator
V har end. dim. Vælg så en ordnet basis $B=[\vec{v_{1}},...,\vec{v_{n}}]$ lad $A \in \mathbb{M}_{n,n}$ være matricen for T, referende til B. Vi kan herved skrive $[T(\vec{v})]_{B}=A [\vec{v}]_{B}$ for alle $\vec{v}\in V$. Vi finder egenværdierne ved... :: $p(\lambda )=det(\lambda I-A)=\lambda ^{n}+c_{n-1 }\lambda ^{n-1}+...+c_{0}$  Så er rødderne egenværdierne.

## Påstand
Givet $A'=P^{-1}AP$ så er $det(A'-\lambda I)=...$:: $det(A-\lambda I)$.



# Fodnoter
[^1]: Kan også skrives som $A \vec{v}=\lambda \vec{v}\Rightarrow (A-\lambda I)\vec{v}=\vec{0}$ givet $V = \mathbb{R}^{n}$.