#forelæsning 
Begyndelsesdato: 07:52   08-11-2022   Uge-45
# Forelæsning
## Komplekse tal
I rækkefølge af størrelse skrives talmængderne således... :: $\mathbb{N}\subseteq \mathbb{Z}\subseteq \mathbb{Q}\subseteq \mathbb{R}\subseteq \mathbb{C}$ hvor $\mathbb{C}$ er de komplekse tal.
<!--SR:!2022-12-01,16,294-->
Vi har de samme regneregler i $\mathbb{C}$ som vi har i $\mathbb{R}$ udover... :: at vi ikke kan bruge uligheder.$<,>,\geq,\leq$ Vi kan ikke fortælle hvilke tal er større end andre.
<!--SR:!2022-11-16,1,210-->
Det vigtigste tal i $\mathbb{C}$ er... :: de komplekse tal, helt specifikt $i=\sqrt{-1}$.
<!--SR:!2022-12-02,17,294-->
Det algebraiske udtryk for $\mathbb{C}$ baseret på reelle tal er... :: givet ved $\mathbb{C}=\{a+ib|a,b \in \mathbb{R} \}$.
<!--SR:!2022-12-01,16,294-->

Definitionen af addition i $\mathbb{C}$ er... :: $(a+ib)+(c+id)=(a+c)+i(b+d)$
<!--SR:!2022-11-30,15,290-->
Definitionen af multiplikation i $\mathbb{C}$ er... :: $zw=(a+ib)(c+id)=(ac-bd)+i(ad+bc)$
<!--SR:!2022-11-29,14,290-->
Definitionen af multiplikation i polarform er... :: $zw=(r_{1}e^{i \theta_{1}})(r_{2}e^{\theta_{2} i})=(r_{1}r_{2})e^{i(\theta_{1}\theta_{2})}$.
<!--SR:!2022-11-16,1,210-->
Definitionen af division i $\mathbb{C}$, givet $\frac{1}{z}\neq \frac{1}{0}$, er... :: $\frac{1}{z}= \frac{1}{a+ib}= \frac{a-ib}{(a+ib)(a-ib)}= \frac{a-ib}{a^{2}+b^{2}}= (\frac{a}{a^{2}+b^{2}})+i(\frac{-b}{a^{2}+b^{2}})$ Man skal huske at forlænge med $a-ib$.[^1]
<!--SR:!2022-12-01,16,290-->
Definitionen af eksponentialfunktionen i $\mathbb{C}$ er... :: $e^{z}=e^{a}(\cos{b}+i \sin{b})\in \mathbb{C}$.[^4]
<!--SR:!2022-11-29,14,290-->

Modulus af w er... :: $\sqrt{w \cdot w}=|w|$
<!--SR:!2022-11-19,4,280-->
<!--SR:!2022-11-16,1,214-->
Værdimængden af den komplekse eksponentialfunktion er... :: hele $\mathbb{C}\backslash 0$ altså alle komplekse tal på nær 0.
<!--SR:!2022-11-19,4,280-->
<!--SR:!2022-11-29,14,290-->
Givet $z=a+ib,w=\frac{1}{a+ib}$ så bliver deres produkt... :: $zw=1=1+i0$.
<!--SR:!2022-12-01,16,294-->
Huskereglen for at regne med komplekse tal er... :: at bruge de sædvanlige regneregler og huske at $i^{2}=-1$.
<!--SR:!2022-11-19,4,280-->
<!--SR:!2022-11-30,15,274-->
Mest for sjov: Hvad er kvadratroden af i? :: $\left(\frac{1}{\sqrt{2}}+ \frac{1}{\sqrt{2}}i\right)$ 
<!--SR:!2022-11-30,15,250-->
Alle komplekse tal har både... :: en reel og kompleks del. ergo $a+ib=c \in \mathbb{C}$.
<!--SR:!2022-12-02,17,294-->

## Geometriske synspunkt
![[Komplekse tal 2022-11-08 08.21.05.excalidraw]]
Hvis vi regner gennem det geometriske synspunkt får vi $ib=$... :: $(0,1)\cdot (b,0)=(0b-10,1b-00)=(0,b)$ og derved $a+ib=(a,0)+(0,b)=(a,b)$
<!--SR:!2022-12-02,17,294-->

## Kompleks konjugering
Givet $z=a+ib,\vec{z}=a-ib.a,b \in \mathbb{R}$ så bliver produktet af de komplekse tal... :: $\vec{z}z \in \mathbb{R}|\vec{z}z \geq 0$ og hvis $z=0\Rightarrow z \vec{z}=0$
<!--SR:!2022-11-21,6,234-->
### Sætning 3.1.5
For alle $z,w \in \mathbb{C}$ er vores regneregler for vektorer... :: $\vec{z}+\vec{w}=\vec{z+w}$, $\vec{z}-\vec{w}=\vec{z-w}$, $\vec{z}\cdot \vec{w}=\overrightarrow{zw}$, $\frac{\vec{z}}{\vec{w}}= \vec{\frac{z}{w}}$ givet $w \neq 0$.
<!--SR:!2022-11-29,14,274-->
Definitionen af $|z|$ er... $\sqrt{z \vec{z}}\in \mathbb{R}\Rightarrow \sqrt{a^{2}+b^{2}}\geq 0$ så vi kan kun få $|z|=0$ hvis $z=0$.
En god huskeregel er den udvidede form af $0\leq a^{2}+b^{2}\in \mathbb{R}=(a+ib)(a-ib)$[^2]
### Polarform
Vi kan bruge polære koordinater til at vise $|z|$ bedre... :: ![[Komplekse tal 2022-11-08 09.06.42.excalidraw]] $|z|=r$ hvor $a=r \cos{\theta },b=r \sin{\theta }$.[^3]
<!--SR:!2022-12-02,17,294-->
Definitionen af z i polarform er... :: $z=r \cos{\theta }+ir \sin{\theta }=re^{i \theta }$ 
<!--SR:!2022-12-01,16,270-->
Vi kan definere r som... :: $r=\sqrt{a^{2}+b^{2}}$ 
<!--SR:!2022-12-01,16,294-->
### Sætning
For alle $z,w \in \mathbb{C}$ så får vi $e^{z+w}=$... :: $e^{z}e^{w}=e^{(a+c)+i(b+d)}$
<!--SR:!2022-11-30,15,294-->
For eksponenter i eksponenter kan vi skrive... :: $(e^{z})^{n}=e^{z}_{1}\cdot ...\cdot e_{n}^{z}=e^{nz}$.
<!--SR:!2022-12-02,17,290-->
Hvis vi har $z=i \theta$ så kan vi udvide til dette i polarform... :: $(\cos{\theta }+i \sin{\theta })^{n}=e^{i n \theta }=\cos{}(n \theta )+i \sin{(n \theta )}=e^{i \theta }$.
<!--SR:!2022-11-19,4,280-->
<!--SR:!2022-11-25,10,270-->

Vi definerer ikke disse operationer
?
$\ln(z)$
$z^{w}$
$\cos^{-1}{z}$
<!--SR:!2022-11-14,3,250-->


### De fem vigtigste tal i matematik
$$e^{i \pi }-1=0$$
# Fodnoter
[^1]: Dette gør nævneren til et reelt tal.
[^2]: Dette er også hvad vi bruger i definitionen ovenover.
[^3]: Denne kaldes den polære form, eller bare polarform.
[^4]: Her er modulus af $\cos{b}+i \sin{b}=1.$