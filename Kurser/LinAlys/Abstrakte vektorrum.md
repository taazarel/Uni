#forelæsning 
Begyndelsesdato: 08:03   27-10-2022   Uge-43
# Flashcards
Disse antagelser skal være til stede for at man kan benytte sig af ekstremalværdisætningen... :: funktionen er lukket og begrænset under mængden, og funktionen er kontinuer på mængden. Så vil funktionen have ekstremum på mængden.
<!--SR:!2022-11-21,19,290-->

Man kan finde lineær uafhængighed ved at gausseliminere til reduceret echelon form, men hvordan er det sandt... :: Det er sandt fordi lineær uafhængighed er defineret som at spannet af vektorene kun har én måde at finde nulvektoren på. nemlig $r_{1}(1,1,0)+r_{2}(1,0,1)+r_{3}(0,1,1)=(0,0,0)$ medfører at $r_{1}=r_{2}=r_{3}=0$.
<!--SR:!2022-12-05,24,290-->


# Dagsplan
- Dimensionsteori
- Lineær uafhængighed

# Forelæsning
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
Et span af vektorer er bare mængden af vektorerne som vi vælger.
$\vec{v_{1}},\vec{v_{2}},..,\vec{v_{n}}$ vektorer i et vektorrum V.
spannet af disse er delmængden
spannet af vektorerne for alle linearkombinationer skrives således:
$span\{\vec{v_{1}},..,\vec{v_{n}}\}=\{r_{1}\vec{v_{1}}+...+r_{n}\vec{v_{n}}|r_{1},...,r_{n}\in \mathbb{R} \}$
altså mængden af alle linearkombinationer.

## Theorem 3.7 (span er underrum)
$span\{\vec{v_{1}},..,\vec{v_{n}} \}$ er et underrum.
### Bevis
- $span\{\vec{v_{1}},..,\vec{v_{n}} \}=\varnothing$ specielt $r_{1}=r_{2}=..=r_{n}=0$ dvs $\vec{o} \in span\{\vec{v_{1}},..,\vec{v_{n}} \}$ 
- Lukket under addition $(r_{1}\vec{v_{1}}+...+r_{n}\vec{v_{n}})+(s_{1}\vec{v_{1}}+...+s_{n}\vec{v_{n}})=(r_{1}+s_{1})\vec{v_{1}}+...+(r_{n}s_{n})\vec{v_{n}} \in span\{\vec{v_{1}},..,\vec{v_{n}} \}$ 
- lukket under multiplikation i $r \in \mathbb{R}$. $s(r_{1}\vec{v_{1}}+...+r_{n}\vec{v_{n}})=(sr_{1})\vec{v_{1}}+...+(sr_{n})\vec{v_{n}}\in span\{\vec{v_{1}},..,\vec{v_{n}} \}$

## Definition 3.8 (Lineær uafhængighed)
En endelig familie $\vec{v_{1}},\vec{v_{2}},...,\vec{v_{n}}$ af vektorer i et vektorrum kaldes lineært uafhængige hvis $r_{1}\vec{v_{1}}+...+r_{n}\vec{v_{n}}=\vec{o} \Rightarrow r_{1}=...=r_{n}=0$
$v_{1},...,v_{i}\in \mathbb{R}^{m}$, udspænder de hele $\mathbb{R}^{m}$? Er de lineært uafhængige?
Hvis man har en kvadratisk matrix vil den altid udspænde hvis den er lineært uafhængig. 
Da kvadratiske [[Matricer uden markovkæder|matricer]] kun udspænder hvis: Udspænder $<=>$ Ingen 0-række. og lineæruafhængig <=> ingen frie variable.

## Definition 2.41 (største/mindsteværdipunkter = max/min punkter)

$\vec{a}\in D_{f} \subseteq \mathbb{R}_{n}$ 
Hvor $D_{f}=$ definitionsmængden for $f:D_{f}\rightarrow \mathbb{R}$
punktet $\vec{a}$ kaldes et maxpunkt hvis $f(\vec{a})\geq f(\vec{x})$ for alle $\vec{x}\in D_{f}$
Punktet kaldes et min punkt hvis $f(\vec{a})\leq f(\vec{x})$ for alle $\vec{x}\in D_{f}$ 

## Ekstremalværdisætningen 2.42
Hvis $A \subseteq \mathbb{R}^{n}$ som er lukket og begrænset, og hvis $f:A \rightarrow \mathbb{R}$ er kontinuert så vil der være både makspunkter og minpunkter for f på mængden A.

## Theorem 3.9
Hvis man har $\vec{v_{1}},...,\vec{v_{n}}$ i et vektorrum V er lineært afhængige <=>[^2] en af vektorerne kan skrives som linearkombination af de øvrige.
### Bevis
Gennem lineær afhængighed:
Der findes $r_{1},...,r_{n}$ som ikke alle er 0, således at $r_{1}\vec{v_{1}}+...+r_{n}\vec{v_{n}}=\vec{o}$
Vi antager at $r_{i}\neq0$
$r_{i}\vec{v_{i}}=-r_{i-1}\vec{v_{i-1}}-r_{i+1}\vec{v_{i+1}}-...-r_{n}v_{n} \Rightarrow \vec{v_{i}}=\frac{1}{r_{i}}(-r_{i-1}\vec{v_{i-1}}-r_{i+1}\vec{v_{i+1}}-...-r_{n}v_{n})$

Gennem antagelse
$\vec{v_{i}}=r_{1}\vec{v_{1}}+...+r_{i-1}\vec{v_{i-1}}+r_{i+1}\vec{v_{i+1}}+...+r_{n}\vec{v_{n}}$
$\vec{o}=r_{1}\vec{v_{1}}+...+r_{i-1}\vec{v_{i-1}}-\vec{v_{i}}+r_{i+1}\vec{v_{i+1}}+...+r_{n}(\vec{v_{n}})$

## Sammenligningssætningen(3.15)

Et vektorrum V $\vec{v_{1}},...,\vec{v_{m}}$ udspænder V og $\vec{w_{1}},...,\vec{w_{n}}$, der er lineært uafhængig i V, da kan vi sige dette om størrelserne n og m... :: $m \geq n$.[^3]
<!--SR:!2022-12-09,28,300-->
### Bevis
Man kan bruge to matricer, en a matrix med mxn dimensioner og en c matrix med nx1 dimensioner.
Derefter viser man en modstrid med at $\vec{w_{1}},...,\vec{w_{n}}$ ikke er lineært uafhængig. Og derfor at der skal være flere rækker m, end søjler n når der gauss-elimineres i w's familie.

## Definition 3.12(Basis)

Vi har en basis af vektorer $\vec{v_{1}},...,\vec{v_{n}}$ i V når... :: Den både udspænder og er lineært uafhængig.
<!--SR:!2022-12-08,27,294-->

## Theorem 3.16
Givet $\vec{v_{1}},...,\vec{v_{m}}\text{ og }\vec{w_{1}},...,\vec{w_{n}}$ er baser da er deres dimensioner... :: $n=m$ kvadratiske.
<!--SR:!2022-12-13,32,303-->
Theorem 3.16 kan bevises med... :: Sammenligningssætningen.
<!--SR:!2022-11-16,9,280-->

## Definition 3.13(Dimension)
Dimensionen af et vektorrum V med en basis med n elementer har... :: n dimensioner og vi kan skrive $dimV=n$
<!--SR:!2022-12-07,26,294-->
### Eksempel
dimensionen af $\mathbb{R}^{n}$ kan skrives som... :: $dim \mathbb{R}^{n}=n$ da vi kan skrive en identitetsmatrix som er nxn.[^4]
<!--SR:!2022-12-11,30,300-->

## Definition 3.14 (Endelige og Uendelige vektorrum)

Et endeligt vektorrum defineres som...
Et uendeligt vektorrum defineres som...
?
Et vektorrum med en endelig base.
Alt som ikke er et endeligt vektorrum
<!--SR:!2022-12-06,25,294-->

## 3.17 (Udtyndningslemmaet)
Vektorrummet V udspændes af familien $\vec{v_{1}},...,\vec{v_{n}}$ givet $\vec{v_{j}}$ kan skrives som en linearkombination af de andre kan vi omdefinere til... :: $V=span \{\vec{v_{1}},...,\vec{v_{n}}  \}\cap \vec{v_{j}}$. Hvis $\vec{v_{1}}=\vec{v_{j}}$ kunne vi skrive; $V=span \{\vec{v_{2}},...,\vec{v_{n}} \}$
<!--SR:!2022-12-08,27,300-->

## 3.18 (Udtydningssætningen)
Familien $\vec{v_{1}},...,\vec{v_{n}}$ udspænder V, så kan man... :: Udtynde familien til en basis.
<!--SR:!2022-12-10,29,304-->
### Bevis
Familien skal være lin. uafhængig, hvis den starter der er vi færdige, ellers kan vi bruge... :: Udtyndingslemmaet da $dim V<n$ og derfor er $\vec{v_{1}},...,\vec{v_{n}}$ ikke lineært uafhængig. Så bruger vi bare 3.17. indtil $dim V=n$
<!--SR:!2022-12-15,30,280-->

## 3.19 (Udvidelseslemmaet)
Hvis vi har et span som $\vec{v_{n+1}}\notin span \{\vec{v_{1}},...,\vec{v_{n}} \}$ hvor spannet er lineært uafhængigt så vil spannet inkluderende $\vec{v_{n+1}}$... :: $\vec{v_{1}},...,\vec{v_{n}},\vec{v_{n+1}}$ være lineært uafhængigt.
<!--SR:!2022-11-29,18,284-->

## 3.20 (Udvidelsessætningen)
Hvis vi har en vektorfamilie $\vec{v_{1}},...,\vec{v_{n}}$ i et endeligt vektorrum med m, dimensioner, kan vi... :: udvide familien til en basis på m dimensioner.
<!--SR:!2022-12-12,31,300-->
### Bevis
Udvidelsesalgoritmen

## Sætning 3.22
Vi har $dim V=n$ og $\vec{v_{1}},...,\vec{v_{n}}$ er det en base hvis... :: den enten udspænder V eller er [[#Definition 3.8 (Lineær uafhængighed)|lineært uafhængig]].[^5]
<!--SR:!2022-11-16,9,274-->

## Definition 3.24 (Koordinater)
Givet er $B=[\vec{u_{1}},...,\vec{u_{n}}]$, som en ordnet basis for vektorrummet V kan vi definere $\vec{v}\in V$ som... :: $\vec{v}=r_{1}\vec{u_{1}}+...+r_{n}\vec{u_{n}}$, som en linearkombination. Dette kan omformuleres til... :: $[\vec{v}]_{B}=\left[\begin{array}{c}r_{1} \\:\\r_{n}\end{array}\right] \in \mathbb{R}^{n}$
<!--SR:!2022-11-16,9,283-->



[^1]: Men hvad nu hvis de x-værdier som man valgte havde løsninger? Så bruger vi eksemplet nedenunder.
[^2]: Betyder: Hvis og KUN hvis.
[^3]: Dette er dimensionsanalyse. DVS analyse af en matrix dimensioner.
[^4]: Alle identitetsmatricer er baser
[^5]: Den må derfor også være det modsatte samtidigt.