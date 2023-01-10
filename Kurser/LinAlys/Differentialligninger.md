#forelæsning 
Begyndelsesdato: Kl. 08:10  Den 03-01-2023   Uge-1
# §10 TL
## Definition (Differentialligninger)
En differentialligning består af... :: En ligning med en funktion som ukendt, og en højere differentieret.[^1]

### Eksempel
$$f'(x)+2xf(x)=x$$
Har løsningen $$f(x)=e^{-x^{2}}+ \frac{1}{2} \Rightarrow f'(x)=-2x e^{-x^{2}}$$
Så kan vi indsætte for at tjekke efter
Her er $f(x)=\frac{1}{2}$ også en løsning.
### Eksempel med fysik
GIvet et faldende objekt har nået terminal velocity så er dens bevægelsesligning: $0=mg-kv$ Her kan vi også skrive $0=m \dot v-kv$, altså har vi en differentialligning.
Her er $v(t)$ altså den ukendte funktion.
Vi finder $\dot v(t)+ \frac{k}{m}v(t)=g$.

## Første ordens lineære differentialligninger[^2]
En første ordens lineær differentialligning er givet ved $f,g:I \to \mathbb{R}$ er kontinuerte, $g(x)=...$::$y'(x)+f(x)y(x)$. Ofte skriver man bare $g=y'+fy$.

## Sætning 10.1.3 (Generel Løsning)
Givet $I \subseteq \mathbb{R}$ er et åbent interval, $f,g:I \to \mathbb{R}$ er kontinuerte. Da er løsningerne til $g=y'+fy$ givet ved... :: $$y(x)=e^{-F(x)}\cdot \left(\int_{}^{} e^{F(x)}g(x)dx+C\right)$$ hvor $C \in \mathbb{R}$ og $F:I \to \mathbb{R}$ er stamfunktionen til f.

## 10.3.1 Med begyndelsesbetingelser
Givet $I \subseteq \mathbb{R}$ er et åbent interval, $f,g:I \to \mathbb{R}$ er kontinuerte, og $y(c)=d$, hvor $c \in I,d \in \mathbb{R}$. Så har vi netop én løsning givet ved... :: $$y(x)=e^{-\int_{c}^{x}f(t)dt}\left(\int_{c}^{x}\left(g\left(t\right)e^{\int_{c}^{t}f(s)ds}\right)dt+d \right) $$
# §10.4 Seperation af variable
## Definition (Seperation af Variable)
Givet $p,q: I \to \mathbb{R}$ er kont. så kan vi skrive... :: $q(y(x))y'(x)=p(x)$. Der er et trick som hedder $\frac{d}{dx}q(y(x))=p(x)$.
## Løsning (Seperation af Variable)
Når man har defineret sin ligning kan vi skrive løsningen som... :: $$\int_{}^{} q(y(x))dy=\int_{}^{} p(x)dx$$
# §10.5 Anden ordens homogen differentialligning
Vi kan finde en anden ordens diff. ligning således hvis den er homogen... :: $y''(x)+p(x)y'(x)+q(x)y(x)=0$ hvilket skrives som dette i fysik $\ddot y(x)+p(x)\dot y(x)+q(x)y(x)=0$.
## Lemma 10.5.1
Givet $y_{1},y_{2}: \mathbb{R}\to \mathbb{R}$ kan løse diff. ligning af anden orden $y''+py'+qy=0$, hvor $C,D \in \mathbb{R}$ er konstanter. Så kan diff. ligningerne også løse... :: $y(x)=Cy_{1}(x)+Dy_{2}(x)$ således.
### Konsekvens af lemma 10.5.1
Givet at dette lemma er sandt vil y blive et underrum skrevet som... :: $\{y:\mathbb{R}\to \mathbb{R}|y''+py'+qy=0 \} \subseteq \mathbb{F_{R}}$.[^3]
## Løsning af andenordens diff. ligning
Givet et 2-dimensionalt underrum og ligningen $y''+py'+qy=0$ så kan vi finde løsningen ved først at udregne... :: andengradspolynomiet $r^{2}+pr+q=0$ hvor $r \in C$ og $y: \mathbb{R}\to \mathbb{R}$ er ubekendte. $D=p^{2}-4q \in \mathbb{R}$.
Når man har løst andengradspolynomiet kan vi finde løsningen af diff. ligningen ved... :: $y_{1}(x)=e^{r_{1}x}\text{ og }y_{2}(x)=e^{r_{2}x}$ er løsninger til diff. hvor $r_{1}\text{ og }r_{2}$ er to reelle rødder. Vi ved også at de differentierede af y bliver $y'(x)=r_{i}e^{r_{i}x}$ og $y''(x)=r_{i}^{2}e^{r_{i}x}$.

Vi finder at løsningen kan skrives som $y''+py'+qy=(r_{i}^{2}+pr_{i}+q)e^{r_{i}x}$. og så at gøre det med både r1 og r2.
## Sætning 10.5.3 Generel løsning til diff ligninger af anden orden.
Givet $D=p^{2}-4q>0$ så er løsningen... :: $y(x)=Ce^{r_{1}x}+De^{r_{2}x}$. hvor $C,D \in \mathbb{R}$ ikke er det samme som D for determinanten.
Andet tilfælde af den generelle løsning. Hvis vi har at $D=0$ så får vi én reel dobbelrod og to løsninger... :: $y_{1}(x)=e^{rx}$ og $y_{2}(x)=xe^{rx}$.
Det tredje tilfælde af den generelle løsning, givet at $D<0$ får vi to komplekse rødder $r_{1}=a+ib$, $r_{2}=a-ib$, og to løsninger... :: $y_{1}(x)=e^{ax}\cos{bx}$ og $y_{2}(x)=e^{ax}\sin{bx}$




[^1]: Differentialligninger er meget vigtige for fysikere.
[^2]: I dette kapitel brugte bogen y=y(x) som illustration af ukendte funktioner. I stedet for det normale f, g og h.
[^3]: VI kan se at dette er en kerne af en operation, hvilket betyder at vi også kan beskrive dette underrum som en lineær operator. da der også eksisterer et billede som er onto.