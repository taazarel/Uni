#### mws572, Luci Fenger, Hold 2
# Opgave 1
Først definerer vi inertimomentet for alle formerne defineret i forhold til aksen Q gennem punktet C.

Ring = $\frac{1}{2}m_{h}R_{h}^{2}$
cylinder $=\frac{1}{2}m_{c}R_{c}+m_{c}R_{h}^{2}$
Pind $=\frac{1}{12}m_{p}L+m_{p}(R_{k}+R_{h})^{2}$
Kugle $=\frac{2}{5}m_{k}R_{k}^{2}+m_{k}(R_{k}+R_{h}+L)^{2}$
Og til sidst finder vi summen af alle disse led:$I_{syst}=\frac{1}{2}m_{h}R_{h}^{2}+\frac{1}{2}m_{c}R_{c}+m_{c}R_{h}^{2}$
$+\frac{1}{12}m_{p}L+m_{p}(R_{k}+R_{h})^{2}+\frac{2}{5}m_{k}R_{k}^{2}+m_{k}(R_{k}+R_{h}+L)^{2}$

# Opgave 2
## a
Skitse af opstilling:
![[Regneøvelse 4 2022-11-29 14.43.03.excalidraw]]

## b
Udvidet kraftdiagram for opstilling:
![[Regneøvelse 4 2022-12-04 21.26.05.excalidraw]]
## c
Kraftmomenterne som krydsprodukter:
$$\sum \tau =\vec{r_{sv}}\times \vec{F_{sv}}+\vec{0}\times \vec{F_{nv}}+\vec{r_{Lv}}\times \vec{F_{Lv}}+\vec{r_{Ev}}\times \vec{F_{Ev}}=0$$
$$\sum \tau =\tau_{sv}-\tau_{Lv}-\tau_{Ev}=0$$
Kraftmomenterne som parallelogram mellem stedvektoren og kræfterne:
$$\sum \tau =\vec{r_{sv}}\vec{F_{sv}}\sin{\theta_{1}}-\vec{r_{Lv}}\vec{F_{Lv}}\sin{\theta_{2}}-\vec{r_{Ev}}\vec{F_{Ev}}\sin{\theta_{3}}=0$$ 
## d
I vores opstilling er $|\theta_{1}|=|\theta_{2}|=|\theta_{3}|=\theta=\frac{\pi}{2}$. og $d=\vec{r_{Lv}}$
Vi kan isolere d og finde den i forhold til de andre kraftmomenter:
$0=\vec{r_{sv}}\vec{F_{sv}}-\vec{r_{Lv}}\vec{F_{Lv}}-\vec{r_{Ev}}\vec{F_{Ev}}$ 
$\vec{d}=\frac{\vec{r_{sv}}\vec{F_{sv}}-\vec{r_{Ev}}\vec{F_{Ev}}}{\vec{F_{Lv}}}$ 
Enhederne passer også her.
## e
Hvis vi antager at massefordelingen i planken er regulær så er tyngdepunktet $\frac{L}{6}$ væk fra punktet P, da tyngdepunktet vil være i midten. Stødpuden er $\frac{L}{4}$ væk fra P.
$$\vec{d}=\frac{\vec{\frac{L}{4}}\vec{F_{sv}}-\vec{\frac{L}{6}}\vec{F_{Ev}}}{\vec{F_{Lv}}}$$
Alt acceleration er tyngdeaccelerationen g. Hvilket er defineret som $10 \frac{m}{s^{2}}$.
Kræfterne er:
$\vec{F_{sv}}=2\text{ kg }\cdot \vec{g}$
$\vec{F_{Ev}}=2\text{ kg }\cdot \vec{g}$
$\vec{F_{Lv}}=0,5\text{ kg }\cdot \vec{g}$ 
Nu indsætter vi vores værdier og får:
$$\vec{d}=\frac{\vec{\frac{L}{4}}2kg-\vec{\frac{L}{6}}2kg}{0,5kg}=4\left(\vec{\frac{L}{4}}-\vec{\frac{L}{6}}\right)=\vec{L}\left(1- \frac{2}{3}\right)=\frac{\vec{L}}{3}$$
## f
Ligevægten brydes og vippens højre ende går mod jorden.
![[Regneøvelse 4 2022-11-29 15.57.35.excalidraw]]
## g
Vi kan opstille vores kraftmomenter således.
$\sum \tau =\vec{r_{sv}}\times \vec{F_{sv}}+\vec{0}\times \vec{F_{nv}}+\vec{r_{Lv}}\times \vec{F_{Lv}}+\vec{r_{Ev}}\times \vec{F_{Ev}}+\vec{r_{fv}}\times \vec{F_{fv}}=\alpha I$$\sum \tau =\tau_{sv}-\tau_{Lv}-\tau_{Ev}-\tau_{fv}=\alpha I$ 
$\sum \tau =\vec{r_{sv}}\vec{F_{sv}}\sin{\theta_{1}}-\vec{r_{Lv}}\vec{F_{Lv}}\sin{\theta_{2}}-\vec{r_{Ev}}\vec{F_{Ev}}\sin{\theta_{3}}-\vec{r_{fv}}\vec{F_{fv}}=\alpha I$
Men de kan også skrives således da vi ved at resten af kræfterne bliver nul:
$\sum \tau =\vec{r_{fv}}\times \vec{F_{fv}}=\alpha I$
$\sum \tau =- \vec{r_{fv}}\vec{F_{fv}}=\alpha I$

## h
(i) 
Gennem rotationsaksen gennem P kan vi finde inertimomentet som en stang. Vi får også at vide i opgaven at vi kan definere alle legemerne som punktmasser, derfor får vi:
$$I_{v}=\frac{1}{12}m_{v}L^2 +m_v\left(\frac{1}{6}L\right)^2 = \frac{1}{9}m_v L$$ Gennem parallelakseteoremet.
(ii) 
Vi kan finde massefordelingen per længdeenhed gennem 7.24. Vores integral skal gå fra $\frac{-1}{3}L$ og $\frac{2}{3}L$ da vi går fra punktet P.
Hvilket giver os:
$$I_{v}=\frac{m_{v}}{L}\int_{\frac{-1}{3}L}^{\frac{2}{3}L}x^{2}\space dx=\frac{1}{9}m_{v}L$$
Vi kan konkludere at dette må være korrekt da begge er i overensstemmelse.
Vi kan skrive inertimomentet af hele systemet som:
$I_{sys}=\frac{1}{9}m_{v}L^{2}+ \frac{1}{16}m_{s}L^{2}+ \frac{1}{9}m_{L}L^{2}+ \frac{4}{9}m_{f}L$

## i
Vi antager at der menes at vi skal finde accelerationen i det øjeblik hvor vippen begynder at vælte. Denne acceleration er nemlig ikke konstant, da vinklen mellem kraftvektorerne og stedvektoren ændrer sig i forhold til tiden.
I dette tilfælde vil alle graderne være $\frac{\pi}{2}$ så $\sin{\theta }$ vil blive 1.
$\frac{d \omega }{dt}=\alpha = g\frac{\frac{1}{4}\vec{L}m_{sv}- \frac{1}{6}\vec{L}m_{Ev}- \frac{1}{3}\vec{L}m_{Lv}- \frac{2}{3}\vec{L}m_{fv}}{I_{sys}}\cdot 360^{\circ}$
Vi ved at der er ligevægt før fuglen lander på vippen, så vi kan skrive $$\alpha =g\vec{L} \frac{-2m_{fv}}{3I_{sys}}\cdot 360^{\circ}$$
Vi ganger her med 360 grader da vinkelaccelerationen giver os en andel af cirklen.
Med de givne værdier så er: $I_{sys}\approx 6.47 kg m^{2}$
$$\alpha= gL\frac{-2m_{fv}}{3I_{sys}}\cdot 360^\circ\approx-5,94 \frac{\circ}{s^{2}}$$
Vi får en negativ værdi, men dette giver mening da rotationen er imod rotationsaksens positive retning.
## j
Vi kan finde vinklen gennem $\tan{\phi  }=\mu_{s}$ Så for at finde vinklen isolerer vi phi:
$$\phi  =\tan^{-1}{\mu_{s}}=\tan^{-1}{0.35}=19,29^{\circ}$$Hvor phi er vinklen for vippen mod vandret.

## k
Da vi har konstant acceleration kan vi bruge bevægelsesligningen:
$$\phi  = \frac{1}{2}\alpha t^{2}+ \omega t+ \phi_{0}$$
I vores tilfælde har vi hverken en starthast og da vores startvinkel er $\phi_{0}=0^{\circ}$ så bliver udtrykket $$\phi=\frac{1}{2}\alpha t^{2}$$
Vi kan isolere tiden $$t=\pm\sqrt{\frac{2\phi}{\alpha}}$$
Nu kan vi indsætte vores tidligere værdier og finde tiden. Vi ser kun på den positive værdi
$$t\approx 2,55 s$$

## m
I dette tilfælde ville vippen dreje hurtigere. Inertimomentet forbliver det samme mens inertien formindskes. Hvilket betyder at længden af vippen skal blive længere for at kompensere. Vi kan se fra vores accelerationsligning at vippen derfor vil dreje hurtigere da den er afhængig af længden i tælleren af brøken.