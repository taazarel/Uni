# §3.1 Kontinuitet i et punkt
Der er kontinuitet i et punkt hvis... :: grænseværdien fra begge sider og funktionsværdien er den samme værdi. $||f(x)-f(a)||< \epsilon$. for $||x-a||< \delta$.[^1]
<!--SR:!2023-02-23,4,270-->

# §3.2 Kontinuerte funktioner
En funktion siges at være kontinuert hvis... :: Funktionen er kontinuert i alle punkter hvor den er defineret. 
<!--SR:!2023-02-23,4,270-->

Supremum af en mængde er det mindste overtal for mængden og skrives som... :: $\forall x \in A: x \leq sup(A)$[^2]
<!--SR:!2023-02-22,3,250-->
Kontinuitetsaksiomet siger at... :: enhver opadbegrænset mængde har et supremum
<!--SR:!2023-02-22,3,250-->
Det største undertal hedder infimum af mængden. Det skrives som... :: $\forall x \in A: x \geq inf(A)$.[^3]
<!--SR:!2023-02-23,4,270-->

En global kontinuert funktion bliver defineret som... :: $\forall \vec{a}>0\space \forall \epsilon >0\space \exists \delta >0:\space ||f(x)-f(a)||<\epsilon$ for alle $x \in A$ med $||x-a||<\delta$.[^4]
<!--SR:!2023-02-26,4,276-->

### Ruselemmaet
Lad $[a_{1},b_{1}]\supset [a_{2},b_{2}]\supset...$ være en følge af intervaller i $\mathbb{R}$ hvor hvert interval er $b_{n+1}-a_{n+1}= \frac{b_{n}-a_{n}}{2}$ for alle $n \in \mathbb{N}$. Siger ruselemmaet at... :: der findes præcist ét tal som indgår i alle mængderne. $\xi \in [a_{n},b_{n}]$.
<!--SR:!2023-02-22,3,250-->

# §3.3 Første hovedsætning
## Sætning 3.21 (Ekstremalværdisætningen)
En funktion som er defineret på et afsluttet og begrænset interval $f:[a,b]\to \mathbb{R}, [a,b]\in \mathbb{R}$. Har... :: en mindste og størsteværdi, og er også begrænset.
<!--SR:!2023-02-23,4,270-->

# §3.4 Anden Hovedsætning
## Skæringssætningen
For en kontinuert funktion $f:[a,b]\to \mathbb{R}$ hvor $[a,b]\subset \mathbb{R}$ vil billedmængden $f([a,b])$... :: indeholde alle tal mellem $f(a)$ og $f(b)$.
<!--SR:!2023-02-25,3,256-->

### Korollar 3.25
Et hvert interval I's billedmængde $f(I)$ er... :: Også et interval, så længe at billedet er bijektivt.
<!--SR:!2023-02-26,4,276-->

For enhver funktion som er strengt voksende, som har et interval som billedmængde... :: Er der en invers funktion $f^{-1}$ af funktionen $f$, som har billedmængden af f's interval. [^5]
<!--SR:!2023-02-26,4,276-->


# §3.5 Tredje Hovedsætning
## Definition 3.33 (Uniform Kontinuitet)
En uniform kontinuert funktion er... :: En stærkere definition på kontinuitet, hvor $\delta$ kun er afhængig af $\epsilon$ og ikke x. Vi kan skrive $$\forall \epsilon > 0 \space \exists \delta>0\space : ||f(\vec{y})-f(\vec{x})||<\epsilon \text{ for } x,y \in A\space ||y-x||<\delta$$
## Definition 3.36 (Lipschitz afbildninger)
En afbildning $f: A \to \mathbb{R}^{m}$ af en mængde $A \subset \mathbb{R}^{k}$ er "Lipschitz", hvis der findes en konstant K[^7] så... :: $||f(y)-f(x)||\leq K||x-y|| \text{ for alle }x,y \in A$.[^6]

## Hovedsætning 3
Enhver kontinuert funktion på et afsluttet og begrænset interval er... :: automatisk også Uniform kontinuert.



[^1]: Herfra kan vi beskrive $||f(x)-f(a)|| = ||\triangle f||$ og $||x-a||=||\triangle x||$. Og som $\triangle x \to 0$ så $\triangle f \to 0$. (Nu kan vi også se at ved meget små forskelle bliver $\triangle x \to  dx$ og $\triangle f \to df$).
[^2]: Hvis b er et overtal for A, så er $sup(A)\leq b$.
[^3]: Hvis b er et undertal for A, så er $b \leq inf(A)$.
[^4]: Hvor afbildningen $f:A \to \mathbb{R}$ hvor $A \subset \mathbb{R}^{k}$.
[^5]: Tag fx exp og log, eller kvadratroden til x og x^2.
[^6]: Vi kan her se at denne altid må være uniform kontinuert.
[^7]: Kaldes også en "Lipschitz konstant"