# Spørgsmål
Hvorfor kan vi egentligt reducere til (7.2)?
Kig på nogle videoer om hvordan (7.1) udledes.
Hvad mener i egentligt med "Analogt"?
burde der ikke være to prikker over theta under (7.6)?

# Metode til rotationsopgaver
1. Tegn opstilling
2. Løg koordinatsystem, positive akser, reference punkt og omdrejningsakse.
3. Opstil kraftdiagram og kraftligninger
4. Opstil Udvidet kraftdiagram og kraftmomentsligninger
5. Opskriv antallet af ubekendte og antallet af ligninger og geometriske bånd.
6. Løs bevægelsesligningen.
# Kapitel 7, rotationsmekanik.
## Definitioner (7.1)
At dreje beskrives som... :: Bevægelse af et legeme omkring en ydre akse med en given afstand
<!--SR:!2023-02-04,68,310-->
At rotere beskrives som... :: Bevægelse af et legeme omkring sig selv, altså en bevægelse omkring akserne i massemidtpunktet.
<!--SR:!2023-02-06,70,315-->
Vi bruger ofte polære koordinater til drejende legemer med disse størrelser... :: $\theta$ som vinklen mellem akserne og længden fra origo r og retningen af stedvektoren $\vec{r}$.
<!--SR:!2023-02-08,72,315-->
Hvis vi har et legeme med jævn cirkelbevægelse kan vi bruge et bevægende koordinatsystem til at... :: beskrive legemet i origo, som legemet drejer sig om som et roterende legeme.
<!--SR:!2023-02-03,67,312-->
Ved jævn cirkelbevægelse har det drejende legeme... :: konstant fart og en hastighedsvektor parallel med den tangentiale akse.[^1]
<!--SR:!2023-02-08,72,315-->


## Cirkelbevægelse (7.2)
For at vedligeholde en jævn cirkelbevægelse skal vi have... :: en kraft som påvirker legemet.[^2] 
<!--SR:!2023-02-07,71,315-->
Accelerationen på et legeme i cirkelbevægelse bliver påvirket af... :: centripetalaccelerationen[^3] som peger mod centrum af cirklen.
<!--SR:!2023-02-05,69,310-->
Centripetal-accelerationen $\vec{a}_{c}$ er givet ved... :: $\vec{a_{c}}=- \frac{\vec{v_{t}}^{2}}{r}\hat{r}$ [^4]
<!--SR:!2023-01-25,58,270-->
Fordi centripetal-accelerationen er parallel med $\hat r=\vec{r}$ så kan vi skrive værdien af $\vec{a_{c}}$ som... :: $a_{c}=|\vec{a_{c}}|= \frac{\vec{v_{t}}^{2}}{r}$.[^5]
<!--SR:!2022-12-25,34,250-->
Ikke jævne cirkelbaner har også en anden acceleration som hedder... :: tangentiel-accelerationen $a_t$.
<!--SR:!2023-02-09,73,312-->
Ujævne cirkelbevægelser er defineret som... :: cirkelbevægelser som ikke har konstant hastighed.
<!--SR:!2023-02-06,70,315-->
Tangentiel-accelerationen $a_{t}$ er givet ved... :: $a_{t}= \frac{d \vec{v_{t}}}{dt}$[^6]
<!--SR:!2022-12-28,23,270-->
Centrifugalkraften bliver defineret som en fiktiv kraft, som er... :: en kraft man føler da man er i et accelereret koordinatsystem.
<!--SR:!2023-02-04,68,315-->


## Rotations[[kinematik]] (7.3)
For at gøre det lettere for os selv kan vi oversætte bevægelsen i et polært koordinatsystem som... :: $s=\theta r$[^7] hvor s er buestykkets længde.
<!--SR:!2023-02-07,71,310-->
Den tidsafledte af $s=\theta r$ skrives som... :: $\dot s=r \dot \theta$ hvor vi kan skrive $\dot \theta =\omega$ altså vinkelhastigheden og $\dot s=v_{t}$ altså den tangentielle fart.[^8]
<!--SR:!2023-01-28,61,292-->
Vi kan finde $a_{t}$ ved at differentiere den tangentielle fart... :: $a_{t}=r \alpha$[^9]
<!--SR:!2023-02-01,65,295-->

Disse er omregningerne fra de kartetiske koordinater til polære
$x \to$
$v=\frac{dx}{dt}=\dot x \to$
$a=\frac{dv}{dt}=\dot v \to$
?
$\theta$
$\omega =  \frac{d\theta}{dt}=\dot \theta$
$\alpha = \frac{d\omega}{dt}=\dot \omega$[^10]
<!--SR:!2023-02-02,66,310-->

Så længe man har konstant acceleration og husker at skifte koordinatsystem så kan vi... :: bruge vores kinematik på præcis den samme metode som normalt.
<!--SR:!2023-02-10,74,315-->


## [[Inerti]] og Inertimoment/Rotationsinerti (7.4)
![[Rotationsinerti.png]]

En punktpartikel som bevæger sig i en cirkel vil altid have den samme buelængde per tidsstep til forskellige snorlængder da... :: vi kan skrive $s_{1}=s_{2}\Rightarrow r_{1}\theta_{1}=r_{2}\theta_{2}\Rightarrow \frac{r_{1}}{r_{2}}=\frac{\theta_{1}}{\theta_{2}}$ (7.14-7.15-7.16)[^11] 
<!--SR:!2023-02-05,69,315-->
Vinkelhastigheden bliver ændret af snorlængden således... :: vinkelhast skrives $\omega = \frac{v_{t}}{r}$ Så hvis vi har en mindre længde, bliver vinkelhastigheden større.
<!--SR:!2023-02-09,73,315-->
Vinkelhastigheden bliver ændret af vinkel og tid således... :: $\omega = \frac{\Delta \theta}{\Delta t}$.
<!--SR:!2023-02-12,73,330-->
Vi kan omskrive den kinetiske energi til et udtryk af vinkelhastigheden... :: $K= \frac{1}{2}mv^{2}= \frac{1}{2}m (r \omega )^{2}$ Som vi også kan skrive som $\frac{1}{2}(mr^{2})\omega ^{2}$ (7.17)[^12]
<!--SR:!2023-01-27,60,270-->
Den rotationskinetiske energi skrives som... :: $K_{ro}=\frac{1}{2}I_{Q}\omega ^{2}$ (7.18)
<!--SR:!2023-02-03,67,310-->
Ligningen af rotationsinertien for en punkt-partikel er... :: $I=mr^{2}$ (7.19)
<!--SR:!2023-02-07,71,315-->
Rotationskinetiske energi som en generel formel... :: bliver skrevet som $$K=\left(\sum_{i}^{N}(\delta m_{i}r_{i}^{2})\right)\omega ^{2}=\frac{1}{2}I_{Q}\omega ^{2}$$ (7.20+7.21)[^13]
<!--SR:!2023-01-24,57,275-->
Inertimomentet $I_{Q}$ i (7.20) kan også integreres til... :: $I_{Q}=\int_{}^{} r^{2}dm$ (7.23)[^14]
<!--SR:!2023-01-31,64,295-->

For jævn massefordeling i legemer kan vi skrive deres inertimoment som dette
Den generelle løsning: $I_{Q}=\int_{}^{} r^{2}dm$
I en dimension...
I to dimensioner...
I tre dimensioner...
?
$I_{Q}=\lambda \int_{}^{} x^{2}dx$ hvor $\lambda = \frac{dm}{dx}$ hvilket beskriver massefordelingen per længdeenhed dx. $\lambda$ er konstant. (7.24)
$I_{Q}=\sigma \int_{}^{} r^{2}dA$ hvor $\sigma= \frac{dm}{dA}$, sigma er massefordelingen over et areal. A er arealet. (7.25)
$I_{Q}=\rho \int_{}^{} r^{2}dV$ hvor $\rho = \frac{dm}{dV}$, rho er massefordelingen over en volumen, V er volumen. (7.26)
<!--SR:!2022-12-31,40,310-->

Parallelakseteoremet beskriver sammenhængen mellem aksen for massemidtpunktet $I_{CM}$ og en vilkårlig parallel akse $I_{Q}$ således... :: $I_{Q}=I_{CM}+md^{2}$ (7.43)[^15]
<!--SR:!2023-01-26,59,275-->
Vinkelretakseteoremet viser sammenhængen mellem alle inertimomenterne over akserne i et tredimensionelt rum... :: $I_{z}=I_{x}+I_{y}$ (7.44) givet at vi har et legeme som er tæt på at være plan. dvs: $dz<<dx,dy$ 
<!--SR:!2023-02-10,74,315-->

## Rotationskinetisk [[energi]] (7.5)
Hvis vi har $\omega, I_{Q} \text{ og } Q$ som er vinkelhastigheden, inertimomentet og omdrejningsaksen, bliver den [[#Inerti og Inertimoment/Rotationsinerti (7.4)|rotationskinetiske]] energi så... :: $K_{rot}=\frac{1}{2}I_{Q}\omega ^{2}$ (7.45)
<!--SR:!2023-02-05,69,312-->
Hvis vi gerne vil have hele den kinetiske energi af et legeme tager vi altså både vores translationsenergi og rotationsenergi i formlen... :: $K_{tot}=K_{CM}+K_{rot}= \frac{1}{2}mv^{2}+ \frac{1}{2}I_{Q}\omega^{2}$. (7.46)
<!--SR:!2023-02-04,68,310-->

## Impulsmoment (7.6)
Impulsmomentet er det samme som impuls for rotationer og skrives som... :: $L_{Q}=I_{Q}\omega$  Husk at skrive L og $\omega$ som vektorer hvis de ikke er størrelser.(7.49)[^16]
<!--SR:!2022-12-20,18,333-->
Impulsmomentet fra translatorisk bevægelse bliver skrevet som... :: $\vec{L_{Q}}=\vec{r_{Q}}\times \vec{p}$ som også kan skrives $\vec{L_{Q}}=\vec{r}\vec{p}\sin{\theta }$  (7.51)[^17]
<!--SR:!2023-03-07,78,353-->
Denne regel bruges til at finde retningen af impulsmomentet af en cirkelbevægelse... :: højrehåndsreglen. Man peger sine fingre i retningen af stedvektoren, og derefter folder man dem mod impulsvektoren, så vil tommelfingeren pege i samme retning som impulsmomentet.
<!--SR:!2023-03-06,77,353-->
Hvis en partikel er i cirkelbevægelse om en akse vil impulsmomentet fra en ydre akse beskrives som... :: $L_{Q}=L(t)$ at være afhængig af tiden. Den kan pege op eller ned[^18]
<!--SR:!2022-12-26,7,293-->
Den totale impulsmoment for en partikel som roterer og drejer skrives som.. :: $\vec{L_{tot}}=\vec{L_{bane}}+\vec{L_{spin}}$  
<!--SR:!2023-03-03,74,333-->

## Kraftmoment (7.7)
Den tidsligt afledte af impulsmomentet skrives som $\frac{d \vec{L}}{dt}=$... :: $d\frac{\vec{r}\times \vec{p}}{dt}= \frac{d \vec{r}}{dt}\times \vec{p}+\vec{r}\times \frac{d \vec{p}}{dt}$ (7.54)
<!--SR:!2023-01-26,45,313-->
Kraftmomentet, eller torque, er det samme som $\frac{d \vec{L}}{dt}=\frac{d \vec{r}}{dt}\times \vec{p}+\vec{r}\times \frac{d \vec{p}}{dt}$, hvor $\vec{F}= \frac{d \vec{p}}{dt}$ og $\vec{v}\times \vec{p}$ er vinkelrette på hinanden da $\vec{p}=m \vec{v}$, så bliver kraftmomentet... :: $\tau =\frac{d \vec{L}}{dt}= \vec{r}\times \vec{F}$ (7.58)[^19]
<!--SR:!2023-03-09,80,349-->


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
[^13]: Den sidste del kan vi skrive da vi ser på vinkelhastigheden i stedet for hastigheden og radius af alle de forskellige punkter.  
[^14]: Dette er den generelle løsning, men vi kan forbedre den hvis vi har et legeme som har en vis symmetri.
[^15]: Hvor d er distance mellem de to akser og m er inertien.
[^16]: L og I er både afhængige af aksen Q. Hvor $L_{Q}$ er impulsmomentet.
[^17]: hvor p er impulsvektoren og $r_{Q}$ er stedvektoren. Omskrevet er $\theta$ vinklen mellem r og p vektorerne.
[^18]: Dette er også hvor elektroners op og ned spin kommer fra.
[^19]: Tau bliver brugt fordi vi også siger torque.