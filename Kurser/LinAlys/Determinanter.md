#forelæsning 
Begyndelsesdato: Kl. 08:08  Den 08-12-2022   Uge-49
## Definition 6.8 (Isometrier)
En isometri fra V til W er en... :: lineær afbildning af $T:V \to W$ som er både injektiv og surjektiv.
V og W er isomorfe hvis der eksisterer... :: en isometri mellem dem $V \to W$.
Vi kan skrive isometri således på papir... :: $T: \mathbb{P}_{3}\to \mathbb{R}^{4}$. hvor $a_{3}x^{3}+...+a_{0}x^{0}\rightarrow (a_{0},...,a_{3})\text{ eller }(a_{3},...,a_{0})$.

### Sætning
Lad V og W være end. dim. Da er V og W isomorfe hvis og kun hvis... :: $dim(V)=dim(W)$.

# §7 Determinanter
## Definition
Determinanten defineres som en transformation på en matrice $det:\mathbb{M}_{n,n}\to \mathbb{R}$. Determinanten skrives således på
En 2x2 matrice...
En 3x3 matrice...
En generisk matrice...
?
En 2x2 matrice:
$$det(\vec{a},\vec{b})=det\left[
\begin{array}{cc}a_{1} & b_{1} \\ a_{2} & b_{2}
\end{array}
\right] =a_{1}b_{2}-a_{2}b_{1}$$
En 3x3 matrice:
$$det(\vec{a},\vec{b},\vec{c})=det\left[
\begin{array}{ccc}a_{1} & b_{1} & c_{1} \\ a_{2} & b_{2} & c_{2} \\ a_{3} & b_{3} & c_{3}
\end{array}
\right]$$$$=a_{1}\cdot det \left[
\begin{array}{cc}b_{2} & c_{2} \\ b_{3} & c_{3}
\end{array}
\right] -b_{1}\cdot det \left[
\begin{array}{cc}a_{2} & c_{2} \\ a_{3} & c_{3}
\end{array}
\right] +c_{1}\cdot det \left[
\begin{array}{cc}a_{2} & b_{2} \\ a_{3} & b_{3}
\end{array}
\right] $$
En generisk matrice:
$$det(A)=\sum_{j=1}^{n}(-1)^{1+j}a_{1j}\cdot det(A_{1j})$$

