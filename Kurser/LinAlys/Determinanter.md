#forelæsning 
Begyndelsesdato: Kl. 08:08  Den 08-12-2022   Uge-49
## Definition 6.8 (Isometrier)
En isometri fra V til W er en... :: lineær afbildning af $T:V \to W$ som er både injektiv og surjektiv.
<!--SR:!2022-12-18,4,270-->
V og W er isomorfe hvis der eksisterer... :: en isometri mellem dem $V \to W$.
<!--SR:!2022-12-18,4,270-->
Vi kan skrive isometri således på papir... :: $T: \mathbb{P}_{3}\to \mathbb{R}^{4}$. hvor $a_{3}x^{3}+...+a_{0}x^{0}\rightarrow (a_{0},...,a_{3})\text{ eller }(a_{3},...,a_{0})$.
<!--SR:!2022-12-18,4,270-->

## Sætning
Lad V og W være end. dim. Da er V og W isomorfe hvis og kun hvis... :: $dim(V)=dim(W)$.
<!--SR:!2022-12-18,4,270-->


# Messer §7.1 Induktionsbevis
Induktionsbeviser er en metode til at bevise påstande for alle $n \in \mathbb{N}$. Den går således: Påstand $S_{n}$ er sand og $S_{n}\Rightarrow S_{n+1}$ er sandt, så er... :: $S_{n}$ sandt for alle $n \in \mathbb{N}$.
<!--SR:!2022-12-18,4,270-->
### Eksempel for induktiontionsbevis
$$\sum_{j=1}^{n}(2j-1)=n^{2}$$ Summen for alle ulige tal er antallet af tallene i anden. Dette er vores $S_{n}$. Vi kan vise at dette passer for $S_{1}$: $$\sum_{j=1}^{n}(2(1)-1)=1^{2}$$ er altså sandt.
Vi kan nu vise at det gælder for vores n+1.
$$\sum_{j=1}^{n+1}(2j-1)=\left(\sum_{j=1}^{n}(2j-1)\right)+2(n+1)-1=n^{2}+(2n+1)=(n+1)^{2}$$
Vi har nu bevise at $S_{n+1}$ er sandt, og derfor må dette gælde for alle ulige naturlige tal.

## §7 Determinanter
## Definition
Determinanten defineres som en transformation på en matrice $det:\mathbb{M}_{n,n}\to \mathbb{R}$. Determinanten skrives således på
En 2x2 matrice...
En 3x3 matrice...
En generisk matrice...
?
En 2x2 matrice:
$$det(\vec{a},\vec{b})=det\left[
\begin{array}{cc}a_{1} & b_{1} \\ a_{2} & b_{2}
\end{array}
\right] =a_{1}b_{2}-a_{2}b_{1}$$
En 3x3 matrice:
$$det(\vec{a},\vec{b},\vec{c})=det\left[
\begin{array}{ccc}a_{1} & b_{1} & c_{1} \\ a_{2} & b_{2} & c_{2} \\ a_{3} & b_{3} & c_{3}
\end{array}
\right]$$$$=a_{1}\cdot det \left[
\begin{array}{cc}b_{2} & c_{2} \\ b_{3} & c_{3}
\end{array}
\right] -b_{1}\cdot det \left[
\begin{array}{cc}a_{2} & c_{2} \\ a_{3} & c_{3}
\end{array}
\right] +c_{1}\cdot det \left[
\begin{array}{cc}a_{2} & b_{2} \\ a_{3} & b_{3}
\end{array}
\right] $$
En generisk matrice:[^1]
$$det(A)=\sum_{j=1}^{n}(-1)^{1+j}a_{1j}\cdot det(A_{1j})$$
Hvor matricen $$A=\left[
\begin{array}{ccc} a_{11} & a_{12} & ... \\ a_{21} & a_{22} & ... \\ \vdots & \vdots & \vdots
\end{array}
\right] $$

## Sætning 7.6 (Rækkeoperationer i matricer)
Lad $A \in \mathbb{M}_{n,n}$. Givet er følgende regler givet for sammenhængen mellem diskriminanten og rækkeoperationer.
(I) Hvis A har en nulrække er... 
(II) Hvis $A \to A'$ og $R_{i}\leftrightarrow R_{j}$  er... 
(III) hvis $A \to A',c \in \mathbb{R}$ og $cR_{i} \to R_{i}$ er... 
(IV) Hvis A har to ens rækker er... 
(V) Hvis $A \to A'$ og $cR_{i} +R_{j} \to R_{j}$ er... 
(VI) Determinanten af I er...  
?
$det(A)=0$ 
$det(A')=-det(A)$ 
$det(A')=c\cdot det(A)$ 
$det(A)=0$
$det(A')=det(A)$
$det(I)=1$[^2]

## Sætning 7.7
Definition af den generelle formel for determinanten af en matrice.
Givet $A \in \mathbb{M}_{n,n}$ og $r,k \in \{1,...,n \}$ så er det(A)=...
?
$$\sum_{k=1}^{n}(-1)^{r+k}a_{rk}\cdot det(A_{rk})$$[^3]

## Sætning 7.9[[Lineære Afbildninger]]
Hvis $A,B \in \mathbb{M}_{n,n}$ så er $det(AB)=...$::$det(A)det(B)$
<!--SR:!2022-12-18,4,278-->

## Definition for transponering
For $A \in \mathbb{M}_{n,n}$, sæt $A^{t}=...$:: matricen hvis (i,j)-te indgang er $a_{ji}$. Altså en spejlbildning i diagonalen.
<!--SR:!2022-12-18,4,278-->

## Sætning 7.12
$det(A^{t})=...$::$det(A)$.
<!--SR:!2022-12-18,4,278-->

## Sætning 7.13 (Konsekvens af 7.6)
Hvis vi kan reducere en matrice $A \in \mathbb{M}_{n,n}$ så vil determinanten... :: Ikke være nul da $A \to ... \to I$ gennem rækkereduktion[^4], og $det(I)\neq 0$ så for at få dette må $det(A)\neq 0$.

## Formel for $A^{-1}$ 7.4
Givet $A_{ij}\in \mathbb{M}_{n-1,n-1}$. Definition: Lad $A \in \mathbb{M}_{n,n}$ så bliver  $adj(A)\in \mathbb{M}_{n,n}$ til matricen hvis indgang $(i,j)$... :: $(-1)^{i+j}det(A_{ji})$.[^5] 

## Sætning 7.14
For alle $A \in \mathbb{M}_{n,n}$ så er $adj(A)=...$ :: $$adj(A)=\left[\begin{array}{ccc}det(A_{11}) & ... & (-1)^{n+1}det(A_{n1}) \\ \vdots &   & \vdots \\ (-1)^{1+n}det(A_{1n}) & ... & (-1)^{n+n}det(A_{nn})\end{array}\right]$$

## Sætning 7.15
Givet $adj(A)A=det(A)I \in \mathbb{M}_{n,n}$, Hvis $A \in \mathbb{M}_{n,n}$ har invers er dens invers defineret ved... :: $$A^{-1}=adj(A)/det(A)$$ Hvilket vi også kan skrive som $(A^{-1})_{ij}= (-1)^{i+j}det\frac{A_{ji}}{det(A)}= \frac{\text{Sum af +/- produkter af indgange}}{\text{Sum af +/- produkter af indgange}}$

## Krydsprodukt på flere end to dimensioner
Definitionen af et krydsprodukt er det samme som determinanten, med vektorerne som søjler... :: uden dens skalarer. Så i tre dimensioner ville det være $$\vec{v}\times \vec{w}=det\left(\left[
\begin{array}{cc}v_{2} & w_{2} \\ v_{3} & w_{3}
\end{array}
\right] \right),-det\left(\left[
\begin{array}{cc}v_{1} & w_{1} \\ v_{3} & w_{3}
\end{array}
\right] \right),det\left(\left[
\begin{array}{cc}v_{1} & w_{1} \\ v_{2} & w_{2}
\end{array}
\right] \right)$$[^6]

## Sætning 7.18 "Algebraiske egenskaber for Krydsprodukt"
Vi har disse egenskaber for krydsprodukter
1. $\vec{v}\times \vec{w}=...$
2. $\vec{v}\times (\vec{w}+\vec{x})=...$
3. $(\vec{v}+\vec{w})\times \vec{x}=...$
4. $r(\vec{v}\times \vec{w})=...$
5. $\vec{v}\times \vec{0}=...$
6. $\vec{v}\times \vec{v}=...$
7. $\vec{v}\cdot (\vec{w}\times \vec{x})$
?
$-\vec{w}\times \vec{v}$
$\vec{v}\times \vec{w}+\vec{v}\times \vec{x}$
$\vec{v}\times \vec{x}+\vec{w}\times \vec{x}$
$(r \vec{v})\times \vec{w}=\vec{v}\times (r \vec{w})$
$\vec{0}=\vec{0}\times \vec{v}$
$\vec{0}$
$det\left(\left[\begin{array}{ccc}- & \vec{u} & - \\ - & \vec{v} & - \\ - & \vec{w} & -\end{array}\right] \right)=(\vec{v}\times \vec{w})\cdot \vec{x}$

## Sætning 7.19 "Geometriske egenskaber af krydsprodukt"
1. $\vec{v}\cdot (\vec{v}\times \vec{w})=\vec{0}$
2. $\vec{w}\cdot (\vec{v}\times \vec{w})=\vec{0}$
3. $||\vec{v}\times \vec{w}||^{2}=...$
4. $||\vec{v}\times \vec{w}||=...$
?
$\vec{0}$
$\vec{0}$
$||\vec{v}||^{2}||\vec{w}||^{2}-(\vec{v}\cdot \vec{w})^{2}$
$||\vec{v}||||\vec{w}||\sin{(\theta )}$

## Orientering af baser
Ordnede baser, $B = [\vec{u_{1}},\vec{u_{2}},\vec{u_{3}}] \in \mathbb{R}^{3}$ inddeles i... :: højrehåndede $det(B)>0$ og venstrehåndede $det(B)<0$ baser.

### Operation på base
$T:\mathbb{R}^{3}\to \mathbb{R}^{3}$ lineær $T(\vec{x})=A \vec{x}$ hvor $A \in \mathbb{M}_{3,3}$. Givet at T er isomorf $\Leftrightarrow$ A har invers $\Leftrightarrow$ $det(A)\neq 0$ så er operationen på basen B... :: $T(B)=B'=[T(\vec{u_{1}}),T(\vec{u_{2}}),T(\vec{u_{3}})]$ også en basis og har samme orientering som B.

## Kryds notation
givet $\vec{v},\vec{w} \in \mathbb{R}^{3}$ så bliver $$det\left[
\begin{array}{ccc}
\vec{i} & \vec{j} & \vec{k} \\ 
\vec{v_{1}} & \vec{v_{2}} & \vec{v_{3}} \\ 
\vec{w_{1}} & \vec{w_{2}} & \vec{w_{3}}
\end{array}
\right]=\vec{v}\times \vec{w}$$ Og dette giver kun mening hvis... :: $\vec{i}=\vec{e_{1}}=(1,0,0)$ $\vec{j}=\vec{e_{2}}$ og $\vec{k}=\vec{e_{3}}$

## Cramers formel
For løsninger til $A \vec{x}=b$, når $t \in \mathbb{R}^{n}$ og $A \in \mathbb{M}_{n,n}$ så er $\vec{x}=...$ :: $A^{-1}b= \frac{1}{det(A)}adj(A)b \Rightarrow x_{j}= \frac{det(A_{j})}{det(A)}, A_{j}\in \mathbb{M}_{n,n}$.


# Fodnoter
[^1]: Dette bliver til en sum af n! led. Så for en 3x3 matrice er det 6 led. Denne formel er meget upraktisk for en datalogisk synspunkt, men kan godt bruges til at give en definition på determinanten.
[^2]: I er identitetsmatricen. Dette kan altså fortælle os hvad determinanten bliver når man reducerer. Enten får man en nulrække eller to ens rækker, og så er det nul, eller også finder man I.
[^3]: r=1 er definitionen af determinanten.
[^4]: her benytter vi 7.6 definitionen til at reducere lettere.
[^5]: Hvor $A=\left[\begin{array}{ccc}a_{11} & ... & a_{1n} \\ \vdots  &   & \vdots \\ a_{n1} & ... & a_{nn}\end{array}\right]$.
[^6]: Husk at $$det\left[
\begin{array}{ccc}- & \vec{u} & - \\ - & \vec{v} & - \\ - & \vec{w} & -
\end{array}
\right] =det \left[
\begin{array}{ccc}| & | & | \\ \vec{u} & \vec{v} & \vec{w} \\ | & | & |
\end{array}
\right] $$