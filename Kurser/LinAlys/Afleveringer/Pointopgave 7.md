# 7.1
## a
Givet er $G(x,y)=((x+y^{2}),(\sin{}(xy)))$ , derved $g_{1}(x,y)=(x+y)^{2}$ og $g_{2}(x,y)=\sin{(xy)}$
Jacobi matricen er defineret som:
$$DG(x,y)=\left[
\begin{array}{cccc}
2(x+y) & 2(x+y) \\ 
y \cos{(xy)} & x \cos{(xy)}
\end{array}
\right] $$
## b

# 7.2
Betragt vektorerne i $\mathbb{R}^{5}$
$$
\begin{array}{cc}
v_{1}=(1,0,3,-1,4) & v_{2}=(2,0,5,-2,2) \\ v_{3}=(-3,0,-7,3,-6) & v_{4}=(4,0,11,-4,8)
\end{array}
$$
## a
*Bestem dimensionen af $V=span(v_{1},v_{2},v_{3},v_{4})$ og udvælg vektorer fra familien som udgør en basis for V og bestem koordinaterne for de øvrige af vektorerne udtrykt i denne basis. Husk at du skal argumentere for dine svar.*

$$\left[
\begin{array}{cccc}
1 & 2 & -3 & 4 \\ 
0 & 0 & 0 & 0 \\ 
3 & 5 & -7 & 11 \\ 
-1 & -2 & 3 & -4 \\ 
4 & 2 & -6 & 8
\end{array}
\right] $$
Vi kan herved se at der findes en nulrække i denne matrix.
$$\left[
\begin{array}{ccccc}
1 & 0 & 3 & -1 & 4 \\ 
2 & 0 & 5 & -2 & 2 \\ 
-3 & 0 & -7 & 3 & -6 \\ 
4 & 0 & 11 & -4 & 8
\end{array}
\right] $$
Vi kan vælge alt på nær nul-rækken dette vil give os en basis med $dim V=3$ da elementerne har 3 dimensioner (efter at vi fjerner nul-rækken og reducerer til echelon form.)

Vi vælger disse vektorer som en basis for V:
$$\left[
\begin{array}{cccc}
1 & 2 & -3 & 4 \\ 
3 & 5 & -7 & 11 \\ 
-1 & -2 & 3 & -4 \\ 
4 & 2 & -6 & 8
\end{array}
\right] \text{ eller }
\left[
\begin{array}{cccc}
1  & 3 & -1 & 4 \\ 
2  & 5 & -2 & 2 \\ 
-3  & -7 & 3 & -6 \\ 
4  & 11 & -4 & 8
\end{array}
\right] $$
**Hvad betyder det at "bestemme koordinaterne for de øvrige af vektorerne udtrykt i denne basis"?**
## b
**Udvid den basis du fandt i a, med passende elementer fra standardbasen for $\mathbb{R}^{5}$, så det samlet udgør en basis for $\mathbb{R}^{5}$.**
Vi kan udvide denne basis med [[Abstrakte vektorrum#3.20 (Udvidelsessætningen)|Udvidelsesalgoritmen]] så vi gør dette:
$$\left[
\begin{array}{cccc}
1 & 2 & -3 & 4 \\ 
0 & 0 & 0 & 0 \\ 
3 & 5 & -7 & 11 \\ 
-1 & -2 & 3 & -4 \\ 
4 & 2 & -6 & 8
\end{array}
\right] \Rightarrow 
\left[
\begin{array}{cccc|ccccc}
1 & 2 & -3 & 4  & 1 & 0 & 0 & 0 & 0\\ 
0 & 0 & 0 & 0  & 0 & 1 & 0 & 0 & 0\\ 
3 & 5 & -7 & 11 & 0 & 0 & 1 & 0 & 0 \\ 
-1 & -2 & 3 & -4 & 0 & 0 & 0 & 1 & 0 \\ 
4 & 2 & -6 & 8 & 0 & 0 & 0 & 0 & 1
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
$$
\begin{array}{ccc}
v_{1}=(1,0,3,-1,4) & v_{2}=(2,0,5,-2,2) & v_{3}=(-3,0,-7,3,-6) \\ v_{4}=(0,1,0,0,0) & v_5=(0,0,0,1,0)
\end{array}
$$

# 7.3
## a

## b

## c
