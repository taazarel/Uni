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


[^1]: Vi kan altså bytte om på dem, så længde at de står i samme rækkefølge.