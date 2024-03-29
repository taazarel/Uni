#kapitel 
# §5.1 Riemann-integralet
Riemann integralet betegnes ved et at dele et interval op i kasser op til funktionen for at markere arealet således... :: for et tal $I \in \mathbb{R}$ og $f:[a,b]\to \mathbb{R}$ $\forall \epsilon > 0\space \exists \delta >0:$  $$|I - \sum_{i=1}^{n}f(\xi_{i})\Delta x_{i}| < \epsilon$$ hvor summen er middelsummen M. (5.1). Hvis f er integrabel så kaldes I for integralet af f, og betegnes $$\int_{a}^{b} f(x) \space dx$$
Hvis f er riemann integrabel så er... :: funktionen både begrænset og integralet I er entydigt.

## Trekantsuligheden for integraler sætning 5.10
Trekantsuligheden for integraler siger at... :: Den absolutte værdi for integralet er mindre end integralet til den absolutte værdi af f. $$|\int_{a}^{b} f(x) dx| \leq \int_{a}^{b}|f(x)|dx$$

## Indskudsreglen sætning 5.11
Hvis f er integrabel over to intervaller som overlapper vil f... :: også være integrabel over hele intervallet. $$\int_{a}^{b}f(x)dx = \int_{a}^{c} f(x)dx + \int_{c}^{b} f(x)dx$$
## Bolzano-egenskaben
En funktion har Bolzano-egenskaben hvis... :: $\forall \epsilon >0 \exists \delta >0:$ $$|\sum_{i=1}^{n}f(\xi_{i})\Delta x_{i} - \sum_{j=1}^{m}f(\eta_{j})\Delta y_{j}| < \epsilon $$ har en $finhed(D)<\delta$ og $finhed(D')<\delta$. [^1]
Hvis en funktion er kontinuert... :: har den Bolzano egenskaben.

# §5.5 Stamfunktionsproblemet
## Definition 5.28
Givet en funktion på I så er dens stam... :: -funktion kontinuert på I og skrives $F'(x)=f(x)$.

## Sætning 5.29 (Infinitesimalregningens hovedsætning)
Lad $f:I \to \mathbb{R}$. Hvis f er kont. i alle punkter så har f en stamfunktion, nemlig... :: $\Phi (x)= \int_{x_{0}}^{x}f(y)dy$ for $x \in I$. Dette betyder altså at der er sammenhæng mellem stamfunktionen/integraler og differentialer.

### Uegentlig integral / improper integral
Vi kan integrere for svære/åbne intervaller ved... :: at bruge uegentlige integraler. Altså at substituere uendeligt med en grænse, eller indsætte -$\epsilon$ ved den åbne grænse.



[^1]: Denne Bolzano egenskab er essentielt det samme som Riemann integrabilitet. Hvis en funktion har Bolzano egenskaben er den altid også Riemann integrabel, og vice versa.