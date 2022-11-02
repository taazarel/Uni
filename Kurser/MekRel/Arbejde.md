#forelæsning 
Begyndelsesdato: 16:21   30-10-2022   Uge-43
# Forberedelse
## Spørgsmål
I 6.4.1, hvorfor skal vi ikke se på den potentielle energi i systemet? Den ændres jo da barnet bliver løftet opad.
Er der ikke også en fortegnsfejl i opgaven, specifikt (6.28)
## [[Kraft]] og [[energi]] (6.1)

Arbejde(Eller energiligningen) beskrives som... :: energiændringen af systemet når det bliver påvirket af en ydre kraft: $W=\triangle E=\triangle K+\triangle U$.
<!--SR:!2022-11-03,3,250-->
I et lukket system... ::: $W=0$
<!--SR:!2022-11-04,4,270!2022-11-04,4,277-->

Arbejdets fortegn beskriver overførslen af energi således...
?
$W>0$ er en overførsel af energi til systemet
$W<0$ er en afgivelse af energi fra systemet
$W=0$ er energikonstanthed i systemet
<!--SR:!2022-11-04,4,277-->

Arbejdet er afhængig af denne størrelse... :: $(\triangle x_{F})$. Hvor $\triangle x_{F}$ er forskydningen af systemets massemidtpunkt.[^1]
<!--SR:!2022-11-04,4,277-->

Kraftens arbejde er positivt når... :: kraften peger samme vej som forskydningen af kontaktpunktet ![[Arbejde 2022-10-30 17.03.20.excalidraw]]
<!--SR:!2022-11-04,4,270-->
Kraftens arbejde er negativt når... :: kraften peger modsatte vej af forskydningen af kontaktpunktet ![[Arbejde 2022-10-30 17.00.05.excalidraw]]
<!--SR:!2022-11-04,4,270-->
## Matematisk beskrivelse af arbejde (6.2)

Man kan beskrive $\Delta K$ som en kraft gennem dette udtryk... :: $\Delta K=ma_{CM,x}(v_{x,i}+ \frac{1}{2}a_{CM,x}(\Delta t)^{2})=ma_{CM,x}\Delta x_{F}=F_{x}\Delta x_{F}$.
<!--SR:!2022-11-04,4,277-->
Når ens system består af en punkt-partikel bliver... :: $W=\Delta E=\Delta K$ og derfor også $W=F_{x}\Delta x_{F}$ [^2]
<!--SR:!2022-11-04,4,270-->

[[Impuls]] bestemmes af kraften gennem... 
Energi bestemmes af kraften gennem... 
?
Tiden, da $p= \frac{F}{\Delta t}$ 
Forskydningen af længden da $\Delta E=F_{x}\Delta x_{F}$
<!--SR:!2022-11-04,4,277-->

Den generelle definition af kraftens arbejde er... :: $W=\int_{\vec{r_{i}}}^{\vec{r_{f}}} \vec{F_{ydre}}(\vec{r})\cdot d \vec{r}$ hvor $\vec{r}$ er positionen.[^3]
<!--SR:!2022-11-04,4,277-->

Den generelle definition af arbejdet skrives som dette i en dimension med en variabel, ikke dissipativ kraft...
Hvis kun en kraft virker på en enkelt partikel i en dimension så bliver arbejdet...
Og hvis der er flere kræfter som virker på samme partikel i en dimension så...
?
$W=\int_{\vec{x_{i}}}^{\vec{x_{f}}} \vec{F_{ydre}}(\vec{x})\cdot d \vec{x}$
$W=\vec{F_{x}}\cdot \Delta \vec{x_{F}}$
$W=\sum \vec{F_{x}}\cdot \Delta \vec{x_{F}}$ Denne ligning kaldes også *Arbejdssætningen* for en partikel.
<!--SR:!2022-11-04,4,277-->

## Valg af system (6.3)
**Her menes der systemer som i systemer af elementer ikke koordinater**

Valg af system er vigtigt da... :: Man kan få vidt forskellige arbejde ud fra det system man vælger[^4]
<!--SR:!2022-11-04,4,277-->
Disse slags energier er vigtige at huske... :: Varmeenergi, indre energi. Disse to sker hvis man har friktion og et element som ikke er en punkt-partikel.
<!--SR:!2022-11-01,1,237-->
Det er vigtigt at inkludere underlaget af et system når der er friktion, da... :: Friktion skaber varmeenergi på begge overflader som gnides mod hinanden. Men vi ved ikke hvordan denne er fordelt.
<!--SR:!2022-11-04,4,277-->
En kraft udfører arbejde når... :: den ikke er med i systemet.
<!--SR:!2022-11-04,4,277-->
Kræfter er kræfter på systemet hvis de er ydre, men hvis de er indre så behandles de som... :: Energiformer, både fjederkraften og tyngdekraften bliver til potentiel energi.
<!--SR:!2022-11-04,4,277-->

## Arbejdet udført af tyngdekraften (6.4)

Tyngdekraftens arbejde er positiv når... :: Systemet falder. Og hvis systemet stiger fra jordens overflade ville det være negativt. Dette er sandt da retningen af forskydningen er den modsatte retning af kraften.
<!--SR:!2022-11-04,4,277-->
Vi kan udlede potentielgravitationsenergi gennem arbejdet ved at se på et faldende system således... :: $W_{E}=\int_{\vec{y_{i}}}^{\vec{y_{f}}} \vec{F_{E}}\cdot d \vec{r}=[F_{E}r]^{y_{f}}_{y_{i}}=F_{E}(y_{f}-y_{i})=F_{E}\Delta y=mg \Delta y$ hvor y-aksen peger parallelt med tyngdekraften.[^5]
<!--SR:!2022-11-03,3,257-->



## Konservativ Kraft (6.5)

(Sandt eller falskt) Når vi kigger på arbejdet af en kraft skal vi se på hele distance rejst... :: Dette er falskt. Vi skal blot se på den samlede forskydning af vektorerne.[^6]
<!--SR:!2022-11-04,4,277-->

Disse kræfter er konservative...
Disse kræfter er ikke konservative...
?
Tyngdekraften, Fjederkraften
Friktionskraften
<!--SR:!2022-11-04,4,277-->

## Arbejde Udført på et fler-partikel-system (6.6)

Vi har et fler-partikel-system når... :: Et legeme er deformerbart, eller vi har flere partikler i systemet.
Arbejdet i et fler-partikel-system bliver beskrevet således... :: $$W_{tot}=W_{1}+W_{2}+...+W_{n}=\sum_{i=1}^{N}W_{i}$$ så længe at den enkelte kraft $F_{i}$ skaber en forskydning.

En ydre kraft vil altid påvirke... :: Massemidtpunktet med en forskydelse ogen acceleration

Ændringen af et systems massemidtpunkts hastighed er...
Forskydningen af et systems massemidtpunkt er...



# Plenum
## Eksempel af bold skubbet af fjeder
![[Arbejde 2022-10-31 10.56.56.excalidraw]]
Hvis F=240 N, m=50g, Vf=30m/s
Hvad er så $\Delta x_{F}$?
$W=\Delta K=F \Delta x_{f}-0$ bliver så til$\frac{1}{2}0.05*30^{2}=22,5 J=F \Delta x_{f}\Rightarrow \Delta x_{f}=\frac{22.5}{240}=0.09 m$

# Fodnoter
[^1]: Det vigtigste i denne sætning er helt klart $\triangle x_{F}$. Dette er beskrevet som hvor stor forskydningen er af det punkt hvor kraften virker på systemet, også kaldet kontaktpunktet.
[^2]: Da en punkt-partikel ikke kan deformeres, og derfor ikke har indre energi.
[^3]: Vi benytter vektorer her da de gælder i lige så mange koordinats retninger som man har lyst til at bruge. **Produktet her er et prikprodukt for $\vec{F}\cdot \vec{r}=|\vec{F}||\vec{r}|\cos{\theta }$ hvor $\theta$ er vinklen mellem de to vektorer.**
[^4]: Ergo at man kan vælge et system af den samme situation som giver en lukket eller åben reaktion i systemet.
[^5]: Bemærk at dette dog er den kinetiske energi som er givet ved den tilbagelagte distance.
[^6]: Givet at vi har en konservativ kraft. Hvilket er en kraft som ikke ændrer sig.