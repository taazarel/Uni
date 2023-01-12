#forelæsning 
Begyndelsesdato: Kl. 08:09  Den 06-12-2022   Uge-49
# Planen
- TK 2.5
- og 3.1
# TK § 2.5
## [[Retningsafledte#Partielt afledte funktioner|Partielt Afledte]] af f af *anden* orden
Vi kan finde partielt afledte af en højere orden således $$\frac{\delta^{2}f}{\delta x_{j}\delta x_{i}}=...$$:: $$\frac{\delta}{\delta x_{j}}\left(\frac{\delta f}{\delta x_{i}}\right)$$ 
<!--SR:!2023-03-22,71,290-->

<!--SR:!2023-01-09,26,294-->

### Eksempel 278
Et eksempel på partielt afledte af anden orden
$f(x,y)=x^{2}y^{3}+y^{2}$ 
$$\frac{\delta^{2}f}{\delta x \delta y}=...$$
$$\frac{\delta^{2}f}{\delta x^{2}}=...$$
$$\frac{\delta ^{2}f}{\delta y \delta x}=...$$
$$\frac{\delta^{2}f}{\delta y^{2}}=...$$
?
$$6xy^{2}$$
$$2y^{3}$$
$$6xy^{2}$$
$$6x^{2}y+2$$
<!--SR:!2023-01-31,42,294-->

## Hessematrix
Vi kan skrive alle muligheder for partielt afledte af en bestemt orden gennem en hessematrice. Vi bruger funktionen i eksempel 278: Det skrives således $$Hf(x,y)=...$$::$$\left[\begin{array}{cc}2y^{3} & 6xy^{2} \\ 6xy^{2} & 6x^{2}y+2\end{array}\right] $$
<!--SR:!2023-01-15,26,294-->

<!--SR:!2023-01-05,22,294-->
### Hessematrix fortsat
Vi kan indsætte værdier i vores hessematrix. Lad os tage funktionen fra 278 som eksempel. Vi finder $Hf(0,0)=...$::$$\left[\begin{array}{cc}0 & 0 \\ 0 & 2\end{array}\right] $$
<!--SR:!2023-04-20,98,323-->

<!--SR:!2023-01-06,23,301-->
## Definition 2.79
Lad $A \subseteq \mathbb{R}^{n}$ være åben, $r \in \mathbb{N}$. Så vil $f:A \to \mathbb{R}$ være $C^{r}$ funktion hvis... :: alle partielt afledte af orden $\leq r$ eksisterer og er kontinuerte.
<!--SR:!2023-01-13,24,294-->

<!--SR:!2022-12-28,14,274-->

## Sætning 2.82
Lad $A \subseteq \mathbb{R}^{n}$ være åben og $r \in \mathbb{N}$ og $f:A \to \mathbb{R}\text{ er }C^{2}$. For $i,j \in \{1,...,n \}$ har vi... :: En associations lov for alle $\vec{a} \in A$: $$\frac{\delta^{2}f}{\delta x_{i}\delta x_{j}}(\vec{a})= \frac{\delta^{2}f}{\delta x_{j}\delta x_{i}}(\vec{a})$$
<!--SR:!2023-04-16,94,314-->

<!--SR:!2022-12-25,11,250-->
### Udvidelse af 2.82
Hvis vi har $f \text{ er }C^{3}$ kan vi anvende... :: $$\frac{\delta^{3}f}{\delta x_{i}\delta x_{j}\delta x_{k}}= \frac{\delta^{3}f}{\delta x_{j}\delta x_{k}\delta x_{i}}$$[^1]
<!--SR:!2023-04-14,92,314-->

<!--SR:!2023-01-04,21,290-->
# TK § 3.1
## Definition af ekstremum
Størsteværdipunkt er det samme som... ::: Globalt maksimumspunkt: $$f(\vec{x})\leq f(\vec{a})\text{ for alle }\vec{x}\in A$$
<!--SR:!2023-01-13,24,303!2023-04-12,90,303-->

<!--SR:!2023-01-06,23,294!2022-12-12,4,274-->
Mindsteværdipunkt er det samme som... ::: Globalt minimumspunkt: $$f(\vec{x})\geq f(\vec{a})\text{ for alle }\vec{x}\in A$$
<!--SR:!2023-04-06,86,314!2023-01-14,25,303-->

<!--SR:!2023-01-08,25,290!2023-01-07,24,294-->

## Definition 3.1
Lad $f:A \to \mathbb{R},A \subseteq \mathbb{R}^{n}$ f har lokalt maksimum i $\vec{a}\in A$ hvis der findes... :: $r>0$ så $f(\vec{x})\leq f(\vec{a})$ for alle $\vec{x}\in A$ med $||\vec{x}-\vec{a}||<r$.[^2]
<!--SR:!2023-01-14,25,303-->

<!--SR:!2023-01-09,26,294-->

## Sætning 3.2
Hvis $f:A \to \mathbb{R}$, $A \subseteq \mathbb{R}^{n}$, hvis $\vec{a}\in A$ er lokalt ekstremumsværdi så er en af disse sandt... :: (i) $\vec{a}\in \delta A$ "Randpunkt", (ii) $\nabla f(\vec{a})$ eksisterer ikke "Singulære punkter", (iii) $\nabla f(\vec{a})=\vec{0}$ "Stationært punk"
<!--SR:!2023-03-25,74,294-->

<!--SR:!2022-12-22,8,234-->

### Eksempel 3.3
Givet er $f:\mathbb{R}^{2}\to \mathbb{R}$ og $f(x,y)=3xy-3x+9y$.
Lad os finde alle lokale maks. og min. 
En af de tre muligheder for 3.2 skal gælde. 
Mulighed 1 er umulig da vores domæne er større end codomænet. Den anden mulighed findes ikke da vi har en gradient.
Det betyder at vi skal finde gradienten.
$$\nabla f(x,y)=\left[
\begin{array}{c}3y-3 \\ 3x+9
\end{array}
\right] $$
Da vi ingen rand- og singulære punkter så må alle lokale maksimum og minimum være stationære.
Det skal altså være alle punkter for gradienten som giver $\nabla f(x,y)=\vec{0}$.
For dette eksempel er det $(x,y)=(-3,1)$.
Men vi skal lige tjekke at dette giver mening så lad os bruge
#### Konturmetode
$f(x,1)=3x-3x+9=9$
og $f(-3,y)=-9y+9+9y=9$
vi finder så punktet $(x,y)=(-3,1)+(t,t)$ og $(x,y)=(-3,1)+(t-t)$
Nu kan vi indsætte disse punkter i vores funktion 
$f(-3+t,1+t)=3t^{2}+9$ Er ikke et lokalt maksimum
$f(-3+t,1-t)=-3t^{2}+9$ Er ikke et lokalt minimum

## Parametriseringsmetoden
Vi ved hvordan vi finder et lokalt min, maks og sadelpunkter for stationære punkter, men vil også gerne vide det for randpunkter.
Givet er $A=D_{1}\subseteq \mathbb{R}^{2}$ hvor $D_{1}=[0,1]\times [0,1]=\{(x,y)\in \mathbb{R}^{2}|\begin{array}{c}0\leq x \leq 1 \\ 0 \leq y \leq 1\end{array} \}$. og funktionen $g:D_{1}\to \mathbb{R}$, $g(x,y)=3x^{2}-x-y+y^{2}$. $\delta D_{1}$ er fire linjestykker, for at finde randpunkterne som kunne være lokale ekstremum... :: parametriserer vi således $g(1,t)=3-1-t+t^{2}=t^{2}-t+2=f(t)$ Vi differentierer $\frac{df(t)}{dt}=2t-1$ og finder hvor $f'(t)=0$ hvilket er $\frac{1}{2}$. Så har vi kandidat til et ekstremum som hedder $(1,\frac{1}{2})$.[^3]
<!--SR:!2023-04-17,95,323-->
Parametriseringsmetoden er god at benytte når... :: Man har to variable, og kan gætte en parametrisering.
<!--SR:!2023-03-20,67,290-->

## Sætning 4.2 (Langranges multiplikatormetode)
Lad f og g være $C^{1}$ funktioner $A \to \mathbb{R},A \subseteq \mathbb{R}^{n}$ (er åben).
Givet er $S=\{\vec{x}\in A|g(\vec{x})=c \},c \in \mathbb{R}$.
Hvis $\vec{a}\in S$ er et lokalt ekstrema for $f:S \to A$ (betyder f på S), så er enten...
?
(i) $\nabla g(\vec{a})=0$
(ii) $\nabla f(\vec{a})=\lambda \nabla g(\vec{a})$ for et $\lambda \in \mathbb{R}$[^4]

Langranges multiplikatormetode giver... :: kandidater til ekstrema, ikke ekstrema i sig selv.
<!--SR:!2023-03-21,68,294-->

## Ligevægtspunkter
Antag at $\vec{x}(t)$ opfylder $\frac{d^{2}}{dt^{2}}\vec{x}(t)=-\nabla V(\vec{x}(t))$ hvor $V:\mathbb{R}^{n}\to \mathbb{R}$. Da vil $$V(\vec{x})=-G \sum \frac{m_{i}}{|\vec{x}-\vec{x}_{i}|}$$Får vi konstante løsninger $\vec{x}(t)=\vec{v} \leftrightarrow \nabla V(\vec{v})=\vec{0}$
Hvis $\vec{v}$ er lokalt min...
Hvis $\vec{v}$ er lokalt max...
?
Får vi en stabil ligevægt
Får vi en ustabil ligevægt[^5]
<!--SR:!2023-01-16,4,306-->

## Sætning 3.4 (ABC kriteriet)
Lad $D=det(Hf(\vec{a}))$ altså determinanten til hessematricen af et punkt a.
Og lad $A$ være egenværdien af hessematricen. $A \vec{x}=\lambda \vec{x}$.
Så får vi tre sandheder
1. Hvis D<0...
2. Hvis D>0 og A>0...
3. Hvis D>0 og A<0...
?
Så er $\vec{a}$ et sadelpunkt
Så er $\vec{a }$ et lokalt minimumspunkt
Så er $\vec{a }$ et lokalt maximumspunkt

### Udvidelse af ABC kriteriet
1. Hvis alle [[Egenværdier]] for $Hf(\vec{a})$ er positive...
2. Hvis alle egenværdier for $Hf(\vec{a})$ er negative...
3. Hvis mindst en egenværdi er positiv og mindst en er negativ...
?
1. Så er $\vec{a}$ et lokalt min.
2. Så er $\vec{a}$ et lokalt max.
3. Så er $\vec{a}$ et sadelpunkt.
<!--SR:!2023-01-15,3,286-->

# Fodnoter
[^1]: Vi kan altså bytte om på dem, så længde at de står i samme rækkefølge.
[^2]: ved uligheden om og så har vi et lokalt minimum
[^3]: Her valgte vi (1,t) da dette er den højre kant af firkanten, hvor vi ikke ved hvad y skal være. (Funktionen tegnes inden i en firkant da den er defineret i D_1)
[^4]: Har n ligninger i n+1 variable hvilket er $(a_{1},...,a_{n},\lambda )\in \mathbb{R}$.
[^5]: Disse to beskriver mange fænomen i fysik. Fx tyngdekraft og elektromagnetiske felter.