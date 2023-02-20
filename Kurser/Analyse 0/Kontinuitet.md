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

### Ruselemmaet
Lad $[a_{1},b_{1}]\supset [a_{2},b_{2}]\supset...$ være en følge af intervaller i $\mathbb{R}$ hvor hvert interval er $b_{n+1}-a_{n+1}= \frac{b_{n}-a_{n}}{2}$ for alle $n \in \mathbb{N}$. Siger ruselemmaet at... :: der findes præcist ét tal som indgår i alle mængderne. $\xi \in [a_{n},b_{n}]$.
<!--SR:!2023-02-22,3,250-->

# §3.3 Første hovedsætning
## Sætning 3.21 (Ekstremalværdisætningen)
En funktion som er defineret på et afsluttet og begrænset interval $f:[a,b]\to \mathbb{R}, [a,b]\in \mathbb{R}$. Har... :: en mindste og størsteværdi, og er også begrænset.
<!--SR:!2023-02-23,4,270-->





[^1]: Herfra kan vi beskrive $||f(x)-f(a)|| = ||\triangle f||$ og $||x-a||=||\triangle x||$. Og som $\triangle x \to 0$ så $\triangle f \to 0$. (Nu kan vi også se at ved meget små forskelle bliver $\triangle x \to  dx$ og $\triangle f \to df$).
[^2]: Hvis b er et overtal for A, så er $sup(A)\leq b$.
[^3]: Hvis b er et undertal for A, så er $b \leq inf(A)$.