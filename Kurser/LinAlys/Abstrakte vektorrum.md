#forelæsning 
Begyndelsesdato: 08:03   27-10-2022   Uge-43
# Flashcards

# Dagsplan
- Dimensionsteori
- Lineær uafhængighed

# Dimensionsteori
## Definition 3.2 (lineær kombination)
Hvis $\vec{v}_{1},...,\vec{v}_{n} \in V$ et vektorrum, da er en linearkombination af disse enhver ny vektor på formen:
$r_{1}\vec{v}_{1}+r_{2}\vec{v}_{2}+...+r_{n}\vec{v}_{n}$, hvor $r_{1}...r_{n} \in \mathbb{R}$.
Her kaldes $r_{1}...r_{n}$ koefficienterne for linearkombination.

### Eksempel
Er $e^{x}$ en linearkombination af $e^{2x},e^{3x}$ i $\mathbb{F}_\mathbb{R}$. Vi skal prøve at finde $r_{1},r_{2} \in \mathbb{R}$ så $e^{x}=r_{1}e^{2x}+r_{2}e^{3x}$ passer for alle x.

Vi starter med $e^{x}=r_{1}e^{2x}+r_{2}e^{3x} \Rightarrow 1=r_{1}e^{x}+r_{2}e^{2x}$ Her har vi altså 2 ligninger med tre ubekendte. 
Ifølge bogens metode:
$$\left[
\begin{array}{cc}
x=-1 &  1=r_{1}e^{-1}+2e^{-2} \\ 
x=0 & 1=r_{1}+r_{2} \\ 
x=1 & 1=r_{1}e+r_{2}e^{2}
\end{array}
\right]$$
Har ingen løsninger, derfor har vi bevist at dette ikke kan være et generelt tilfælde.[^1]

Man kan også bruge denne metode til at finde om der er en generel løsning.

$$1=\lim_{x \to \infty}(r_{1}e^{x}+r_{2}e^{2x})=\left[
\begin{array}{cc}
\infty & r_{2}>0 \\ 
-\infty & r_{2}<0 \\ 
\infty & r_{2}=0,r_{1}>0 \\
-\infty & r_{2}=0,r_{1}<0 \\ 
0 & r_{2}=0,r_{1}=0
\end{array}
\right]$$
Og derved kan vi se at dette ingen løsninger har for $r_{1},r_{2}$.

### Eksempel
Er $q(x)=x^{2}+x+2$ en linearkombination af $P_{1}(x)=x^{2}+5,P_{2}(x)=x^{2}+2x-1$?
Vi leder efter $r_{1},r_{2}\in \mathbb{R}$ så 
$q(x)=r_{1}P_{1}(x)+r_{2}P_{2}(x) \Rightarrow x^{2}+x+2=r_{1}(x^{2}+5)+r_{2}(x^{2}+2x-1)=(r_{1}+r_{2})x^{2}+2r_{2}x+5r_{1}-r_{2}$ Herefter kan vi opstille vores ligningssystem.
$$\left[
\begin{array}{c}
r_{1}+r_{2}=1 \\ 2r_{2}=1 \\ 5r_{1}r_{2}=2
\end{array}
\right]
=\left[
\begin{array}{cc|c}
1 & 1 & 1 \\ 
0 & 2 & 1 \\ 
5 & -1 & 2
\end{array}
\right]\rightarrow
\left[
\begin{array}{cc|c}
1 & 1 & 1 \\ 0 & 2 & 1 \\ 0 & -6 & -3
\end{array}
\right]\rightarrow
\left[
\begin{array}{cc|c}
1 & 1 & 1 \\ 0 & 2 & 1  \\ 0 & 0 & 0
\end{array}
\right]$$
Ja! q er en linearkombination af $P_{1},P_{2}$.

## Defintion 3.4 (Span)
$\vec{v_{1}},\vec{v_{2}},..,\vec{v_{n}}$ vektorer i et vektorrum V.
spannet af disse er delmængden
spannet skrives således:
$span\{\vec{v_{1}},..,\vec{v_{n}}\}=\{r_{1}\vec{v_{1}}+...+r_{n}\vec{v_{n}}|r_{1},...,r_{n}\in \mathbb{R} \}$
altså mængden af alle linearkombinationer.

## Theorem 3.7 (span er underrum)
$span\{\vec{v_{1}},..,\vec{v_{n}} \}$ er et underrum.
### Bevis
- $span\{\vec{v_{1}},..,\vec{v_{n}} \}=\varnothing$ specielt $r_{1}=r_{2}=..=r_{n}=0$ dvs $\vec{o} \in span\{\vec{v_{1}},..,\vec{v_{n}} \}$ 
- Lukket under addition $(r_{1}\vec{v_{1}}+...+r_{n}\vec{v_{n}})+(s_{1}\vec{v_{1}}+...+s_{n}\vec{v_{n}})=(r_{1}+s_{1})\vec{v_{1}}+...+(r_{n}s_{n})\vec{v_{n}} \in span\{\vec{v_{1}},..,\vec{v_{n}} \}$ 
- lukket under multiplikation i $r \in \mathbb{R}$. $s(r_{1}\vec{v_{1}}+...+r_{n}\vec{v_{n}})=(sr_{1})\vec{v_{1}}+...+(sr_{n})\vec{v_{n}}\in span\{\vec{v_{1}},..,\vec{v_{n}} \}$



[^1]: Men hvad nu hvis de x-værdier som man valgte havde løsninger? Så bruger vi eksemplet nedenunder.