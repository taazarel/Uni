# 7.1
## a
**Udregn Jacobimatricen $DG(x,y)$ for funktionen $G(x,y)$.**

Givet er $G(x,y)=((x+y^{2}),(\sin{}(xy)))$ , derved $g_{1}(x,y)=(x+y)^{2}$ og $g_{2}(x,y)=\sin{(xy)}$
Jacobi matricen er defineret som:
$$DG(x,y)=\left[
\begin{array}{cccc}
2(x+y) & 2(x+y) \\ 
y \cos{(xy)} & x \cos{(xy)}
\end{array}
\right] $$
## b
**Vis at hastighedsvektoren for den sammensatte funktion $F\circ c:\mathbb{R}\to \mathbb{R}^{2}$ er givet ved $\frac{d}{dt}F(c(t))=DF(c(t))\cdot c'(t)$.**

Givet er $$F(c(t))=(f_{1}(c(t)),f_{2}(c(t)))$$
$\frac{d}{dt}F(c(t))=$
$$\left(\frac{\delta f_{1}(c(t))}{\delta c_{1}(t)} \frac{\delta c_{1}(t)}{\delta t}+ \frac{\delta f_{1}(c(t))}{\delta c_{2}(t)} \frac{\delta c_{2}(t)}{\delta t},\frac{\delta f_{2}(c(t))}{\delta c_{1}(t)} \frac{\delta c_{1}(t)}{\delta t}+ \frac{\delta f_{2}(c(t))}{\delta c_{2}(t)} \frac{\delta c_{2}(t)}{\delta t}\right)$$
Hvilket også kan skrives som:
$$\Rightarrow \left[
\begin{array}{c}
\frac{\delta f_{1}(c(t))}{\delta c_{1}(t)} \frac{\delta c_{1}(t)}{\delta t}+ \frac{\delta f_{1}(c(t))}{\delta c_{2}(t)} \frac{\delta c_{2}(t)}{\delta t} \\ 
\frac{\delta f_{2}(c(t))}{\delta c_{1}(t)} \frac{\delta c_{1}(t)}{\delta t}+ \frac{\delta f_{2}(c(t))}{\delta c_{2}(t)} \frac{\delta c_{2}(t)}{\delta t}
\end{array}
\right] $$
Jacobimatricen er givet som
$$DF(c(t))=\left[
\begin{array}{cc}
\frac{\delta f_{1}(c(t))}{\delta c_{1}(t)} & \frac{\delta f_{1}(c(t))}{\delta c_{2}(t)} \\ 
\frac{\delta f_{2}(c(t))}{\delta c_{1}(t)} & \frac{\delta f_{2}(c(t))}{\delta c_{2}(t)}
\end{array}
\right] $$
og $c'(t)=$
$$\frac{d}{dt}c(t)=\left[
\begin{array}{}
\frac{\delta c_{1}(t)}{\delta t} \\ \frac{\delta c_{2}(t)}{\delta t}
\end{array}
\right] $$
Nu kan vi finde den højre side af ligningen som et matrixprodukt
$$DF(c(t))\cdot c'(t)= \left[
\begin{array}{c}
\frac{\delta f_{1}(c(t))}{\delta c_{1}(t)} \frac{\delta c_{1}(t)}{\delta t}+ \frac{\delta f_{1}(c(t))}{\delta c_{2}(t)} \frac{\delta c_{2}(t)}{\delta t} \\ 
\frac{\delta f_{2}(c(t))}{\delta c_{1}(t)} \frac{\delta c_{1}(t)}{\delta t}+ \frac{\delta f_{2}(c(t))}{\delta c_{2}(t)} \frac{\delta c_{2}(t)}{\delta t}
\end{array}
\right]$$
Herved har vi fundet $\frac{d}{dt}F(c(t))=DF(c(t))\cdot c'(t)$.
# 7.2
**Betragt vektorerne i $\mathbb{R}^{5}$**
$$
\begin{array}{cc}
v_{1}=(1,0,3,-1,4) & v_{2}=(2,0,5,-2,2) \\ v_{3}=(-3,0,-7,3,-6) & v_{4}=(4,0,11,-4,8)
\end{array}
$$
## a
**Bestem dimensionen af $V=span(v_{1},v_{2},v_{3},v_{4})$ og udvælg vektorer fra familien som udgør en basis for V og bestem koordinaterne for de øvrige af vektorerne udtrykt i denne basis. Husk at du skal argumentere for dine svar.**

$$\left[
\begin{array}{cccc}
1 & 2 & -3 & 4 \\ 
0 & 0 & 0 & 0 \\ 
3 & 5 & -7 & 11 \\ 
-1 & -2 & 3 & -4 \\ 
4 & 2 & -6 & 8
\end{array}
\right] $$
Vi kan herved se at der findes to nulrækker i denne matrix, da række 4 kan findes ved række 1.

Vi finder at $dim V=3$ da familien har 3 dimensioner (efter at vi fjerner nul-rækken og reducerer til echelon form.)

Vi vælger disse vektorer som en basis for V:
$$\left[
\begin{array}{ccc}
1 & 2 & -3 \\ 
0 & 0 & 0  \\ 
3 & 5 & -7  \\ 
-1 & -2 & 3  \\ 
4 & 2 & -6
\end{array}
\right]$$
Altså vektorerne $span \{v_{1},v_{2},v_{3} \}$ hvilket har disse koordinater i V
$$\Rightarrow  \left[
\begin{array}{ccc}
1 & 2 & -3 \\ 
3 & 5 & -7 \\ 
4 & 2 & -6
\end{array}
\right]$$
## b
**Udvid den basis du fandt i a, med passende elementer fra standardbasen for $\mathbb{R}^{5}$, så det samlet udgør en basis for $\mathbb{R}^{5}$.**

Vi kan udvide denne basis med [[Abstrakte vektorrum#3.20 (Udvidelsessætningen)|Udvidelsesalgoritmen]] så vi gør dette:
$$\left[
\begin{array}{ccc}
1 & 2 & -3  \\ 
0 & 0 & 0  \\ 
3 & 5 & -7  \\ 
-1 & -2 & 3  \\ 
4 & 2 & -6
\end{array}
\right] \Rightarrow 
\left[
\begin{array}{ccc|ccccc}
1 & 2 & -3   & 1 & 0 & 0 & 0 & 0\\ 
0 & 0 & 0   & 0 & 1 & 0 & 0 & 0\\ 
3 & 5 & -7  & 0 & 0 & 1 & 0 & 0 \\ 
-1 & -2 & 3  & 0 & 0 & 0 & 1 & 0 \\ 
4 & 2 & -6  & 0 & 0 & 0 & 0 & 1
\end{array}
\right] $$
Vi kan allerede her se hvad vi har brug for. For at være sikker kan man forkorte til echelon form. For tidens skyld så skipper vi frem til resultatet.
$$\left[
\begin{array}{ccccc}
1 & 2 & -3 & 0 & 0 \\ 
0 & 0 & 0 & 1 & 0 \\ 
3 & 5 & -7 & 0 & 0 \\ 
-1 & -2 & 3 & 0 & 1 \\ 
4 & 2 & -6 & 0 & 0
\end{array}
\right]$$
Dette er en udvidet basis som udspænder $\mathbb{R}^{5}$.

Hvilket vi også kan skrive som denne vektorfamilie:
$\{v_{1},v_{2},v_{3},v_{5},v_{6} \}$
$$
\begin{array}{ccc}
v_{1}=(1,0,3,-1,4) & v_{2}=(2,0,5,-2,2) & v_{3}=(-3,0,-7,3,-6) \\ v_{5}=(0,1,0,0,0) & v_6=(0,0,0,1,0)
\end{array}
$$
# 7.3
$E(\theta ,v)=\frac{1}{2}mv^{2}-mgl \cos{(\theta )}$ 
## a
**Bestem den affine funktion, der tangerer energifunktionen E i et punkt $(\theta_{1},v_{1})$.**

Lad os forkorte punktet til $(\theta_{1},v_{1})=(\vec{a})$ og $(\theta,v)=(\vec{x})$
En tangenthyperplan, hvilket er det samme som en affin funktion som tangerer en funktion er givet ved: $h(\vec{x})=E(\vec{a})+\nabla E(\vec{a})\cdot (\vec{x}-\vec{a})$.
Vi kan indsætte og reducere vores funktioner således 

$h(\vec{x})=(\frac{1}{2}m(v_{1})^{2}-mgl \cos{(\theta_{1} )})+(mgl \sin{(\theta_{1})},mv_{1})\cdot (\theta-\theta_{1},v-v_{1})$
$\Rightarrow h(\vec{x})=(\frac{1}{2}m(v_{1})^{2}-mgl \cos{(\theta_{1} )})+mgl \sin{\theta_{1}}(\theta-\theta_{1})+mv_{1}v-m(v_{1})^{2}$ 
$\Rightarrow h(\vec{x})=m(gl(\sin{\theta_{1}}(\theta-\theta_{1})-\cos{\theta_{1}})+v_{1}v- \frac{1}{2}(v_{1})^{2})$
Dette er den affine funktion som tangerer E i punktet $\vec{a}=(\theta_{1},v_{1})$.

## b
**Vis at i alle punkter $(\theta_{1},v_{1})\neq (n \pi ,0)$ for $n \in \mathbb{Z}$ har niveaukurven for E gennem punktet en tangent og find ligningen til denne. 
Beskriv niveaukurverne gennem punkterne $(n \pi ,0)$for $n \in \mathbb{Z}$.**

Vi kan ved 2.75 i TK se en definition for en niveaukurves tangent hvilket er givet ved: $\nabla E(\vec{a})\cdot (\vec{x}-\vec{a})=0$ så længe at $\nabla E(\vec{a})\neq \vec{0}$ dette giver at tangenthyperplanen er: $h(\vec{x})=E(\vec{a})$.

Ved $(\vec{a})=(n \pi ,0)$ så bliver $\nabla E(\vec{a})=\vec{0}$ da $\cos{(n\pi)}=0,v=0$ når $n \in \mathbb{Z}$ hvilket betyder at vores definition ikke fungerer. 
## c
**Tegn niveaukurver for udvalgte (positive) værdier af E og illustrer hvordan der er to kvalitativt forskellige "slags" niveaukurver, adskilt af niveaukurven for en bestemt værdi $E_{0}$. 
Find $E_{0}$ ved at eksperimentere. 
Giver den fundne værdi mening?**

Værdien er et sted mellem 9 og 10. og fra 10 til 11 er der et til skift
