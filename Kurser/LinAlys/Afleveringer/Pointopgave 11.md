## mws572 Luci Fenger
# 1
Skitsen kommer til at blive en halv cirkel med centrum i origo.
![[Pointopgave 11 2022-12-19 17.38.01.excalidraw]]
Givet er $$A=\{(x,y)\in \mathbb{R}^{2}|x^{2}+2y^{2}\leq 1,x \geq 0\} \subseteq \mathbb{R}^{2}$$
Og funktionen $f(x,y)=xy^{2}-x^{2}$.
Da vi har to krav, selve underrummet og funktionen kan vi benytte Laranges formel, finde de kritiske punkter, og skal også huske at finde punkterne hvor funktionen ikke er kontinuer, altså knækket på top og bund.

OBS: Jeg byttede om på f og g, da jeg først opdagede det til sidst har jeg ikke tid til at rette det, bare husk:
$f(x,y)=x^{2}+2y^{2}-1$
$g(x,y)=xy^{2}-x^{2}$

Vi starter med at finde gradienterne.

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
Og her enten $y=\pm \frac{1}{\sqrt{2}}$ eller $y=0$.
Dette giver os tre punkter $(0,\pm \frac{1}{\sqrt{2}})$ og $(1,0)$.
Nu kan vi finde lambda. Her bruger vi de originale gradienter:
$$4y=\lambda (2xy) \Rightarrow \lambda =\frac{2}{x}$$
$$2x= \lambda (y^{2}-2x) \Rightarrow 2x = \frac{2}{x}(y^{2}-2x) \Rightarrow \frac{2y^{2}}{x}-4=2x$$
$$\Rightarrow 2y^{2}=2x^{2}+4x \Rightarrow y^{2}=x^{2}+2x$$
Nu hvor vi har fundet y som en afhængig af x kan vi indsætte i f.
$$f(x,y)=x^{2}+2y^{2}-1=0\Rightarrow 3x^{2}+4x-1$$
Nu kan vi finde determinanten og finde x
$$d=4^{2}-(4*3*(-1))=28$$
$$x= \frac{-4\pm\sqrt{28}}{6}= \frac{-2\pm\sqrt{7}}{3}$$
Her kan vi se bort fra den negative kvadratrod, da x skal være positiv.
$$y=\pm\sqrt{x^{2}+2x}=\pm \sqrt{\frac{2}{3} (-2 + \sqrt{7}) + \frac{1}{9} (-2 + \sqrt{7}^2)}\approx \pm 0.7$$
Så vi har fundet de kritiske punkter $$\left(\frac{-2+\sqrt{7}}{3},0.7\right)\text{ og }\left(\frac{-2+\sqrt{7}}{3},-0.7\right)$$
De sidste to punkter finder vi der hvor randen knækker (ikke er kontinuert).
Det må være når $x=0$ og derfor bliver $y=\pm \frac{1}{\sqrt{2}}$. 
Herfra kan vi indsætte vores punkter i funktionen for at sammenligne dem.
$\left(\frac{-2+\sqrt{7}}{3},0.7\right)\text{ og }\left(\frac{-2+\sqrt{7}}{3},-0.7\right)$ Vi har også $(0,\frac{1}{\sqrt{2}})\text{ og }(0,- \frac{1}{\sqrt{2}})$ og til sidst $(1,0)\text{ og }(0,0)$.
Vi indsætter disse i $g(x,y)$
$g(\frac{-2+\sqrt{7}}{3},\pm0.7)=0.059$ Maxpunkter
$g(0,\pm \frac{1}{\sqrt{2}})=0$ Sadelpunkter
$g(1,0)=-1$ Minimumspunkt
$g(0,0)=0$ Sadelpunkt

Med dette er vi færdige.
# 2
## (a)
Hvis $det(A)=1$ så er $det(A)det(B)=1$ derfor må $det(AB)=1$hvilket vi finder gennem den associative lov. Dette betyder at $AB \in SL_{n}(\mathbb{Z})$.
## (b)
Givet er en matrice hvor alle indgange er hele. Dette giver os en invers matrix $A^{-1}$ hvor alle indgange er hele. Vi definerer $AA^{-1}=I$ . Desuden ved vi at $det(I)=1$ Hvilket betyder $det(AA^{-1})=det(A)det(A^{-1})\Rightarrow det(A^{-1})=1$ Dette skal være sandt da vi ved at $det(A)=1$.

# 3
## (a)
Dette er den generelle ligning til en plan.
$\vec{e}\cdot (\vec{x}-\vec{a})=0$
Vi indsætter en af vores punkter
$\vec{e}\cdot (\vec{x}-(2,1,3))=0$
Nu finder vi to vektorer i planen, som går mellem vores tre punkter.
$(1,-2,1)-(2,1,3)=(-1,-3,-2)$
$(0,1,5)-(2,1,3)=(-2,0,2)$
Til sidst finder vi enhedsvektoren. Som vi ved skal være ortonormal på disse to vektorer.
$\vec{e}=(-1,-3,-2)\times (-2,0,2)=(-6,-2,-6)$
Planens ligning kan udtrykkes ved $(-6,-2,-6)\cdot (\vec{x}-(2,1,3))=0$
## (b)
Vi er givet et punkt og to vektorer som kan ligge i planen. Så vi kan bruge vektorerne til at finde normalvektoren.
$\vec{e}=(5,1,7)\times (-3,2,2)=(-12,-31,13)$
$(-3,2,2)\times (5,1,7)=(12,31,-13)=-\vec{e}$
Planens ligning kan udtrykkes ved $(-12,-31,13)\cdot (\vec{x}-(1,0,-4))=0$.
<<<<<<< HEAD
Vi finder at planens ligning ikke er tom, da vi kan finde
$(-12,-31,13)\cdot ((1,0,-4)-(1,0,-4))=0$.
Vi finder at der er lukket under addition $(-12,-31,13)\cdot (\vec{x}-(1,0,-4))+(-12,-31,13)\cdot (\vec{v}-(1,0,-4))=0+0=0$$(-12,-31,13)\cdot (\vec{x}-(1,0,-4)+\vec{v}-(1,0,-4))=0$
$(-12,-31,13)\cdot (\vec{x}+\vec{v}-(2,0,-8))=0$
Vi finder at der er lukket under multiplikation ved
$(-12,-31,13)\cdot (\vec{x}-(1,0,-4))(-12,-31,13)\cdot (\vec{v}-(1,0,-4))=0$.
$(-12,-31,13)\cdot (\vec{x}\vec{v}-(1,0,-4)^{2}-\vec{x})$

## (c)
Først udvider vi den venstre side.
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
Efter finder vi den venstre side
$$T(\vec{v})\times T(\vec{w})=(v_{2},v_{3},v_{1})\times (w_{2},w_{3},w_{1})$$
$$=\left[
\begin{array}{c}
v_{3}w_{1}-v_{1}w_{3} \\ 
-(v_{2}w_{1}-v_{1}w_{2}) \\ 
v_{2}w_{3}-v_{3}w_{2}
\end{array}
\right] $$
Vi kan herved se at $T(\vec{v}\times \vec{w})=T(\vec{v})\times T(\vec{w})$. Altså at dette er sandt.

Nej det ville ikke være det samme for det andet scenarie da vi kan modbevise med:
$\vec{v}=\vec{e_{1}}$ og $\vec{w}=\vec{e_{2}}$, så bliver $T(\vec{v})=\vec{e_{2}}$ og $T(\vec{w})=\vec{e_{1}}$.
Nu kan vi vise at $T(\vec{v}\times \vec{w})=T(\vec{e_{3}})=\vec{e_{3}}$ da $\vec{e_{3}}=(0,0,1)$ 
men derimod bliver $T(\vec{v})\times T(\vec{w})=\vec{e_{2}}\times \vec{e_{1}}=-\vec{e_{3}}$. 