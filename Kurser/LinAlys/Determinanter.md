#forelæsning 
Begyndelsesdato: Kl. 08:08  Den 08-12-2022   Uge-49
## Definition 6.8 (Isometrier)
En isometri fra V til W er en... :: lineær afbildning af $T:V \to W$ som er både injektiv og surjektiv.
V og W er isomorfe hvis der eksisterer... :: en isometri mellem dem $V \to W$.
Vi kan skrive isometri således på papir... :: $T: \mathbb{P}_{3}\to \mathbb{R}^{4}$. hvor $a_{3}x^{3}+...+a_{0}x^{0}\rightarrow (a_{0},...,a_{3})\text{ eller }(a_{3},...,a_{0})$.

## Sætning
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
En generisk matrice:[^1]
$$det(A)=\sum_{j=1}^{n}(-1)^{1+j}a_{1j}\cdot det(A_{1j})$$
Hvor matricen $$A=\left[
\begin{array}{ccc} a_{11} & a_{12} & ... \\ a_{21} & a_{22} & ... \\ \vdots & \vdots & \vdots
\end{array}
\right] $$

## Sætning 7.6 (Rækkeoperationer i matricer)
Lad $A \in \mathbb{M}_{n,n}$. Givet er følgende regler givet for sammenhængen mellem diskriminanten og rækkeoperationer.
(I) Hvis A har en nulrække er... 
(II) Hvis $A \to A'$ og $R_{i}\leftrightarrow R_{j}$  er... 
(III) hvis $A \to A',c \in \mathbb{R}$ og $cR_{i} \to R_{i}$ er... 
(IV) Hvis A har to ens rækker er... 
(V) Hvis $A \to A'$ og $cR_{i} +R_{j} \to R_{j}$ er... 
(VI) Determinanten af I er...  
?
$det(A)=0$ 
$det(A')=-det(A)$ 
$det(A')=c\cdot det(A)$ 
$det(A)=0$
$det(A')=det(A)$
$det(I)=1$[^2]

## Sætning 7.7
Definition af den generelle formel for determinanten af en matrice.
Givet $A \in \mathbb{M}_{n,n}$ og $r,k \in \{1,...,n \}$ så er det(A)=...
?
$$\sum_{k=1}^{n}(-1)^{r+k}a_{rk}\cdot det(A_{rk})$$[^3]

## Sætning 7.9[[Lineære Afbildninger]]
Hvis $A,B \in \mathbb{M}_{n,n}$ så er $det(AB)=...$::$det(A)det(B)$

## Definition for transponering
For $A \in \mathbb{M}_{n,n}$, sæt $A^{t}=...$:: matricen hvis (i,j)-te indgang er $a_{ji}$. Altså en spejlbildning i diagonalen.

## Sætning 7.12
$det(A^{t})=...$::$det(A)$.

# Fodnoter
[^1]: Dette bliver til en sum af n! led. Så for en 3x3 matrice er det 6 led. Denne formel er meget upraktisk for en datalogisk synspunkt, men kan godt bruges til at give en definition på determinanten.
[^2]: I er identitetsmatricen. Dette kan altså fortælle os hvad determinanten bliver når man reducerer. Enten får man en nulrække eller to ens rækker, og så er det nul, eller også finder man I.
[^3]: r=1 er definitionen af determinanten.