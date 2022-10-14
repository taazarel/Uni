#forelæsning 
Begyndelsesdato: 07:54   13-10-2022   Uge-41
# Dagens emner
- Matrix invers
- Rang af matrix
- Invertible matricer
- Løse ligningssystemer med matrix invers
- Finde invers ved Gauss elimination

# Flashcards
Hvis det gælder at både A og B er kvadratiske og invertible af lige store dimensioner hvad gælder så for AB? 
?
det gælder at AB er invertibel
det gælder at $(AB)^{-1}=B^{-1}A^{-1}$

Hvis det gælder at både A og B er nxn matricer så gælder det at deres produkt er... :: både $AB=I$ og $BA=I$.

En invertibel matrix betyder... :: En matrix med præcis én Invers.

Den invertible af $A$ er $A^{-1}$, og den invertible af $A^{-1}$ er... :: $(A^{-1})^{-1}=A$

Man finder en matrix's invers gennem gauss elimination gennem... :: $[A|I]=[I|A^{-1}]$ 

Der findes tre forskellige slags af inverse matricer
?
Venstre invers givet ved $A_{mn}B_{nm}=I_{m}$
Højre invers givet ved $B_{nm}A_{mn}=I_{n}$
Den invertibles invers givet ved $AB=I_{m}$ og $AB=I_{n}$ givet $n=m$.

Rang af matricer er defineret som... :: $rang(A)=$ nummeret af ledende 1-tal.
Hvis en matrix har n ud af n ledende 1-tal siger man at dens rang er ... ::: en fuld rang.


# Matrix Invers
Givet er en matrix $A \in \mathbb{M}_{mn}$ 
1. Hvis der findes et $B \in \mathbb{M}_{nm}$ sådan at $AB=I_{m}$[^1] siger vi at B er en højre invers til A. (vi ganger den på fra højre side.)
2. Hvis der findes et $B \in \mathbb{M}_{nm}$ sådan at $BA=I_{m}$ kaldes B en venstre invers til A.
3. Hvis der findes et $B \in \mathbb{M}_{nm}$ så både 1 og 2 gælder så kaldes A invertibel og B kaldes en invers.[^2]
##### OBS: Når n=m og enten 1, eller 2 gælder så gælder den anden også for det samme B.

Hvis A har en venstre invers, dvs at $BA=I$ så vil ligningssystemet så vil $A \vec{x}=\vec{b}$ hvor $$A=\left[
\begin{array}{ccc}
a_{11} & ... & a_{1n} \\ 
: & : & : \\ 
a_{m1} & ... & a_{mn}
\end{array}
\right],
\vec{x}=
\left[
\begin{array}{c}
x_{1} \\ : \\ x_{n}
\end{array}
\right]
,\vec{b}=
\left[
\begin{array}{c}
b_{1} \\ : \\ b_{m}
\end{array}
\right]$$
så vil $A \vec{x}=\vec{b}$ have en løsning. 
$=B(A \vec{x})=B \vec{b}\Rightarrow (BA)\vec{x}=B \vec{b}\Rightarrow I \vec{x}=B \vec{b} \Rightarrow \vec{x}=B \vec{b}$ 
Vi har derfor konkluderet at hvis A har en venstre invers da vil $A \rightarrow (gauss) \rightarrow$ Række echelonform uden 0-rækker.

## Teorem 5.7
*En invertibel matrix har præcis én invers.*

### Bevis
Vi vil vise noget stærkere nemlig $AC=I_{m}$ og $BA=I_{n}$ giver at $B=C$.

$B=BI_{m}\Rightarrow B(AC)=(BA)C \Rightarrow I_{n}C=C$ 

## Teorem 5.8: Invers af Invers
Hvis A er invertibel, da er $A^{-1}$ også invertibel og $(A^{-1})^{-1}=A$ 

### Bevis
$(A^{-1})^{-1}$ er den matrix der opfylder at $A^{-1}(A^{-1})^{-1}=I$ og $(A^{-1})^{-1}A^{-1}=I$ men det passer for $(A^{-1})^{-1}=A$: da har vi at $A^{-1}A=I$ og $AA^{-1}=I$

## Teorem 5.9: Invers af Produkt
hvis $A,B \in \mathbb{M}_{nn}$ er invertible der er $AB$ invertibel og $(AB)^{-1}=B^{-1}A^{-1}$ (Husk rækkefølgen)

### Bevis
Vi skal tjekke at $(AB)(B^{-1}A^{-1})=A((BB^{-1})A^{1})= A(IA^{-1})=AA^{-1}=I$

# Gauss Elimination til at finde højre invers
C er højre invers af A, hvis $AC=I$. 
$$A=\left[
\begin{array}{ccc}
a_{11} & ... & a_{1n} \\ 
: & : & : \\ 
a_{m1} & ... & a_{mn}
\end{array}
\right],
C=\left[
\begin{array}{ccc}
c_{11} & ... & c_{1m} \\ 
: & : & : \\ 
c_{n1} & ... & c_{nm}
\end{array}
\right]$$
Hvor n,m er ubekendte.
$$C=\left[
\begin{array}{ccc}
| &   & | \\ 
\vec{c_{1}} & ... & \vec{c_{m}} \\ 
| &   & |
\end{array}
\right]$$
Dvs $$A \vec{c_{1}}=\left[
\begin{array}{c}
1 \\ 0 \\ : \\ 0
\end{array}
\right],A \vec{c_{2}}=
\left[
\begin{array}{c}
0 \\ 1 \\ : \\ 0
\end{array}
\right]
,...,A \vec{c_{m}}=\left[
\begin{array}{c}
0 \\ 0 \\ : \\ 1
\end{array}
\right]$$
m liningssystemer med m ligninger af n ubekendte.
De m ligningssytemer har alle A som koefficientmatrix. Vi kan løse dem alle ved at se på megaudvidedekoefficientmatricen.
$$\left[
\begin{array}{c|cccc}
A & 1 & 0 & ... & 0 \\ 
  & 0 & 1 & ... & 0 \\ 
  & : & : & ... & : \\ 
  & 0 & 0 & ... & 1
\end{array}
\right]=[A|I]$$
Vi anker hvis A er nxn: $[A|I]\rightarrow[I|A^{-1}]$ 

# Definition 5.10 (Rang af Matrix)
$rang(A)=rank(A)=$ antallet af ledende 1-taller efter Gauss elimination.

## Teorem 5.11 
Antallet af ledende 1-taller er uafhængige af valg af rækkeoperationer, så rangen er veldefineret.

## Teorem 5.12 (Eksistens af højre invers)
$A \in \mathbb{M}_{mn}$ har en højre invers hvis og KUN HVIS $rang(A)=m$. dvs der er et ledende 1-tal i hver række og $m \leq n$.

### Bevis (<=)
$$[A|I]\rightarrow \left[
\begin{array}{ccc|c}
1 & ... & 0 & * \\ 
0 & ... & 0 & * \\ 
0 & ... & 1 & *
\end{array}
\right]$$
Hvis $A \in \mathbb{M}_{nn}$ rang(A)=m så $[A|I]=[I|A^{-1}]$ 
Dvs $AC=I$ har mindst en løsning da der ikke er 0-rækker.

### Bevis (=>) 
Hvis der findes en højre invers så har ligningssystem $AC=I$ løsninger.
vi kunne have situationen
$$[A|I]=\left[
\begin{array}{ccc|ccc}
* & * & * & * & * & * \\ 
0 & ... & 0 & 0 & ... & 0
\end{array}
\right]$$
Det kan ikke lade sig gøre 
$$I=\left[
\begin{array}{ccc}
1 &... &  0 \\ 0  & ...& 1
\end{array}
\right]=\left[
\begin{array}{ccc}
* & * & * \\ 
0 & ... & 0
\end{array}
\right]$$
Hvilket er reduceret række echelon form. Dette er absurd hvis vi starter med I.

## Mirakel 5.13
Hvis $A,B$ er nxn matricer og $AB=I$ da vil $BA=I$.
### Bevis
$AB=I$ betyder at $[A|I]\rightarrow[I|C]$.
Hvis dette er sandt så kan vi finde at $[C|I]\rightarrow[I|A]$.
Derfor må A være højreinvers til C og C til A. Og derfor må $C=B$ da B var en højreinvers.



[^1]: I_m er identitetsmatricen til m rækker og kolonner
[^2]: Vi kommer til at se at det kræver n=m og at der kun kan være ét B