# Kapitel 10
### Kogebog til Partikelproblemer
1. Vælg et inertialkoordinatsystem
2. Undersøg om vi har energibevarelse $\Delta E = 0$ eller impulsbevarelse $\Delta p = 0$. Hvis én eksisterer gør de begge da de hænger sammen. Skriv deres løsninger ned.
3. Brug formlen $E^{2}-p^{2}=m^{2}$
4. Brug formlen $\vec{v}= \frac{\vec{p}c^{2}}{E^{2}}$

## 10.1
Virkningen i relativitetsteori skrives som... :: $S=K \int_{}^{}d \tau$. Hvor tau er egentid.
<!--SR:!2023-03-28,60,290-->
Ved at indsætte den ikke relativistiske virkning $L_{non-rel}=\frac{1}{2}mv^{2}$ i Virkningen for relativitet, Finder vi... :: $L=K \sqrt{1-v^{2}}$ og for at dette skal være sand skal K være -m. Så vi får $L=\frac{-mc^{2}}{\gamma }$ (10.6)
<!--SR:!2023-01-30,3,250-->
Virkningen, med lysets hast genindført skrives som... :: $$S=-mc^{2} \int_{i}^{f} \frac{1}{\gamma }dt$$ (10.7)
<!--SR:!2023-02-20,24,270-->

## 10.2
Den relativistiske impuls bliver beskrevet ved... :: $p= \gamma mv$[^1] (10.9) Vi kan også omskrive dette til $p=m \frac{dx}{d \tau }$ da $\gamma v = \gamma \frac{dx}{dt}$.
<!--SR:!2023-03-22,54,290-->
Invarianten tau, som betegner egentid findes gennem de to ikke invarianter... :: $\tau ^{2}=t^{2}-x^{2}$. (10.91)
<!--SR:!2023-03-29,61,290-->

## 10.3
Hvis vi benytter formlen for den totale energi (5.30) sammen med (10.6) finder vi den relativistiske energi er dette... :: $E=m \gamma$ og hvis vi indfører lysets hastighed igen får vi $E=\gamma mc^{2}$.
<!--SR:!2023-03-24,56,290-->
Massen er en invariant størrelse som kan findes ved... :: $m^{2}=E^{2}-p^{2}$. (10.33)
<!--SR:!2023-03-21,53,290-->
Egentiden er en invariant størrelse som kan findes ved... :: $\tau ^{2}=t^{2}-x^{2}$
<!--SR:!2023-03-24,56,290-->
Center af momentum kan findes mellem to partikler således... :: $$\frac{v_{cm}}{c}= \frac{1-\frac{1}{\gamma}}{\frac{v_{i}}{c}}= \frac{1-\sqrt{1-\frac{v^{2}}{c^{2}}}}{\frac{v}{c}} $$
<!--SR:!2023-03-17,49,270-->

## 10.4
Vi kan finde hastigheden af en partikel ved at bruge energi og impuls... :: $\vec{v}= \frac{\vec{p}}{E}$ (10.34)
<!--SR:!2023-03-27,59,290-->
For en masseløs partikel, såsom fotoner er deres energi... :: $E_{foton}=p_{foton}c$ Og dette finder vi fra (10.33).
<!--SR:!2023-01-30,3,241-->
Når vi har at der findes enten impuls eller energikonstanthed så er... :: det sandt for alle koordinatsystemer. Og det betyder også at den anden er sand.
<!--SR:!2023-03-22,54,290-->
Energikonstanthed i relativitetsteori skrives som... :: $E_{i}=\gamma mc^{2}=m=E_{f}=E_{1}+E_{2}$
<!--SR:!2023-03-25,57,290-->
Impulskonstanthed i relativitetsteori skrives som... :: $\vec{p_{i}}=\gamma mv=1m(0)=0=\vec{p_f}=\vec{p_{1}}+\vec{p_{2}}$[^2]
<!--SR:!2023-03-23,55,290-->

## 10.5
Kig de her eksempler igennem når du har mere tid. Vi vil gerne bruge dem til at styrke forståelsen af arbejdsspørgsmål.

## 10.6 4-vektorer
Hvis en 3-vektor er en vektor som transformeres gennem rotation i et 3-dimensionelt rum så er 4-vektorer... :: en vektor som kan transformeres i et 4-dimensionalt rum gennem lorentztransformationer. Og kan skrives $a=(a_{0},a_{1},a_{2},a_{3})=(t,x,y,z)$.
<!--SR:!2023-03-26,58,290-->

Givet $a=(a_{0},a_{1},a_{2},a_{3})=(t,x,y,z)$ er en 4-vektor så skrives den transformeret gennem lorentztransformationerne...
?
$t'=\gamma (t-vx)$
$x'=\gamma (x-vt)$
$y'=y$
$z'=z$[^3]
<!--SR:!2023-03-20,52,270-->

Vi kan manipulere 4-vektorer da de bliver transformeret lineært af LT(Lorentz Transformationer). Så hvis vi vil have hastighedsvektoren kan vi skrive... :: Tage forskellen mellem to vektorer, og dividere med invarianten $d \tau$ $$v=\left(\frac{dt}{d\tau}, \frac{dx}{d\tau}, \frac{dy}{d\tau}, \frac{dz}{d\tau}\right)$$ Dette kan omskrives til $$v=(\gamma ,\gamma \vec{v})$$[^4]
<!--SR:!2023-01-30,3,250-->

Vi finder energi-impulsvektoren, en 4-vektor som beskriver P ved at transformere hastighedsvektoren. Vi ganger den invariante masse på og finder... :: $P=(\gamma m, \gamma m \vec{v})=(E,\vec{p})$. (10.88)[^5]
<!--SR:!2023-03-26,58,290-->

Helt generelt gælder det at et indre produkt af 4-vektorer er invariant. Vi skriver... :: $\langle a,b \rangle =a_{0}b_{0}- \langle \vec{a},\vec{b}\rangle$ (10.93)
<!--SR:!2023-03-25,57,290-->

4-vektoren for acceleration findes ved at differentiere med $\tau$ på hast-vektoren... :: $$A=\left(\gamma ^{4}v \dot v, \gamma ^{4}v \dot v \vec{v}+ \gamma ^{2} \frac{d\vec{v}}{dt}\right)$$ (10.95)
<!--SR:!2023-02-18,22,250-->

Vi kan finde 4-vektoren for kraft gennem energi-impulsvektoren (10.88)... :: $F=\left(\frac{dE}{d \tau }, \frac{d\vec{p}}{d \tau}\right)$ (10.96). Når vi har konstant m, så kan vi skrive $F=mA=m\left(\gamma ^{4}v \dot v, \gamma ^{4}v \dot v \vec{v}+ \gamma ^{2} \frac{d\vec{v}}{dt}\right)$ (10.97)
<!--SR:!2023-01-30,3,230-->


# Fodnoter
[^1]: Når vi har en gamma tæt på 1. Betyder det bare at v er så lille at relativitet ikke spiller en rolle.
[^2]: Både energikonstanthed og impulskonstanthed gælder da v=0. Her er m og v i forhold til hele systemet. Det er pi og pf, Ei og Ef også.
[^3]: Disse to sidste antager at vi ikke bevæger os i disse dimensioner i forhold til et andet koordinatsystem.
[^4]: Dette gælder da $dt=\gamma d \tau$. 
[^5]: HUSK: MEGET VIGTIGT: da dette er en 4-vektor kan vi bruge LT på den.