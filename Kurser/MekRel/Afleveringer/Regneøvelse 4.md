# Opgave 1
Ring = $\frac{1}{2}m_{h}R_{h}^{2}$
cylinder $=\frac{1}{2}m_{c}R_{c}+m_{c}R_{h}^{2}$
Pind $=\frac{1}{12}m_{p}L+m_{p}(R_{k}+R_{h})^{2}$
Kugle $=\frac{2}{5}m_{k}R_{k}^{2}+m_{k}(R_{k}+R_{h}+L)^{2}$
Systemets inertimoment $I_{syst}=\frac{1}{2}m_{h}R_{h}^{2}+\frac{1}{2}m_{c}R_{c}+m_{c}R_{h}^{2}+\frac{1}{12}m_{p}L+m_{p}(R_{k}+R_{h})^{2}+\frac{2}{5}m_{k}R_{k}^{2}+m_{k}(R_{k}+R_{h}+L)^{2}$


# Opgave 2
## a
![[Regneøvelse 4 2022-11-29 14.43.03.excalidraw]]
## b
![[Regneøvelse 4 2022-11-29 14.55.11.excalidraw]]
## c
$\sum \tau =\vec{r_{sv}}\times \vec{F_{sv}}+\vec{0}\times \vec{F_{nv}}+\vec{r_{Lv}}\times \vec{F_{Lv}}+\vec{r_{Ev}}\times \vec{F_{Ev}}=0$  
$\sum \tau =\tau_{sv}-\tau_{Lv}-\tau_{Ev}=0$
## d
$\sum \tau =\vec{r_{sv}}\vec{F_{sv}}\sin{\theta_{1}}-\vec{r_{Lv}}\vec{F_{Lv}}\sin{\theta_{2}}-\vec{r_{Ev}}\vec{F_{Ev}}\sin{\theta_{3}}=0$ 
I dette tilfælde er $|\theta_{1}|=|\theta_{2}|=|\theta_{3}|=\theta=\frac{\pi}{2}$. og $d=\vec{r_{Lv}}$
$0=\vec{r_{sv}}\vec{F_{sv}}-\vec{r_{Lv}}\vec{F_{Lv}}-\vec{r_{Ev}}\vec{F_{Ev}}$ 
$\vec{d}=\frac{\vec{r_{sv}}\vec{F_{sv}}-\vec{r_{Ev}}\vec{F_{Ev}}}{\vec{F_{Lv}}}$ Enhederne passer også her.
## e
Hvis vi antager at massefordelingen i planken er regulær så er tyngdepunktet $\frac{L}{6}$ væk fra punktet P.
$\vec{d}=\frac{\vec{\frac{L}{4}}\vec{F_{sv}}-\vec{\frac{L}{6}}\vec{F_{Ev}}}{\vec{F_{Lv}}}$ .
Alt acceleration er tyngdeaccelerationen g.
$\vec{F_{sv}}=2\text{ kg }\cdot \vec{g}$
$\vec{F_{Ev}}=2\text{ kg }\cdot \vec{g}$
$\vec{F_{Lv}}=0,5\text{ kg }\cdot \vec{g}$ 
Så bliver d til 
$$\vec{d}=\frac{\vec{\frac{L}{4}}2kg-\vec{\frac{L}{6}}2kg}{0,5kg}=4\left(\vec{\frac{L}{4}}-\vec{\frac{L}{6}}\right)=\vec{L}\left(1- \frac{2}{3}\right)=\frac{\vec{L}}{3}$$
## f
Vippens højre ende vil falde mod jorden.
![[Regneøvelse 4 2022-11-29 15.57.35.excalidraw]]
## g
$\sum \tau =\vec{r_{sv}}\times \vec{F_{sv}}+\vec{0}\times \vec{F_{nv}}+\vec{r_{Lv}}\times \vec{F_{Lv}}+\vec{r_{Ev}}\times \vec{F_{Ev}}+\vec{r_{fv}}\times \vec{F_{fv}}=\alpha I$$\sum \tau =\tau_{sv}-\tau_{Lv}-\tau_{Ev}-\tau_{fv}=\alpha I$ 
$\sum \tau =\vec{r_{sv}}\vec{F_{sv}}\sin{\theta_{1}}-\vec{r_{Lv}}\vec{F_{Lv}}\sin{\theta_{2}}-\vec{r_{Ev}}\vec{F_{Ev}}\sin{\theta_{3}}-\vec{r_{fv}}\vec{F_{fv}}=\alpha I$

## h
(i) $$I_{v}=\frac{1}{12}m_{v}L^2 +m_v\left(\frac{1}{6}L\right)^2 = \frac{1}{9}m_v L$$  
(ii) $I_{v}=\frac{m_{v}}{L}\int_{\frac{-1}{3}L}^{\frac{2}{3}L}x^{2}\space dx=\frac{1}{9}m_{v}L$
Vi ser på (7.24) som guide.
$I_{sys}=\frac{1}{9}m_{v}L^{2}+ \frac{1}{16}m_{s}L^{2}+ \frac{1}{9}m_{L}L^{2}+ \frac{4}{9}m_{f}L$

## i
Vi antager at der menes at vi skal finde accelerationen i det øjeblik hvor vippen begynder at vælte. Denne acceleration er nemlig ikke konstant, da vinklen mellem kraftvektorerne og stedvektoren ændrer sig i forhold til tiden.
I dette tilfælde vil alle graderne være $\frac{\pi}{2}$ så $\sin{\theta }$ vil blive 1.
$\frac{d \omega }{dt}=\alpha = g\frac{\frac{1}{4}\vec{L}m_{sv}- \frac{1}{6}\vec{L}m_{Ev}- \frac{1}{3}\vec{L}m_{Lv}- \frac{2}{3}\vec{L}m_{fv}}{I_{sys}}\cdot 360^{\circ}$
Vi ved at der er ligvægt før fuglen lander på vippen, så vi kan skrive $$\alpha =g\vec{L} \frac{2m_{fv}}{3I_{sys}}\cdot 360^{\circ}$$
$I_{sys}\approx 6.47 kg m^{2}$
$\alpha= \frac{\frac{2}{3}\vec{L}m_{fv}}{I_{sys}}=-5,94 \frac{\circ}{s^{2}}$   
## j
Vi kan finde vinklen gennem $\tan{\theta }=\mu_{s}$ Så for at finde vinklen isolerer vi theta $\theta =\tan^{-1}{\mu_{s}}=\tan^{-1}{0.35}=19,29^{\circ}$  
## k

## m
