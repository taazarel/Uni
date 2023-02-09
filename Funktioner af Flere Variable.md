#kapitel 
Givet to ortonormale vektorer $\vec{x}\cdot \vec{y}=0$ så vil $||x \cdot y||^{2}=...$:: $||x||^{2}+||y^{2}||$ 
### Cauchy-Schwarz ulighed
For to vektorer $\vec{x},\vec{y}\in \mathbb{R}^{k}$ kan vi opsætte en ulighed, selvom vi ikke normalt må gøre dette. Den skrives som... :: $|x \cdot y| \leq ||x|| \space ||y||$.
Trekants uligheden findes gennem Cauchy-Scwarz uligheden og skrives... :: $||x + y|| = ||x|| + ||y||$
Den omvendte trekantsulighed er... :: $|||x|| - ||y||| \leq ||x-y||$  

Ved lineære afbildninger kan vi lade C være en $m \times k$ matrice på $\mathbb{R}^{k}\to \mathbb{R}^{m}$ givet ved $\vec{x} \to C \vec{x}$.[^1] Afbildningen er lineær hvis... :: $C(\vec{x}+ \vec{y})=C \vec{x} + C \vec{y}$.
Lineære afbildninger opfylder denne ulighed $||C \vec{x}|| \leq$... :: $$\sqrt{\left(\sum_{i=1}^{m}\sum_{j=1}^{k} c_{ij}^{2}\right)}$$
# Topologiske begreber
## Definition
Lad $A \subset \mathbb{R}^{k}$ være en mængde. Vi har et pukt $\vec{x}\in A$ som er et indre punkt hvis der findes et $\rho > 0$ så får vi... :: $||\vec{y}-\vec{x}||<\rho \Rightarrow y \in A$.
## Definition (Afsluttede mængder)
Lad $A \subset \mathbb{R}^{k}$. Et punkt $\vec{x}\in \mathbb{R}^{k}$ er et kontaktpunkt for A hvis... :: $\forall \rho > 0 \exists \vec{y} \in A : ||\vec{y}-\vec{x}|| < \rho$    

## Strategi til Epsilon delta gymnastik
- Hav et gæt, eller tanke om hvad grænseværdien b er.
- Undersøg relationen mellem $|f(x)-b| \text{ og } |x-a|$.
- Vælg så en "Afpareringsstrategi"
### True strike formel
Der er en række kriterier som skal opnåes før vi kan få en sikker gevinst.
1. Kriterie; Hvis det gælder for et passende C > 0 gælder at: $|f(x)-b| \leq C|x-a|$ for alle $x \in I \backslash \{ a\}$. Kan man parere ved...
?
- at vælge $\delta = \delta (\epsilon )= \frac{\epsilon}{C}$ for et givet $\epsilon >0$. Hvis $|x-a|<\delta$
- 

## Definition (Grænseværdi 1D)
Lad $f : I \backslash \{ a\}\to \mathbb{R}$ hvor $a \in I$ er et indre punkt i intervallet I, og lad $b \in \mathbb{R}$. Hvis det gælder at $\forall \epsilon > 0 \exists \delta >0$ : $|f(x)-b| < \epsilon$ for alle $x \in I \backslash \{ a\}$ med $|x-a|< \delta$. Så vil f have b som "grænseværdi" i "grænseovergangen" $x \to a$ og dette skrives som... ::: $f(x)\to b$ for $x \to a$




[^1]: Her er det vigtigt at x er en søjle med k tal