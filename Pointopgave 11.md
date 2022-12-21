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
Her ser vi at ifølge langranges multiplikatormetode så vil $\nabla g(0,0)=\vec{0}$ være en kandidat. For at teste dette indsætter vi i $f(x,y)$. $f(0,0)=0^{2}+2(0)^{2}\leq 1, 0 \geq 0$. Da disse begge er sande finder vi et lokalt ekstrema ved $(0,0)$. Og dette er et minimum da vi får $f(0,0)=0 \leq 1$.
De andre værdier på randen kan vi finde ved dette: $\nabla f(\vec{a}) = \lambda \nabla g(\vec{a})$, hvor $\lambda \in \mathbb{R}$.
Vi udvider:
$$
\begin{array}{c}
2x=\lambda y^{2}-2x \\ 
4y=\lambda 2xy
\end{array}
$$
Og isolerer lambda.
$$
\begin{array}{c}
\lambda y^{2}=4x\\ 
\lambda x=2
\end{array}\Rightarrow 
\begin{array}{c}
\lambda =\frac{4x}{y^{2}} \\ 
\lambda =\frac{2}{x}
\end{array} 
$$
Her har vi reduceret til to ligninger med to ubekendte.
$$\frac{4x}{y^{2}}=\frac{2}{x}\Rightarrow 4x^{2}=2y^{2}\Rightarrow \sqrt{2x^{2}}=\sqrt{y^{2}}\Rightarrow y=\sqrt{2x^{2}}$$
Nu indsætter vi blot dette i $f(x,y)$ og finder x.
$$f(x,y)=x^{2}+2y^{2}-1\leq 0\Rightarrow x^{2}+2(\sqrt{2x^{2}})-1\Rightarrow x^{2}+2x^{2}-1$$
$$=3x^{2}-1$$
Lad os finde determinanten.
$$d=b^{2}-4ac=0^{2}-4(3)(-1)=12$$
Siden vores determinant er positiv må vi have to reelle løsninger. Lad os finde dem:
$$x=\pm \frac{\sqrt{d}}{2a}= \pm \frac{\sqrt{12}}{6}=\pm \frac{\sqrt{3}}{3}$$
For at finde vores y-værdier kan vi indsætte i den formel som vi fandt for y.
$$y=\sqrt{2\left(\pm\frac{\sqrt{3}}{3}\right)^{2}}=\sqrt{\frac{2}{3}}=\frac{\sqrt{6}}{3}$$
Læg mærke til at $\pm$ forsvinder her da vi hæver i anden.
Disse to punkter på kanten bliver
$$\left(\frac{\sqrt{3}}{3},\frac{\sqrt{6}}{3}\right),\left(\frac{-\sqrt{3}}{3},\frac{\sqrt{6}}{3}\right)$$
Lad os indtaste disse værdier i f, for at teste dem.
$$f\left(\frac{\sqrt{3}}{3},\frac{\sqrt{6}}{3}\right)=\frac{1}{3}+2 \frac{6}{9}-1=\frac{1}{3}+ \frac{12}{9}- \frac{9}{9}=\frac{1}{3}+ \frac{1}{3}=\frac{2}{3}$$
Det andet punkt er ikke gyldigt da vi ved at $x \geq 0$ og i det andet punkt er x negativt.

Hvis $(1,0)$ så $f(1,0)=0$ max punkt. 
Vi kan også finde $f(0,\pm \sqrt{\frac{1}{2}})=2(\frac{1}{2})=0$. Er også et max punkt. 
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
$(-3,2,2)\times (5,1,7)=(12,31,-13)=-\vec{e}$
Planens ligning kan udtrykkes ved $(-12,-31,13)\cdot (\vec{x}-(1,0,-4))=0$.
Vi finder at planens ligning ikke er tom, da vi kan finde
$(-12,-31,13)\cdot ((1,0,-4)-(1,0,-4))=0$.
Vi finder at der er lukket under addition $(-12,-31,13)\cdot (\vec{x}-(1,0,-4))+(-12,-31,13)\cdot (\vec{v}-(1,0,-4))=0+0=0$$(-12,-31,13)\cdot (\vec{x}-(1,0,-4)+\vec{v}-(1,0,-4))=0$
$(-12,-31,13)\cdot (\vec{x}+\vec{v}-(2,0,-8))=0$
Vi finder at der er lukket under multiplikation ved
$(-12,-31,13)\cdot (\vec{x}-(1,0,-4))(-12,-31,13)\cdot (\vec{v}-(1,0,-4))=0$.
$(-12,-31,13)\cdot (\vec{x}\vec{v}-(1,0,-4)^{2}-\vec{x})$
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