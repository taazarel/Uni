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
$$det(I)=det(AA^{-1})=det(A)det(A^{-1})=1$$
Hvad vi har opskrevet betyder at determinanten til begge matricer skal enten være +1 eller -1. 
Determinanten til Identitetsmatricen er altid 1, siden at begge matricer skal kun heltal som indgange vil determinanten altid være et helt tal, for både $A$ og $A^{-1}$. Dette betyder at vi kun kan få 1 som resultat hvis begge tal er 1, med samme fortegn.

# 10.3
Lad $A \in \mathbb{M}_{2,2}$ være invertibel og opfylde $A^{t}=A$ hvor $A^{t}$ betegner den transponderede som i pointopgave 8, og lad $f:\mathbb{R}^{2}\to \mathbb{R}$ være funktionen givet ved prikproduktet
$$f(\vec{v})=\vec{v}(A \vec{v})$$
## (a)
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
$$p(x)=f(x,1)=(x,1)\cdot(A (x,1))$$


## (c)
