## a Tegn


## b
En stangs inertimoment er $I_{cm}=\frac{1}{12}m l^{2}$. Men da vores stang roterer omkring punktet P som er distancen d væk fra CM så bruger vi parallelakseteoremet. 
Vi finder $I_{P} = \frac{1}{12}ml^{2}+md^{2} \Rightarrow \frac{1}{12}Mb^{2}+Md^{2}$ 
Nu kan vi indsætte vores værdier og finde værdien af $I_{P}$. Lad os gøre det: $$I_{P}=\frac{1}{12} \cdot 0.2 kg \cdot 0.5m^{2} + 0.2kg \cdot 0.2m^{2} = \frac{73}{6000} kg\space m^{2} \approx 0.012 kg\space m^{2}$$
## c
Vi kan benytte at vi har et lukket system til at finde den kinetiske energi af metalkuglen, og derved skrive $E = \frac{1}{2}m v^{2}= \frac{1}{2}I_{P}\omega^{2}$. Her antager vi at kuglen opfører sig som en punktpartikel, altså kun kinetisk energi.

Så kan vi opskrive vinkelhast efter stødet således: $$\omega = \sqrt{\frac{2E}{I_{P}}} \approx 6.41 \frac{1}{s}$$
## d Tegn

## e
$$\sum \vec{\tau } = \vec{\tau_{Mg}} + \vec{\tau_{Mn}}+\vec{\tau_{m_{k}g}}$$
$$\sum \tau = -dF_{Mg}-d_{k}F_{m_{k}g}= I_{P} \ddot \theta $$

## f
Vi kan udvide kraftmomentsligningen som vi fandt i (e) til at finde $$\ddot \theta = -g\theta \frac{dM+d_{k}m_{k}}{I_{P}}$$Ved små vinkler er $\sin{\theta }=\theta$.

Nu kan vi bruge denne til at finde $$\ddot \theta + \omega ^{2} \theta = 0$$ hvor $\omega= \sqrt{g  \left(\frac{dM+d_{k}m_{k}}{I_{P}}\right)}\approx 5.86 \frac{1}{s}$.
Dette giver os bevægelses ligningen $$\theta(t)=A \cos{\left(\omega t+ \phi \right)}$$Ved $\theta (t)=0$ er dette kun muligt hvis $\cos{(\omega t + \phi )}=0$ Så derfor må $\phi = \frac{\pi}{2}$.
Vi kan differentiere dette, da vi kender vinkelhastigheden ved tiden t = 0s efter stødet. 

$$\dot \theta(t) = -A \omega \sin{(\omega t + \phi )}$$
$$\dot \theta (0)=-A \omega \sin{(\phi )}=12.82 \frac{1}{s} \Rightarrow A = - \frac{\dot\theta}{\omega} $$
Endelig kan vi indsætte vores værdier og finde amplituden, som er det samme som max vinklen $A = \theta_{max}$.
$$A = \frac{\dot \theta}{\sqrt{g\frac{dM+d_{k}m_{k}}{I_{P}}}}\approx 1.09^{\circ}$$
Her kan vi se at max vinklen er lille. Ved $A = 1.09^{\circ}$ er usikkerheden så lille ved approksimationer om fx $\sin{\theta }= \theta$ for at vi kan se bort fra forskellen. 

## g
Svigningstiden T er givet ved $$T = 2 \pi \frac{1}{\omega} =1.07 s$$
## h
Efter et sekunds rejsetid vil stangen have svunget $\frac{1s}{T}$ gange frem og tilbage. Derfor vil antallet af grader være. $$\frac{1s}{T} \cdot A \cdot 2 = 2.04^{\circ}$$
## i
tangentielfarten er givet ved $v_{t}=\omega r = \omega d_{k} =2.05 \frac{m}{s}$  