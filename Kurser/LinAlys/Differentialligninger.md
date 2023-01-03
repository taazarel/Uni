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


[^1]: Differentialligninger er meget vigtige for fysikere.
[^2]: I dette kapitel brugte bogen y=y(x) som illustration af ukendte funktioner. I stedet for det normale f, g og h.