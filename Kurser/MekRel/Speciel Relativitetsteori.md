# Se også
[[Forelæsning den 12 december]] for hvad vi vil opstille i kurset.

# Kogebog
1. Lav en skitse
2. Opstil et rumtidsdiagram
3. Hvad skal findes? Hvilke variable, normalt er det langt x' aksen.
4. Vælg den "rigtige" LT (Lorentz transformation)
5. Regne, regne $\Rightarrow$ fortolk.

# 9.1 Lysets hastighed
Lysets hastighed er altid konstant, dette kan lade sig gøre fordi... :: uanset hvilken fart du har kan rumtiden bøjes, derfor kan lys altid have c som sin fart (i vakuum).
<!--SR:!2023-01-08,20,290-->
Lysets hastighed er... :: Den hurtigste information i universet. Skrives med c. og har størrelsen: $10 \cdot 10^{8} \frac{m}{s}$.
<!--SR:!2023-01-06,18,290-->
Ofte bruger vi dette til at måle distance... :: distancen lyset tilbagelægges over et givent interval i tid. Set som fx lyssekund og lysår.
<!--SR:!2023-01-05,17,290-->


# 9.2 Speciel Relativitetsteori
Ifølge Einsteins teori er
Lysets hastighed...
Tid...
Rum...
?
Uafhængigt af observantes hast
Tid og rum er begge ikke absolutte, men Rumtid, hvad de begge er en del af **er** absolut. Dette betyder blot at deres forhold skal ændres men både tid og rum kan strækkes og presses.

Rumtid kan plottes i to dimensioner således... :: som en kegleform, hvor randen er lysets hast. ![[Pasted image 20221209150323.png]].
<!--SR:!2023-01-09,21,290-->

# 9.3 Koordinat Transformationer

For at finde en transformation mellem to observanters synspunkter skal vi... :: Opskrive en transformation mellem deres koordinatsystemer som er relative til dem.
<!--SR:!2023-01-09,21,290-->
For at vise problemet med Transformationen mellem to inertial koordinatsystemer set som Newtons tid og rum kan vi opskrive: $x'=x-vt$ eller $x=x'+vt'$ og $t'=t$. Hvis vi nu havde en til partikel kunne vi beskrive hastigheden således $x=v_{2}t$ og $x'=(v_{2}-v)t'$. Og hvis dette er sandt får vi et problem når... :: Vi bruger denne transformation for et foton. Så vil lysets hastighed ændre sig baseret på hvem der observerer det, og derfor vil vi have modstrid med Maxwells ligninger.![[Pasted image 20221209161024.png]]
<!--SR:!2023-01-07,19,290-->

# 9.4 Samtidighed
Samtidighed for ens eget synspunkt vises som... :: en horisontal linje i rumtidsdiagrammet.
<!--SR:!2022-12-23,4,288-->
Samtidighed for en anden persons inertialsystem vises som... :: en lige linje der danner en vinkel med referencepunktets samtidighed.[^1]
Vi kan lave tre linjer i et rumtidsdiagram når vi har et andet synspunkt repræsenteret i det... :: som er Et objekt der sidder stille $x=vt$, et foton $x=t$ og samtidighedslinjen $t=vx$ 
<!--SR:!2022-12-23,4,288-->
Hvis vi indfører lysets hast i linjerne for rumtidsdiagrammet $x=vt,x=t \text{ og }x=\frac{t}{v}$ så får vi... :: $x=vt \text{ for et stille objekt},x=ct \text{ for et foton }, t=\frac{vx}{c^{2}} \text{ for samtidigheden}$
<!--SR:!2022-12-23,4,288-->
Kausalitet siger at... :: når begivenhed A laver begivenhed B så sker A før B, og alle synspunkter kan sige dette.[^2]

Vi kan aldrig blive enige om rækkefølge af A så B i... :: Spacelike begivenheder da vi kan finde forskellige synspunkter til dem.
Vi kan blive enige om rækkefølge af A så B i... :: Timelike begivenheder da vi aldrig kan få en hældning med mere end 45 grader (Lysets graf)
<!--SR:!2022-12-23,4,288-->

# 9.5 Lorentz Transformation
Regulært koordinatsystem = det som står stille.
Hvis x' bevæger sig mod højre fra x så finder vi:
1. Vi kan finde placeringen i et regulært koordinatsystem (x',t') ved...
2. Vi kan finde tiden i et regulært koordinatsystem ved...
3. Hvis vi sammensætter $x'=(x-vt)h(v^{2})$ med $t'=(t-vx)k(v^{2})$ får vi...
4. Vi kan også skrive 1. og 2. som set fra det bevægende system således...
?
 1. $x'=(x-vt)h(v^{2})$ (9.24) hvor h er afhængig af v, altså både tid og rum. Og v er i anden da der ikke er nogen foretrukken retning i rummet.
 2. $t'=(t-vx)k(v^{2})$ (9.25)
 3. at h og k er den samme funktion da $x=t$ og $x'=t'$.[^3]
 4. $x=(x'+vt')h(v^{2}),t=(t'+vx')h(v^{2})$, da det blot vil være at ændre fortegnet.
<!--SR:!2022-12-23,4,288-->

Lorentz-faktoren skrives som $\gamma (v)=...$::$$\frac{1}{\sqrt{1-v^{2}}}$$ (9.28)

Koordinat transformationerne for lorentz transformationer er opsamlet nedenunder, på den anden side er med c. Her er det bare c=1. 
1. $t'=\gamma (t-vx)$...
2. $x'=\gamma (x-vt)$...
3. $t=\gamma (t'+vx')$...
4. $x=\gamma (x'+vt')$...
5. $\gamma = \frac{1}{\sqrt{1-v^{2}}}$...
?
1. $t'=\gamma (t- vx/c^{2})$
2. $x'=\gamma (x-vt)$
3. $t=\gamma (t'+ \frac{vx'}{c^{2}})$
4. $x=\gamma (x'+vt')$
5. $\gamma = \frac{1}{\sqrt{1- \frac{v^{2}}{c^{2}}}}$

[^1]: Dette sker da lysets hast altid danner rette vinkler fra begge sider. Så to linjer der skærer det samme punkt, for et system som bevæger sig(Har skæve tidslinjer) betyder at deres skæringspunkt ikke bliver den samme tid for samme distance. Vi kan herfra tegne en linje mellem disse punkter, og dette vil være samtidigheden af det andet referencesystem.
[^2]: Dette virker ikke for begivenheder som sker forskellige steder i rummet.