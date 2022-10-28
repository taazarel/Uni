# 1
## a
Afgør om polynomierne 
$p_{1}(x)=x^{2}-1,p_{2}(x)=2x^{2}+x,p_{3}(x)=x+1$
er lineært uafhængige i funktionsrummet $\mathbb{F}_{\mathbb{R}}$.
Hvis disse polynomier er lineært uafhængige i $\mathbb{F}_{\mathbb{R}}$, så ville de ingen frie variable have i en række-echelon form, med en vilkårlig polynomie i $\mathbb{F}_{\mathbb{R}}$.
altså:
$r_{1}(x^{2}-1)+r_{2}(2x^{2}+x)+r_{3}(x+1)=ax^{2}+bx+c$, hvor $r_{1},r_{2},r_{3}\in \mathbb{R}$. 
Hvilket vi kan omskrive til tre ligninger med tre ubekendte.
$$
\begin{array}{c}
r_{1}+r_{2}=a \\ r_{2}+r_{3}=b \\ -r_{1}+r_{3}=c
\end{array}
$$
Og derefter skrive som en koefficientsmatrice.
$$\left[
\begin{array}{ccc|c}
1 & 2 & 0 & a \\ 0 & 1 & 1 & b \\ -1 & 0 & 1 & c
\end{array}
\right]\to
\left[
\begin{array}{ccc|c}
1 & 2 & 0 & a \\ 0 & 1 & 1 & b \\ 0 & 0 & -1 & c+a-2b
\end{array}
\right]\to
\left[
\begin{array}{ccc|c}
1 & 2 & 0 & a \\ 0 & 1 & 0 & b+c+a-2b \\ 0 & 0 & 1 & 2b-a-c
\end{array}
\right]$$
$$\to
\left[
\begin{array}{ccc|c}
1 & 0 & 0 & a-2(b+c+a-2b) \\ 0 & 1 & 0 & b+c+a-2b \\ 0 & 0 & 1 & 2b-a-c
\end{array}
\right]\to
\left[
\begin{array}{ccc|c}
1 & 0 & 0 & 2b-a-2c \\ 0 & 1 & 0 & a+c-b \\ 0 & 0 & 1 & 2b-a-c
\end{array}
\right]$$
Vi kan herved se at:
- Der er ingen frie variabler da:
	- $r_{1}=2b-a-2c$
	- $r_{2}=a+c-b$
	- $r_{3}=2b-a-c$
- Derfor må polynomierne være lineært uafhængige i funktionsrummet $\mathbb{F}_{\mathbb{R}}$. 
## b
Vis, at det underrum i $\mathbb{F}_{\mathbb{R}}$, der udspændes af polynomierne i (a) udgøres af alle polynomier af grad højst 2 dvs. af $\mathbb{P}_{2}$ 

Vi kalder $span(p_{1},p_{2},p_{3})=V$. Vi skal herved vise at mængden $V=\mathbb{P}_{2}$, hvor $V,\mathbb{P}_{2} \subseteq \mathbb{F}_{\mathbb{R}}$.
Nu kan vi finde et vilkårligt polynomie af højst 2 grad, dvs. 2 grad: $ax^{2}+bx+c \in \mathbb{P}_{2}$. Hvis det er sandt at V udspænder hele $\mathbb{P}_{2}$ så må der findes $r_{1},r_{2},r_{3} \in \mathbb{R}$ som gør 
$r_{1}(p_{1})+r_{2}(p_{2})+r_{3}(p_{3})=ax^{2}+bx+c$, et sandt udtryk.

Men dette har vi jo netop bevist i (a). Så hermed kan vi se at underrummet som V spanner i $\mathbb{F}_{\mathbb{R}}$ er det samme som alle polynomier af 2 grad, dvs. $V=\mathbb{P}_{2}$.

# 2
## a

## b

# 3
## a

## b
For at gøre det let for os selv bruger vi bare forslaget i opgaven, dvs. $m=1, c=300$.
Vi benytter os af python til at finde taylorpolynomierne af 4 og 