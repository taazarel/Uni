#forelæsning 
Begyndelsesdato: Kl. 08:09  Den 06-12-2022   Uge-49
# Planen
- TK 2.5
- og 3.1
# TK § 2.5
## [[Retningsafledte#Partielt afledte funktioner|Partielt Afledte]] af f af *anden* orden
Vi kan finde partielt afledte af en højere orden således $$\frac{\delta^{2}f}{\delta x_{j}\delta x_{i}}=...$$:: $$\frac{\delta}{\delta x_{j}}\left(\frac{\delta f}{\delta x_{i}}\right)$$ 

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

## Hessematrix
Vi kan skrive alle muligheder for partielt afledte af en bestemt orden gennem en hessematrice. Vi bruger funktionen i eksempel 278: Det skrives således $$Hf(x,y)=...$$::$$\left[
\begin{array}{cc}2y^{3} & 6xy^{2} \\ 6xy^{2} & 6x^{2}y+2
\end{array}
\right] $$
### Hessematrix fortsat
Vi kan indsætte værdier i vores hessematrix. Lad os tage funktionen fra 278 som eksempel. Vi finder $Hf(0,0)=...$::$$\left[
\begin{array}{cc}0 & 0 \\ 0 & 2
\end{array}
\right] $$
## Definition 2.79
Lad $A \subseteq \mathbb{R}^{n}$ være åben, $r \in \mathbb{N}$. Så vil $f:A \to \mathbb{R}$ være $C^{r}$ funktion hvis... :: alle partielt afledte af orden $\leq r$ eksisterer og er kontinuerte.

## Sætning 2.82
Lad $A \subseteq \mathbb{R}^{n}$ være åben og $r \in \mathbb{N}$ og $f:A \to \mathbb{R}\text{ er }C^{2}$. For $i,j \in \{1,...,n \}$ har vi... :: En associations lov for alle $\vec{a} \in A$: $$\frac{\delta^{2}f}{\delta x_{i}\delta x_{j}}(\vec{a})= \frac{\delta^{2}f}{\delta x_{j}\delta x_{i}}(\vec{a})$$
### Udvidelse af 2.82
Hvis vi har $f \text{ er }C^{3}$ kan vi anvende... :: $$\frac{\delta^{3}f}{\delta x_{i}\delta x_{j}\delta x_{k}}= \frac{\delta^{3}f}{\delta x_{j}\delta x_{k}\delta x_{i}}$$[^1]
# TK § 3.1
## Definition af ekstremum
Størsteværdipunkt er det samme som... ::: Globalt maksimumspunkt: $$f(\vec{x})\leq f(\vec{a})\text{ for alle }\vec{x}\in A$$
Mindsteværdipunkt er det samme som... ::: Globalt minimumspunkt: $$f(\vec{x})\geq f(\vec{a})\text{ for alle }\vec{x}\in A$$

## Definition 3.1
Lad $f:A \to \mathbb{R},A \subseteq \mathbb{R}^{n}$ f har lokalt maksimum i $\vec{a}\in A$ hvis der findes... :: $r>0$ så $f(\vec{x})\leq f(\vec{a})$ for alle $\vec{x}\in A$ med $||\vec{x}-\vec{a}||<r$.[^2]

## Sætning 3.2
Hvis $f:A \to \mathbb{R}$, $A \subseteq \mathbb{R}^{n}$, hvis $\vec{a}\in A$ er lokalt ekstremumsværdi så er en af disse sandt... :: (i) $\vec{a}\in \delta A$ "Randpunkt", (ii) $\nabla f(\vec{a})$ eksisterer ikke "Singulære punkter", (iii) $\nabla f(\vec{a})=\vec{0}$ "Stationært punk"

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


# Fodnoter

[^1]: Vi kan altså bytte om på dem, så længde at de står i samme rækkefølge.
[^2]: ved uligheden om og så har vi et lokalt minimum