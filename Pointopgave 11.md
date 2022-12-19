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
Men her vil gradienten til f ikke fungere da den ikke tager forhold til mængden. Vi kan derfor definere:
$$x=\sqrt{1-2y^{2}}$$
Selvom vi får en kvadratrod her ser vi kun på den positive, da vi har kravet at x skal være større end 0.
$$y=\pm\sqrt{\frac{1-x^{2}}{2}}$$
Nu kan vi indsætte i gradienten til f for begge tilfælde:
$$\nabla f\left(x,\sqrt{\frac{1-x^{2}}{2}}\right)=\left[
\begin{array}{c}
2x \\ 
\pm4\sqrt{\frac{1-x^{2}}{2}}
\end{array}
\right] $$
Her finder vi enten $x=0$ eller $x=1$.
$$\nabla f(\sqrt{1-2y^{2}},y)=\left[
\begin{array}{c}
2\sqrt{1-2y^{2}} \\ 
4y
\end{array}
\right] $$
Og her enten $y=\pm 1/\sqrt{2}$ eller $y=0$.

$$2x= \lambda (y^{2}-2x) \Rightarrow 2x = \frac{2}{x}(y^{2}-2x) \Rightarrow \frac{2y^{2}}{x}-4=2x$$
$$\Rightarrow 2y^{2}=2x^{2}+4x \Rightarrow y^{2}=x^{2}+2x$$
$$4y=\lambda (2xy) \Rightarrow \lambda =\frac{2}{x}$$
$$f(x,y)=x^{2}+2y^{2}-1=0\Rightarrow 3x^{2}+4x-1$$
$$d=4^{2}-(4*3*(-1))=28$$
$$x= \frac{-4\pm\sqrt{28}}{6}= \frac{-4\pm2\sqrt{7}}{6}$$
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
