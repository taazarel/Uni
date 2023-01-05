#forelæsning 
Begyndelsesdato: 10:54   10-10-2022   Uge-41
# Flashcards


# Euler-lagrange formlen
$L=K-U$ , hvor $L=$ Mindstevirkningen, $K=$ den kinetiske [[energi]], og $U=$ den potentielle energi.
Normalt skrives den totale energi i et system således: $E=K+U$. 
Det gælder at L kan være en funktion som skrives... :: $L(x,v,t)$.
<!--SR:!2023-07-05,203,316-->

Mindstevirkningsprincippet skrives som... :: $\left[L=K-U\right]$.
<!--SR:!2023-01-08,69,314-->

$L=K-U$ kaldes også mindstevirkningsprincippet, og den kan bruges til at beskrive bevægelsen af et objekt.
Objekter bevæger sig over... :: Den korteste længde/mindste virkning/the path of least resistance.
<!--SR:!2022-12-23,4,305-->
<!--SR:!2023-03-02,73,335-->

<!--SR:!2023-02-25,89,270-->
Derfor bliver objekters baner altid den af "least resistance".

Man kan differentiere denne formel for at finde en bedre en.
$L=\frac{1}{2}mv^{2}-mgx$, denne differentieret er $\frac{\delta L}{\delta x}=- \frac{\delta U}{\delta x}=-mg$ og $\frac{\delta L}{\delta v}= \frac{\delta K}{\delta v}=mv$. Vi kan også differentiere dette igen for at finde en acceleration, og derfor have masse gange acceleration i begge tilfælde.
$$\frac{d}{dt}(\frac{\delta L}{\delta v})=ma$$
Nu kan vi indsætte i mindstevirkningsprincippet.
Lagrange formlen skrives som... :: $$\left[\left[\frac{d}{dt} \left(\frac{\delta L}{\delta v}\right)= \frac{\delta L}{\delta x}\right]\right]$$.
<!--SR:!2023-10-28,296,330-->
Denne formel kaldes også for Euler-Lagrange formlen. Enheden for "Lagrangen" er Joule.
fx er: Euler lagrange ligningen for noget i fald i et tyngdefelt er derfor: $ma=-mg$ 

Definitionen af det absolutte nulpunkt er ligegyldigt, da vi blot beskriver det som en konstant, hvilket forsvinder når vi differentierer. Derudover er størrelsesordenen af vores målte energi også ligegyldig, formlen ville stadigvæk virke.

## Eksempler
![[Mindstevirkningsprincippet 2022-10-10 11.35.30.excalidraw]]
$x_{1}=l-x_{2}$
$x_{1}^{'}=-x_{2}^{'} \Rightarrow x_{1}^{'2}=-x_{2}^{'2}$ 

Her kan man enten bruge kraftdiagrammer og kraftligninger, og derved få 2 ligninger med to ubekendte, eller bruge mindstevirkningsprincippet og finde 1 ligningen med 1 ubekendt, da vi ingen snorspænding har.
Dette gør vi over 7 trin:
1. $K=\frac{1}{2}(m_{1}+m_{2})x_{1}^{'2}$
2. $U=-m_{1}gx_{1}-m_{2}g(l-x_{1})$ 
3. $L=\frac{1}{2}(m_{1}+m_{2})x_{1}^{'2}-(-m_{1}gx_{1}-m_{2}g(l-x_{1}))$ 
4. $\frac{\delta L}{\delta x_{1}}=m_{1}g-m_{2}g$
5. $\frac{dL}{dv_{1}}=(m_{1}+m_{2})x_{1}^{'}$ 
6. $\frac{d}{dt}(\frac{dL}{dv_{1}})=(m_{1}+m_{2})x_{1}^{''}$
7. $(m_{1}+m_{2})x_{1}^{''}=(m_{1}-m_{2})g\Rightarrow x^{''}_{1}= \frac{m_{1}-m_{2}}{m_{1}+m_{2}}g$ 
OBS[^1]

# Forberedelse
## Impulsbevarelse
Hvis vi har konstant potential i et system så bliver euler-larange ligningen $L=K-konstant$ hvilket betyder at vores larange funktion bliver:
$\frac{d}{dt}\left(\frac{\delta L}{\delta v}\right) =\frac{d}{dt}(mv)=0$ da vi differentierer en konstant. 
Men $p=mv$ er vores [[Impuls]], så derfor kan vi se at vores impuls er konstant, da accelerationen bliver 0.
Under konstant potientiale bliver lagrange ligningen... :: $\frac{d}{dt}\left(\frac{\delta L}{\delta v}\right) =\frac{d}{dt}(mv)=0$
<!--SR:!2023-04-22,142,296-->

Lagrangen er altså dannet af en del som er afhængig af hastighed(K) og en som er afhængig af rummet(U). OG hvis vores Lagrange er uafhængig af rummet har vi impulsbevarelse og rumlig homogenitet.
Når Lagrange funktionen er uafhængig af rummet har vi... :: Rumlig homogenitet/rumlig forskydningssymmetri og impulsbevarelse.
<!--SR:!2023-04-13,135,296-->

Vi får også at vores impuls er additiv da Lagrangen også er det $p=\frac{\delta L}{\delta v}$.
Impuls er additiv da... :: $p=\frac{\delta L}{\delta v}$.
<!--SR:!2023-07-07,205,316-->

## Energibevarelse
Når Lagrange funktionen er uafhængig af tiden får vi... :: Energibevarelse.
<!--SR:!2023-07-06,204,316-->
Den generelle ligning for den tidsligt afledte L er... :: $\frac{dL}{dt}=\frac{\delta L}{\delta x}v+ \frac{\delta L}{\delta v}a+ \frac{\delta L}{\delta t}$.
<!--SR:!2023-01-28,45,316-->


Og hvis vi har tidslig symmetri så bliver $\frac{\delta L}{\delta t}=0$.
Dette kombineret med EL ligningen på første led ovenover bliver til $$\frac{dL}{dt}=\frac{d}{dt}\left(\frac{\delta L}{\delta v}\right)v+\frac{\delta L}{\delta v}a$$
Hvilket kan omskrives til $$H=v \frac{\delta L}{\delta v}-L,$$
og hermed ser vi at hvis vores EL ligning er uafhængig af tiden bliver $H=K+U$ og vi har derfor energibevarelse.
Lagrange funktionens tidsafledte funktion er... ::: $H=v \frac{\delta L}{\delta v}-L$.
<!--SR:!2023-03-04,93,256!2023-05-11,148,296-->
$H=v \frac{\delta L}{\delta v}-L$ under tidslig symmetri er... ::: $H=K+U$.
<!--SR:!2023-07-08,206,316!2023-05-13,159,298-->

Hvis der er flere variabler som L er afhængig af i rummet bliver Hamilton liningen: $$H=\sum_{i}q'_{i} \frac{\delta L}{\delta q'_{1}}-L$$
Hvilket bare viser at alle variablerne skal summes.
Tidslig symmetri, eller at tiden ikke indgår symmetrisk betyder blot... :: at reaktionen ikke vil blive ændret uanset om vi gør det i morgen eller om 5 måneder.
<!--SR:!2023-05-12,158,296-->
Når vi har tidslig symmetri kan vi også se at energi er additiv.

## Andre bevarede størrelser
I tredimensionelt rum er vektorer bevaret dvs $\vec{J}=\vec{r}x \vec{p}$ og derved kan vi se bevareslse gennem $\frac{d\vec{J}}{dt}=0$, hvilket er impulsmomentets vektor.

Der er 7 bevarede størrelser i alt, de er... :: Impuls i 3 forskellige dimensioner, impulsmomentet J i tre forskellige dimensioner og energi.
<!--SR:!2023-06-12,185,316-->

## [[Funktioner af flere variable#Polære koordinater:|Polære Koordinater]]
Spørgsmål om hvad fanden der sker i (5.35) da jeg ingen ide har !?

Gennem polære koordinater kan vi se at en acceleration bliver til centrifugal kraften.
$L=\frac{1}{2}m(r'^{2}+r^{2}\theta'^{2})$ hvilket bliver til $mr''=mr \theta '^{2}$ 
Hvor at centrifugalaccelerationen er $a=r \theta'^{2}$.

### Eksempler
#### Vippe
![[Mindstevirkningsprincippet 2022-10-28 08.26.45.excalidraw]]
0. Brug polære koordinater
1. $K=\frac{1}{2}m_{1}(l_{1}\theta^{´})^{2}+ \frac{1}{2}m_{2}(l_{2}\theta^{´})^{2}$  
2. $U=-m_{1}g(l_{1}\sin{\theta})+m_{2}g(l_{2}\sin{ \theta})$ 
3. $L=\frac{1}{2}m_{1}(l_{1}\theta^{´})^{2}+ \frac{1}{2}m_{2}(l_{2}\theta^{´})^{2}-(-m_{1}g(l_{1}\sin{\theta})+m_{2}g(l_{2}\sin{ \theta)})$
4. $\frac{dL}{d \theta}=m_{1}gl_{1}\cos{\theta}-m_{2}l_{2}\cos{\theta}\Rightarrow (m_{1}l_{1}-m_{2}l_{2})g\cos{\theta}$  
5. $\frac{dL}{d \theta^{´}}=(m_{1}l_{1}^{2}+m_{2}l_{2}^{2})\theta^{´}$
6. $\frac{d}{dt} \frac{dL}{d \theta^{´}}=(m_{1}l_{1}^{2}+m_{2}l_{2}^{2})\theta^{´´}$
7. $\frac{d}{dt} \frac{dL}{d \theta^{´}}=\frac{dL}{d \theta} \Rightarrow \theta^{´´}= g\cos{\theta}\frac{(m_{1}l_{1}-m_{2}l_{2})}{m_{1}l_{1}^{2}+m_{2}l_{2}^{2}}$ 
Lad os tjekke grænseværdien når barn 1 hopper af vippen:
$$-g \cos{\theta} \frac{1}{l_{2}}$$
Dette ligner meget et matematisk pendul.
Vi kan også se at (7) har ligevægt når: $g=0,\cos{\theta}=0,m_{1}l_{1}-m_{2}l_{2}=0$
Især er den sidste del relevant. Vi kan nemlig se at kraften på begge sider af vippen vil blive: $gm_{1}l_{1}-gm_{2}l_{2}=0$ ved ligevægt. Dette er en kraft ganget længden, hvilket er et kraftmoment, eller (leveraction.).

#### Fjendul
![[Mindstevirkningsprincippet 2022-10-28 08.50.02.excalidraw]]
0. Vælge koordinater: l(t) og $\theta(t)$
1. $K=\frac{1}{2}m(x^{´}+y^{´})^{2}\Rightarrow \frac{1}{2}m(l^{´2}+l^{2}\theta^{´2})$ 
Lille tangent:
$\frac{dK}{dx}=l^{´}\sin{\theta}+l \cos({\theta})\theta^{´}$
$\frac{dK}{dy}=l^{´}\cos{\theta}-l \sin({\theta})\theta^{´}$
$l^{´2}+l^{2}\theta^{´2}=x^{´2}+y^{´2}=l^{´2}\sin^{2}{\theta}+l^{2}\cos^{2}{(\theta)}\theta^{´2}+2ll^{´}\sin{\theta}\cos{\theta}(\theta^{´})+l^{´2}\cos^{2}{\theta}+l^{2}\sin{\theta^{2}}(\theta^{´2})-2ll^{´}\sin{\theta}\cos{\theta}(\theta^{´})$
$\Rightarrow l^{´2}\sin^{2}{\theta}+l^{2}\cos^{2}{(\theta)}\theta^{´2}+l^{´2}\cos^{2}{\theta}+l^{2}\sin{\theta^{2}}(\theta^{´2})\Rightarrow l^{´2}+l^{2}\theta^{´2}$
Dette sætter vi ind i stedet for x og y i K.
2. $U=\frac{1}{2}k \triangle x +mgh \Rightarrow \frac{1}{2}k \delta l^{2} -\cos{\theta}lmg$ [^2]
3. $L=\frac{1}{2}m(l^{´2}+l^{2}\theta^{´2})+lmg \cos{\theta}- \frac{1}{2}k \delta l^{2}$ 
Vi finder to euler lagrange ligninger, en for l, og en for $\theta$. De bliver altså:
$\frac{d}{dt}(\frac{dL}{d \delta l^{´}})=\frac{dL}{d \delta l}$ Den for længden og:
$\frac{d}{dt}(\frac{dL}{d \delta \theta^{´}})=\frac{dL}{d \theta}$ Den for vinklen $\theta$.
HUSK: $d(t)=l_{0}+\delta l(t)$ 
Jeg laver den for længden.
4. $\frac{dL}{dl}=mg \cos{\theta}-k \delta l$
5. $\frac{dL}{dl^{´}}=m \theta^{´}( \delta l^{´}+l_{0})$ 
6. $\frac{d}{dt}(\frac{dL}{dl^{´}})=m \theta^{´2}( \delta l^{´}+l_{0})$ 
7. $\frac{d}{dt}(\frac{dL}{d \delta l^{´}})=\frac{dL}{d \delta l}\Rightarrow m \delta l^{´´}=m \theta^{´2}( \delta l^{´}+l_{0})+mg \cos{\theta}-k \delta l \Rightarrow \delta l^{´´}= \theta^{´2}( \delta l^{´}+l_{0})+g \cos{\theta}-\frac{k \delta l}{m}$ 

Hvis vinklen går mod nul så bliver:
$dl^{´´}=g- \frac{k \delta l}{m}$

#### Dobbelt pendul
![[Mindstevirkningsprincippet 2022-10-28 09.53.52.excalidraw]]
Bemærk at $l_{1}+l_{2}=$ snorlængden $\Rightarrow l_{1}^{´}+l_{2}^{´}=0 \Rightarrow (l_{1}^{´})^{2}=(-l_{2}^{´})^{2}$

0. Koordinaterne vi vælger er $\theta,l_{2}$
1. $K=\frac{1}{2}mv_{1}^{2}+ \frac{1}{2}mv_{2}^{2} \Rightarrow \frac{1}{2}ml_{1}^{´2}+ \frac{1}{2}m(l_{1}^{´2}+l_{2}^{2}\theta^{´2})$
2. $U=mgh - mgh \Rightarrow mgl_{2}-mg\cos{\theta}l_{2}$ [^3]
3. $L=\frac{1}{2}ml_{1}^{´2}+ \frac{1}{2}m(l_{1}^{´2}+l_{2}^{2}\theta^{´2}) +mg\cos{\theta}l_{2}-mgl_{2}$
4. $\frac{dL}{dl_{2}}=mg-mg \cos{\theta}$ og $\frac{dL}{d \theta}=-mgl_{2} \sin{\theta}$ 
5. $\frac{dL}{dl_{2}^{´}}=ml_{2}^{´}+ml_{2}^{´}$ og $\frac{dL}{d \theta^{´}}=ml_{2}^{2}\theta^{´}$ 
6. $\frac{dL}{dl_{2}}=2ml_{2}^{´´}$ og $\frac{dL}{d \theta^{´}}=ml_{2}^{2}\theta^{´´}$
7. Vi har stadigvæk to ligninger: $\frac{d}{dt}(2ml_{2}^{´})=mg-mg \cos{\theta}$ og $\frac{d}{dt}(ml_{2}^{2}\theta^{´})=-mgl_{2} \sin{\theta}$
Hvis vinklen er lille så rykker loddene sig ikke da: $\sin{\theta}=\theta,\cos{\theta}=1$ så;
$2ml_{2}^{´´}=mg-mg \cos{\theta} \Rightarrow l_{2}^{´´}=0$

Hvis vinklen bliver større så bliver forskydningen
Hvor A er starter amplituden $A=\frac{\theta}{\cos{l_{2}\omega t}}$
$l_{2}^{´´}=gA^{2}\omega^{2}\sin^{2}{\omega t}- \frac{g}{2}A^{2}\cos^{2}{\omega t}$ 



[^1]: Man kan også skrive x' som v, og x'' som a. Dette vil jeg gøre i fremtiden da det er lettere at skrive i $\LaTeX$. Derudover er det også lettere at bruge d, istedet for $\delta$, så det vil jeg også gøre.
[^2]: Hvor $l(t)=l_{0}+\delta l(t)$
[^3]: Hint; man kan vælge to forskellige nulpunkter, en til hver kasse