#forelæsning 
Begyndelsesdato: 16:21   30-10-2022   Uge-43
# Kraft og energi (6.1)

Arbejde(Eller energiligningen) beskrives som... :: energiændringen af systemet når det bliver påvirket af en ydre kraft: $W=\triangle E=\triangle K+\triangle U$.
I et lukket system... ::: $W=0$

Arbejdets fortegn beskriver overførslen af energi således...
?
$W>0$ er en overførsel af energi til systemet
$W<0$ er en afgivelse af energi fra systemet
$W=0$ er energikonstanthed i systemet

Arbejdet er afhængig af denne størrelse... :: $(\triangle x_{F})$. Hvor $\triangle x_{F}$ er forskydningen af systemets massemidtpunkt.[^1]

Kraftens arbejde er positivt når... :: kraften peger samme vej som forskydningen af kontaktpunktet ![[Arbejde 2022-10-30 17.03.20.excalidraw]]
Kraftens arbejde er negativt når... :: kraften peger modsatte vej af forskydningen af kontaktpunktet ![[Arbejde 2022-10-30 17.00.05.excalidraw]]
# Matematisk beskrivelse af arbejde (6.2)

Man kan beskrive $\Delta K$ som en kraft gennem dette udtryk... :: $\Delta K=ma_{CM,x}(v_{x,i}+ \frac{1}{2}a_{CM,x}(\Delta t)^{2})=ma_{CM,x}\Delta x_{F}=F_{x}\Delta x_{F}$.
Når ens system består af en punkt-partikel bliver... :: $W=\Delta E=\Delta K$ og derfor også $W=F_{x}\Delta x_{F}$ [^2]

Impuls bestemmes af kraften gennem... 
Energi bestemmes af kraften gennem... 
?
Tiden, da $p= \frac{F}{\Delta t}$ 
Forskydningen af længden da $\Delta E=F_{x}\Delta x_{F}$

Den generelle definition af kraftens arbejde er... :: $W=\int_{\vec{r_{i}}}^{\vec{r_{f}}} \vec{F_{ydre}}(\vec{r})\cdot d \vec{r}$ hvor $\vec{r}$ er positionen.[^3]

Den generelle definition af arbejdet skrives som dette i en dimension med en variabel, ikke dissipativ kraft...
Hvis kun en kraft virker på en enkelt partikel i en dimension så bliver arbejdet...
Og hvis der er flere kræfter som virker på samme partikel i en dimension så...
?
$W=\int_{\vec{x_{i}}}^{\vec{x_{f}}} \vec{F_{ydre}}(\vec{x})\cdot d \vec{x}$
$W=\vec{F_{x}}\cdot \Delta \vec{x_{F}}$
$W=\sum \vec{F_{x}}\cdot \Delta \vec{x_{F}}$ Denne ligning kaldes også *Arbejdssætningen* for en partikel.

# Valg af system (6.3)
**Her menes der systemer som i systemer af elementer ikke koordinater**

Valg af system er vigtigt da... :: Man kan få vidt forskellige arbejde ud fra det system man vælger[^4]
Disse slags energier er vigtige at huske... :: Varmeenergi, indre energi. Disse to sker hvis man har friktion og et element som ikke er en punkt-partikel.
Det er vigtigt at inkludere underlaget af et system når der er friktion, da... :: Friktion skaber varmeenergi på begge overflader som gnides mod hinanden. Men vi ved ikke hvordan denne er fordelt.
En kraft udfører arbejde når... :: den ikke er med i systemet.
Kræfter er kræfter på systemet hvis de er ydre, men hvis de er indre så behandles de som... :: Energiformer, både fjederkraften og tyngdekraften bliver til potentiel energi.

# Arbejdet udført af tyngdekraften (6.4)


[^1]: Det vigtigste i denne sætning er helt klart $\triangle x_{F}$. Dette er beskrevet som hvor stor forskydningen er af det punkt hvor kraften virker på systemet, også kaldet kontaktpunktet.
[^2]: Da en punkt-partikel ikke kan deformeres, og derfor ikke har indre energi.
[^3]: Vi benytter vektorer her da de gælder i lige så mange koordinats retninger som man har lyst til at bruge. **Produktet her er et prikprodukt for $\vec{F}\cdot \vec{r}=|\vec{F}||\vec{r}|\cos{\theta }$ hvor $\theta$ er vinklen mellem de to vektorer.**
[^4]: Ergo at man kan vælge et system af den samme situation som giver en lukket eller åben reaktion i systemet.