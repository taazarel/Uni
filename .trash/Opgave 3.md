#aflevering 
# Opgave 

# Opgave 5
## a
$$\nabla f(x,y,z)= \left(
\begin{array}{c}
\sin{x}-z \\ 3y-z  \\ 2z-(x+y)
\end{array}
\right)$$
Når $\nabla f(x,y,z)= \vec{0}$ så er punktet stationært. Hvis vi indsætter $(0,0,0)$ får vi $$\nabla f(0,0,0)= \left(
\begin{array}{c}
\sin{0}-0 \\ 3(0)-0 \\ 2(0)-(0+0)
\end{array}
\right)= \left(
\begin{array}{c}
0 \\ 0 \\ 0
\end{array}
\right)= \vec{0}$$
Derfor må $(0,0,0)$ være et stationært punkt.

## b
$$D^{2}f(x,y,z)= \left[
\begin{array}{ccc}
\cos{x} & 0 & -1 \\ 
0 & 3 & -1 \\ 
-1 & -1 & 2
\end{array}
\right] $$
$$D^{2}f(0,0,0)= \left[
\begin{array}{ccc}
1 & 0 & -1 \\ 
0 & 3 & -1 \\ 
-1 & -1 & 2
\end{array}
\right]$$
Vi kan finde det karakteristiske polynomie med $det(D^{2}f - \lambda I)$.
$$det(D^{2}f(0,0,0)- \lambda I)=(1-\lambda)((3-\lambda )(2-\lambda )-1)+ (-1)(0(-1)-(-1)3-\lambda)$$
$$= (1-\lambda)(6-5\lambda +\lambda^{2}-1)-(3-\lambda)$$
$$=6-5\lambda +\lambda ^{2}-1 -6\lambda +5\lambda ^{2}-\lambda ^{3}+\lambda -3+\lambda = -\lambda^{3}+6\lambda ^{2}-9\lambda +2$$
Vi vil gerne finde værdien for lambda når udtrykket er lig med nul. For at gøre dette lettere kan vi skrive
$$-(\lambda -2)(\lambda ^{2}-4\lambda +1)=0$$
Her kan vi allerede se at en løsning er $\lambda =2$.
Men den anden er blot et andengradspolynomie, så vi løser dette.
Først finder vi determinanten $d = (-4)^{2} - 4(1)(1)=12$ og derefter indsætter vi.
$$\lambda = \frac{-(-4)\pm \sqrt{12}}{2(1)}=2 \pm \frac{\sqrt{12}}{2}= 2 \pm \frac{\sqrt{12}}{\sqrt{4}}=2\pm \sqrt{\frac{12}{4}}=2\pm \sqrt{3}$$
Siden vi har en 3x3 matrix så får vi maks tre egenværdier. Her er vores egenværdier $\lambda =2, \lambda =2+\sqrt{3}, \lambda =2-\sqrt{3}$.

## c
