# 10.1
Lad $f:\mathbb{R}^{2}\to \mathbb{R}$ være givet ved $f(x,y)=sin(x)sin(y)$
## (a)
Vis at (0,0) og $(0,\pi )$ er stationære punkter og udregn Hessematricen $Hf(0,0)$.
$$\nabla f(x,y)=\left[
\begin{array}{c}
\cos{(x)}\sin{(y)} \\ 
\sin{(x)}\cos{(y)}
\end{array}
\right] $$
$$\nabla f(0,0)=\left[
\begin{array}{c}\cos{(0)}\sin{(0)} \\ \sin{(0)}\cos{(0)}
\end{array}
\right] =\vec{0}$$
$$\nabla f(n \pi ,n \pi )=\vec{0}$$
$$Hf(x,y)=\left[
\begin{array}{cc}
(-\sin{x})\sin{y}  & \cos{x}\cos{y} \\ 
\cos{x}\cos{y} & \sin{x}(-\sin{y})
\end{array}
\right] $$
$$Hf(0,0)=\left[
\begin{array}{cc}0 & 1 \\ 1 & 0
\end{array}
\right] $$
## (b)
![[pointopgave 10 1.b.png]]
Ved visuel inspektion kan vi konkludere at det stationære punkt $(0,0)$ må være et sadelpunkt.
## (c)
Brug konturer til at vise at $(0,\pi )$ er et sadelpunkt.
![[pointopgave 10 1.c.png]]
Her kan vi finde at alle punkter med pi og/eller nul er sadelpunkter.
# 10.2
Lad $A \in \mathbb{M}_{3,3}$ være matricen $$A=\left[
\begin{array}{cc}4 & 3 & 7  \\ 1 & 1 & 2 \\ 3 & 2 & 6
\end{array}
\right] $$
## (a)
Vis at det(A)=1.
$$det(A)=4 \cdot  det \left[
\begin{array}{cc}1  & 2 \\ 2 & 6
\end{array}
\right] -3 \cdot det \left[
\begin{array}{cc}1 & 2 \\ 3 & 6
\end{array}
\right] +7 \cdot det \left[
\begin{array}{cc} 1 & 1 \\ 3 & 2
\end{array}
\right] $$
$$det(A)=4(6-4)-3(6-6)+7(2-3)=8-0-7=1$$
## (b)
Beregn $A^{-1}$ og bevis at $det(A^{-1})=1$.
$$[A|I]=\left[
\begin{array}{ccc|ccc}
4 & 3 & 7 & 1 & 0 & 0 \\ 
1 & 1 & 2 & 0 & 1 & 0 \\ 
3 & 2 & 6 & 0 & 0 & 1
\end{array}
\right] \Rightarrow \left[
\begin{array}{ccc|ccc}
1 & 0 & 0  & 2 & -4 & -1 \\ 
0 & 1 & 0 & 0 & 3 & -1 \\ 
0 & 0 & 1 & -1 & 1 & 1
\end{array}
\right] $$
$$det(A^{-1})=2(3+1)+4(0-1)-1(0+3)=8-4-3=1$$
## (c)
$$det(I)=det(BB^{-1})=det(B)det(B^{-1})=1$$
Hvad vi har opskrevet betyder at determinanten til begge matricer skal enten være +1 eller -1. 
Determinanten til Identitetsmatricen er altid 1, siden at begge matricer skal kun heltal som indgange vil determinanten altid være et helt tal, for både $B$ og $B^{-1}$. Dette betyder at vi kun kan få 1 som resultat hvis begge tal er 1, med samme fortegn.

# 10.3
Lad $A \in \mathbb{M}_{2,2}$ være invertibel og opfylde $A^{t}=A$ hvor $A^{t}$ betegner den transponderede som i pointopgave 8, og lad $f:\mathbb{R}^{2}\to \mathbb{R}$ være funktionen givet ved prikproduktet
$$f(\vec{v})=\vec{v}(A \vec{v})$$
## (a)
Vi at $\nabla f(\vec{v})=2A \vec{v}$ og konkludér at $\vec{v}=(0,0)$ er det eneste stationære punkt for f. Vis også at Hessematricen $Hf(0,0)$ er 2A.
$$f(\vec{v})=\vec{v}\cdot (A \vec{v})=A \vec{v}^{2}$$
$$\nabla f(\vec{v})= \frac{\delta f}{\delta \vec{v}}=2A \vec{v}$$
For at dette skal give $\vec{0}$ så må $2A \vec{v}=\vec{0}\Rightarrow \vec{v}=\vec{0}$.
Hessematricen er:
$$Hf(\vec{v})=\left[
\begin{array}{c}2A
\end{array}
\right] $$
v forsvinder da vi differentier i forhold til den to gange, og den er blot 1 værdi da vi har 1 variabel.
$$Hf(\vec{0})=[2A]$$
## (b)
Beregn diskriminanten af $p(x)=f(x,1)\in \mathbb{P}_2$ og relater den til determinanten af A.
$$p(x)=f(x,1)=(x,1)^{2}\cdot(A)$$
$$p(x)=(x^{2}+1) \cdot det(A)$$
$$d=0^{2}-4(1)(det(A))=-4det(A)$$

## (c)
Antag nu at $det(A)<0$, og brug (b) til at vise at der både findes et punkt $\vec{v}\in \mathbb{R}^{2}$ med $f(\vec{v})>0$ og et punkt $\vec{w}$ med $f(\vec{w})<0$.
$$x= \frac{-b\pm\sqrt{d}}{2a}= \pm \frac{\sqrt{-(det(A))}}{2}$$
Da determinanten til A er negativ bliver kvadratroden positiv, derfor reel og så har vi to reelle rødder.
Vi finder $\pm$ derfor at $f(\vec{v})>0$ og $f(\vec{w})<0$ disse to punkter eksisterer.