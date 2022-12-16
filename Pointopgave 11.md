# 1
Givet er $$A=\{(x,y)\in \mathbb{R}^{2}|x^{2}+2y^{2}\leq 1,x \geq 0\} \subseteq \mathbb{R}^{2}$$
Og funktionen $f(x,y)=xy^{2}-x^{2}$.
Da vi har to krav, selve underrummet og funktionen kan vi benytte Laranges formel.
$f(x,y)=x^{2}+2y^{2}-1$
$g(x,y)=xy^{2}-x^{2}$

$$\nabla f(x,y)=\left[
\begin{array}{c}
2x \\ 4y
\end{array}
\right] $$
$$\nabla g(x,y)=\left[
\begin{array}{cc}
y^{2}-2x \\ 2xy
\end{array}
\right] $$
For at disse kan blive nul skal vi sætte
$\nabla f(0,0)=\vec{0}$ og $\nabla g(0,0)=\vec{0}$.
$\nabla f = \lambda \nabla g$


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
$$T(\vec{v})\times T(\vec{w})=$$
Ja det samme ville gælde for definitionen af $T(x,y,z)=(y,x,z)$.