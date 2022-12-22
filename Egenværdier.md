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



# Fodnoter
[^1]: Kan også skrives som $A \vec{v}=\lambda \vec{v}\Rightarrow (A-\lambda I)\vec{v}=\vec{0}$ givet $V = \mathbb{R}^{n}$.