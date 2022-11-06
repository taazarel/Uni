# Spørgsmål
Hvorfor kan vi egentligt reducere til (7.2)?
Kig på nogle videoer om hvordan (7.1) udledes.
Hvad mener i egentligt med "Analogt"?
burde der ikke være to prikker over theta under (7.6)?

# Kapitel 7, rotationsmekanik.
## Definitioner (7.1)
At dreje beskrives som... :: Bevægelse af et legeme omkring en ydre akse med en given afstand
At rotere beskrives som... :: Bevægelse af et legeme omkring sig selv, altså en bevægelse omkring akserne i massemidtpunktet.
Vi bruger ofte polære koordinater til drejende legemer med disse størrelser... :: $\theta$ som vinklen mellem akserne og længden fra origo r og retningen af stedvektoren $\vec{r}$.
Hvis vi har et legeme med jævn cirkelbevægelse kan vi bruge et bevægende koordinatsystem til at... :: beskrive legemet i origo, som legemet drejer sig om som et roterende legeme.
Ved jævn cirkelbevægelse har det drejende legeme... :: konstant fart og en hastighedsvektor parallel med den tangentiale akse.[^1]


## Cirkelbevægelse (7.2)
For at vedligeholde en jævn cirkelbevægelse skal vi have... :: en kraft som påvirker legemet.[^2] 
Accelerationen på et legeme i cirkelbevægelse bliver påvirket af... :: centripetalaccelerationen[^3] som peger mod centrum af cirklen.
Centripetal-accelerationen $\vec{a}_{c}$ er givet ved... :: $\vec{a_{c}}=- \frac{\vec{v_{t}}^{2}}{r}\hat{r}$ [^4]
Fordi centripetal-accelerationen er parallel med $\hat r=\vec{r}$ så kan vi skrive værdien af $\vec{a_{c}}$ som... :: $a_{c}=|\vec{a_{c}}|= \frac{\vec{v_{t}}^{2}}{r}$.[^5]
Ikke jævne cirkelbaner har også en anden acceleration som hedder... :: tangentiel-accelerationen $a_t$.
Ujævne cirkelbevægelser er defineret som... :: cirkelbevægelser som ikke har konstant hastighed.
Tangentiel-accelerationen $a_{t}$ er givet ved... :: $a_{t}= \frac{d \vec{v_{t}}}{dt}$[^6]
Centrifugalkraften bliver defineret som en fiktiv kraft, som er... :: en kraft man føler da man er i et accelereret koordinatsystem.


## Rotations[[kinematik]] (7.3)
For at gøre det lettere for os selv kan vi oversætte bevægelsen i et polært koordinatsystem som... :: $s=\theta r$[^7] hvor s er buestykkets længde.
Den tidsafledte (7.4) skrives som... :: $\dot s=r \dot \theta$ hvor vi kan skrive $\dot \theta =\omega$ altså vinkelhastigheden og $\dot s=v_{t}$ altså den tangentielle fart.[^8]
Vi kan finde $a_{t}$ ved at differentiere den tangentielle fart... :: $a_{t}=r \alpha$[^9]

Disse er omregningerne fra de kartetiske koordinater til polære
$x \to$
$v=\frac{dx}{dt}=\dot x \to$
$a=\frac{dv}{dt}=\dot v \to$
?
$\theta$
$\omega =  \frac{d\theta}{dt}=\dot \theta$
$\alpha = \frac{d\omega}{dt}=\dot \omega$[^10]

Så længe man har konstant acceleration og husker at skifte koordinatsystem så kan vi... :: bruge vores kinematik på præcis den samme metode som normalt.


## [[Inerti]] og Inertimoment/Rotationsinerti (7.4)
![[Rotationsinerti.png]]

En punktpartikel som bevæger sig i en cirkel vil altid have den samme buelængde per tidsstep til forskellige snorlængder da... :: vi kan skrive $s_{1}=s_{2}\Rightarrow r_{1}\theta_{1}=r_{2}\theta_{2}\Rightarrow \frac{r_{1}}{r_{2}}=\frac{\theta_{1}}{\theta_{2}}$ (7.14-7.15-7.16)[^11] 
Vinkelhastigheden bliver ændret af snorlængden således... :: vinkelhast skrives $\omega = \frac{\Delta \theta}{\Delta t}$ Så hvis vi har en mindre længde, bliver vinklen større og så bliver hastigheden større.
Vi kan omskrive den kinetiske energi til et udtryk af vinkelhastigheden... :: $K= \frac{1}{2}mv^{2}= \frac{1}{2}m (r \omega )^{2}$ Som vi også kan skrive som $\frac{1}{2}(mr^{2})\omega ^{2}$ (7.17)[^12]
Den rotationskinetiske energi skrives som... :: $K_{ro}=\frac{1}{2}I_{Q}\omega ^{2}$ (7.18)
Ligningen af rotationsinertien for en punkt-partikel er... :: $I=mr^{2}$


## Rotationskinetisk [[energi]] (7.5)
Hvis vi har $\omega, I_{Q} \text{ og } Q$ som er vinkelhastigheden, inertimomentet og omdrejningsaksen, bliver den [[#Inerti og Inertimoment/Rotationsinerti (7.4)|rotationskinetiske]] energi så... :: $K_{rot}=\frac{1}{2}I_{Q}\omega ^{2}$ (7.45)
Hvis vi gerne vil have hele den kinetiske energi af et legeme tager vi altså både vores translationsenergi og rotationsenergi i formlen... :: $K_{tot}=K_{CM}+K_{rot}= \frac{1}{2}mv^{2}+ \frac{1}{2}I_{Q}\omega^{2}$. (7.46)

## Fodnoter
[^1]: Dette kaldes også tangential-hastigheden $\vec{v_{t}}$
[^2]: Jo mindre r, desto højere kraft.
[^3]: Centripetal betyder center-søgende på latin.
[^4]: Hvor $\hat r$ er enhedsvektoren for stedvektoren. Som starter i origo og peger mod legemet. (7.1)
[^5]: Dette kaldes også (7.2)
[^6]: (7.3)
[^7]: (7.4)
[^8]: Vi kan herved skrive ligningen som $v_{t}=r \omega$ (7.5)
[^9]: (7.6)
[^10]: Disse er defineret som, fra top til bund (7.7),(7.8) og (7.9)
[^11]: hvilket bare betyder at deres buelængde er bevaret, selvom snorlængden og vinklen ikke er. Vi kan også vise dette ved $s=v \Delta t$ Ergo hvis deres hastighed er det samme, og vi kigger på det samme tidsstep er buelængden det samme.
[^12]: Vi kan nemlig skrive $(mr^{2})\omega ^{2}$ som $I_{Q}$ hvilket er brugbart i  (7.18)