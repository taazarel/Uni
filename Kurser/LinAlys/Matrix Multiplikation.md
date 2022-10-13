#forelæsning 
# Matrix multiplikation
## Definition 5.1 (Matrix Multiplikation)
$$A_{mxn}=\begin{array}{ccc}
a_11 & ... & a_{1n} \\ 
: & : & : \\ 
a_{m1} & ... & a_{mn}
\end{array}$$
$$B_{nxp}\begin{array}{ccc}
b_{11} & ... & b_{1p} \\ 
: & : & : \\
b_{n1} & ... & b_{np}
\end{array}$$

Og vi vælger to tal $[A]_{ij}=a_{ij},[B]_{jk}=b_{jk}$ kan vi finde at
$AB_{mxp},[AB]_{ik}=a_{i1}b_{1k}+...+a_{in}b_{nk}=\sum\limits_{j=1}^{n}a_{ij}b_{jk}$ , hvor $i=1,...,m$ og $k=1,...,p$.
## Definition 5.2 (Kvadratiske matricer)
En kvadratisk matrix er en matrix med samme antal søjler og rækker.
fx en nxn matrix.
$$A=
\left[
\begin{array}
&a_{11}&...&a_{1n} \\ 
:&&: \\
a_{m1}&... & a_{mn}
\end{array}
\right]
$$
Hvis A og B er kvadratiske matricer vil AB og BA være kvadratiske matrixer med samme antal søjler og rækker.

## Definition 5.3 (Identitetsmatricen)
$$
I_{n}=\begin{array}
&1_{11} & 0_{1n} \\ 
0_{n1} & 1_{nn}
\end{array}
$$
Hvis A er en mxn matrix så er $A*I_{n}=I_{m}*A=A$.

## Theorem 5.4 (Regneregler for matrix multiplikation)
**Advarsel:** $A*B=B*A$ er IKKE sandt i matrixmultiplikation.

- $(AB)C=A(BC)$ Associative lov
- $A(B+B')=AB+AB'$ Distributive Lov
- $(A+A')B=AB+A'B$ Distributive Lov
- $A_{mxn}I_{n}=I_{m}A_{mxn}=A$ Identitetsloven

### Eksempel
Man kan eventuelt bruge dette til lineære ligningssystemer.

$$A=\left[
\begin{array}{ccc}
2 & -3 & 1 \\ 
1 & 4 & -3
\end{array}
\right]$$
$$B=\left[
\begin{array}{c} 8 \\ 5
\end{array}
\right]$$
Højreside matricen.
$$X=\left[
\begin{array}{c}
x \\ y \\ z
\end{array}
\right]$$
$$AX=\left[
\begin{array}{ccc}
2 & -3 & 1 \\ 
1 & 4 & -3
\end{array}
\right]
\left[
\begin{array}{c}
x \\ y \\ z
\end{array}
\right]=
\left[
\begin{array}{ccc}
2x & -3y & z \\ 
x & 4y & -3z
\end{array}
\right]
$$
Vi kan altså skrive vores ligningssytem som $AX=B$
Hvis A har en invers da vil: $X=A^{-1}B$.



