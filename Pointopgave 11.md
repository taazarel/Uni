# 1

# 2
## (a)
Hvis $det(A)=1$ så er $det(A)det(B)=1$ derfor $det(AB)=1$ hvilket betyder at $AB \in SL_{n}(\mathbb{Z})$.
## (b)
Givet er en matrice hvor alle indgange er hele. Dette giver os en invers matrix $A^{-1}$ hvor alle indgange er hele. Så kan vi definere $AA^{-1}=I$ og da dette altid er sandt, (medmindre vektorrummet er abstrakt), $det(I)=1$ Hvilket betyder $det(AA^{-1})=det(A)det(A^{-1})\Rightarrow det(A^{-1})=1$ Dette skal være sandt da vi ved at $det(A)=1$.

# 3
## (a)
$\vec{e}\cdot (\vec{x}-\vec{a})=0$
$\vec{e}\cdot (\vec{x}-(2,1,3))=0$
$(1,-2,1)-(2,1,3)=(-1,-3,-2)$
$(0,1,5)-(2,1,3)=(-2,0,2)$
$\vec{e}=(-1,-3,-2)\times (-2,0,2)=(-6,-2,-6)$
Planens ligning kan udtrykkes ved $(-6,-2,-6)\cdot (\vec{x}-(2,1,3))=0$
## (b)
Vi er givet et punkt og to vektorer som kan ligge i planen. Så vi kan bruge vektorerne til at finde normalvektoren.
$\vec{e}=(5,1,7)\times (-3,2,2)=(-12,-31,13)$
Planens ligning kan udtrykkes ved $(-12,-31,13)\cdot (\vec{x}-(1,0,-4))=0$.
Er dette et underrum af $\mathbb{R}^{3}$? 
**Lav den her før vi slutter**
## (c)
$$T(\vec{v}\times \vec{w})=T\left(\left[
\begin{array}{c}
v_{2}w_{3}-v_{3}w_{2} \\ 
v_{3}w_{1}-v_{1}w_{3} \\ 
v_{1}w_{2}-v_{2}w_{1}
\end{array}
\right]\right) =\left[
\begin{array}{c}
v_{3}w_{1}-v_{1}w_{3} \\ 
v_{1}w_{2}-v_{2}w_{1} \\ 
v_{2}w_{3}-v_{3}w_{2} \\ 
\end{array}
\right] $$
$$T(\vec{v})\times T(\vec{w})=(v_{2},v_{3},v_{1})\times (w_{2},w_{3},w_{1})$$
$$=\left[
\begin{array}{c}
v_{3}w_{1}-v_{1}w_{3} \\ 
-(v_{2}w_{1}-v_{1}w_{2}) \\ 
v_{2}w_{3}-v_{3}w_{2}
\end{array}
\right] $$
Vi kan herved se at $T(\vec{v}\times \vec{w})=T(\vec{v})\times T(\vec{w})$. Altså at dette er sandt.

Nej det ville ikke være det samme for dette scenarie da vi kan modbevise med:$\vec{v}=\vec{e_{1}}$ og $\vec{w}=\vec{e_{2}}$, så bliver $T(\vec{v})=\vec{e_{2}}$ og $T(\vec{w})=\vec{e_{1}}$.
Nu kan vi vise at $T(\vec{v}\times \vec{w})=T(\vec{e_{3}})=\vec{e_{3}}$ da $\vec{e_{3}}=(0,0,1)$ men at $T(\vec{v})\times T(\vec{w})=-\vec{e_{3}}$.
