#kapitel 
# §1.1 Talrummet $\mathbb{R}^{k}$
Vektorer er altid... :: søjler. Det kan godt være at de skrives som rækker i teksten, men de er stadigvæk søjler.
Givet to ortpgonale/vinkelrette vektorer $\vec{x}\cdot \vec{y}=0$ så vil $||x \cdot y||^{2}=...$:: $||x||^{2}+||y^{2}||$ 
### Cauchy-Schwarz ulighed
For to vektorer $\vec{x},\vec{y}\in \mathbb{R}^{k}$ kan vi opsætte en ulighed, selvom vi ikke normalt må gøre dette. Den skrives som... :: $|x \cdot y| \leq ||x|| \space ||y||$.
Trekants uligheden findes gennem Cauchy-Scwarz uligheden og skrives... :: $||x + y|| = ||x|| + ||y||$
Den omvendte trekantsulighed er... :: $|||x|| - ||y||| \leq ||x-y||$  

Ved lineære afbildninger kan vi lade C være en $m \times k$ matrice på $\mathbb{R}^{k}\to \mathbb{R}^{m}$ givet ved $\vec{x} \to C \vec{x}$.[^1] Afbildningen er lineær hvis... :: $C(\vec{x}+ \vec{y})=C \vec{x} + C \vec{y}$.
Lineære afbildninger opfylder denne ulighed $||C \vec{x}|| \leq$... :: $$\sqrt{\left(\sum_{i=1}^{m}\sum_{j=1}^{k} c_{ij}^{2}\right)}$$
## Definition 1.2
Normen/Længden af en vektor $\vec{x}\in \mathbb{R}^{k}$ er skrevet som... :: $||x|| = \sqrt{\vec{x}\cdot \vec{x}}$[^2]
En hyperplan bliver defineret som... :: $H = \{\vec{x}\cdot \vec{b}|\vec{x}\in \mathbb{R}^{k} \}$.

## Definition 1.9
En delmængde $A \subset \mathbb{R}^{k}$ er "Konveks" hvis det gælder for alle to punkter som ligger i delmængden at en linje tegnet mellem dem forbliver inde i delmængden totalt. Helt konkret skrives... :: $\lambda \vec{x}+(1-\lambda )\vec{y} \in A \text{ for alle }\vec{x},\vec{y}\in A, \lambda \in (0,1)$[^3]
Hvis en mængde er "Stjerneformet" omkring et punkt betyder det... :: at alle linjestykker som indeholder dette punkt er fuldkomment inde i mængden. Vi skriver $\lambda \vec{x_{0}}+(1-\lambda )\vec{y} \in A \text{ for alle }\vec{y}\in A, \lambda \in (0,1)$.


# §1.2 Topologiske begreber
## Definition 1.12 (Indre punkt)
Punktet $\vec{x}\in \mathbb{R}^k$ er et indre punkt i A, hvis der findes en kugle med punktet som centrum der er indeholdt i A. Matematisk kan vi skrive... :: $\exists \rho > 0: \space K(\vec{x}, \rho ) \subset A$.
## Definition 1.13 (kontaktpunkt)
Et punkt $\vec{x}\in \mathbb{R}^k$ er et kontaktpunkt for en mængde $A \subset \mathbb{R}^{k}$ hvis alle kugler omkring punktet indeholder mindst ét punkt af A[^4]. Vi definerer kontaktpunkter... :: $\forall \rho >0: \space K(\vec{x}, \rho ) \cap A \neq 0$.
## Definition (Afsluttede mængder)
Lad $A \subset \mathbb{R}^{k}$. Et punkt $\vec{x}\in \mathbb{R}^{k}$ er et kontaktpunkt for A hvis... :: $\forall \rho > 0 \exists \vec{y} \in A : ||\vec{y}-\vec{x}|| < \rho$

Hvad er Komplementærmængden... ::: alle punkter som mængden ikke er, $A^{c}=\mathbb{R}^{k}\backslash A$ 
Hvad er Randen af mængden... ::: Afslutningen af mængden uden de indre punkter $\delta A = \vec{A}\backslash A^{\circ}$.
Hvad er Afslutningen... ::: Mængden af kontaktpunkter for A. Skrives som $\vec{A}$.
En mængde er begrænset... :: når der findes en kugle omkring $\vec{0}$ som indeholder mængden.

# §1.3 Afbildninger fra $\mathbb{R}^{k}$ til $\mathbb{R}^{m}$



[^1]: Her er det vigtigt at x er en søjle med k tal
[^2]: Dette er altid muligt pga $\vec{x}\cdot \vec{x}\geq 0$.
[^3]: Lambda må ikke være defineret i 0 eller 1.
[^4]: Ja, hvis x er defineret i A kan man bare bruge dette som bevis.