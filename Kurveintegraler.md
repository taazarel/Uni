#kapitel 
# §7.1 Kurvebegrebet
## Definition 7.1
En kontinuert afbildning $r:I \to \mathbb{R}^{k}$ af et interval $I \to \mathbb{R}$ kaldes... :: en **parameterfremstilling** for en kontinuert **kurve**. Hvis r er en $C^{n}$ afbildning er det en $C^{n}$-kurve.

## Definition 7.5 (Reparametrisering)
Lad $r: I \to \mathbb{R}^{k}$ og $\hat r:J \to \mathbb{R}^{k}$ være parameterfremstillinger. De har samme **kurve** når... :: der findes en **reparametrisering**, hvilket er en strengt voksende og surjektiv funktion $\phi :J \to I$ så $r(\phi (u))=\hat r(u)$ for alle $u \in J$.

# §7.3 Kurvelængde
## Definition 7.17 (Kurvelængde)
For en kontinuert kurve $r: [a,b]\to \mathbb{R}^{m}$ med begrænset, afsluttet parameterinterval er **kurvelængden** givet som... :: $l=sup \{l(D)|D \text{ endelig inddeling af [a,b]} \}$ hvis $l<\infty$ så er kurven **rektificerbar**.

### Sætning 7.19
Hvis en kurve som er stykkevist $C^{1}$ så er dens længde... :: $l=\int_{a}^{b}||r'(t)||dt$ og den er også altid rektificerbar.

### Ingredienser for kurveintegralet
- lad $\Omega \subset \mathbb{R}^{k}$ være en åben mængde og lad $V:\Omega \to \mathbb{R}^{k}$ være et vektorfelt.

## Kurveintegral for stykkevist $C^{1}$-kurve.
Hvis $V:\Omega \to \mathbb{R}^{k}$ er et kontinuert vektorfelt og hvis $r:[a,b]\to \Omega$ er en stykkevist $C^{1}$ kurve så eksisterer kurveintegralet... :: $$\int_{\gamma}^{} V \cdot dr= \int_{a}^{b} V(r(t))\cdot r'(t)dt$$
