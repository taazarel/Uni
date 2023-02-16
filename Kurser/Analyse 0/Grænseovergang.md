#kapitel 
# §2.1 Grænseovergang i 1D
## Strategi til Epsilon delta gymnastik
- Hav et gæt, eller tanke om hvad grænseværdien b er.
- Undersøg relationen mellem $|f(x)-b| \text{ og } |x-a|$.
- Vælg så en "Afpareringsstrategi"
### True strike formler (Afpareringsstrategier)
Der er en række kriterier som skal opnåes før vi kan få en sikker gevinst.[^1]
1. Kriterie; Hvis det gælder for et passende C > 0 gælder at: $|f(x)-b| \leq C|x-a|$ for alle $x \in I \backslash \{ a\}$. Kan man parere ved...
2. Kriterie; Hvis der for et passende C > 0 gælder: $|f(x)-b|\leq C|x-a|^{2}$ for alle $x \in I \backslash \{ a\}$. Så kan vi...
3. Kriterie; Hvis der for et passende C > 0 og $\delta_{0}>0$ gælder at $|f(x)-b|\leq C|x-a|$ for alle $x \in I \backslash \{ a\}$ med $|x-a|<\delta_{0}$. Kan vi afparere med...
?
- at vælge $\delta = \delta (\epsilon )= \frac{\epsilon}{C}$ for et givet $\epsilon >0$. Hvis $|x-a|<\delta$
- vinde over et givet $\epsilon >0$ ved at vælge $\delta (\epsilon )= \sqrt{\frac{\epsilon}{C}}$.
- $\delta (\epsilon )=min \{\frac{\epsilon}{C},\delta_{0} \}$ for et givet $\epsilon > 0$.
 

## Definition 2.1 (Grænseværdi 1D)
Lad $f : I \backslash \{ a\}\to \mathbb{R}$ hvor $a \in I$ er et indre punkt i intervallet I, og lad $b \in \mathbb{R}$. Hvis det gælder at $\forall \epsilon > 0 \space\exists \delta >0$ : $|f(x)-b| < \epsilon$ for alle $x \in I \backslash \{ a\}$ med $|x-a|< \delta$. Så vil f have b som "grænseværdi" i "grænseovergangen" $x \to a$ og dette skrives som... ::: $f(x)\to b$ for $x \to a$

# §2.3 Grænseovergang i flere dimensioner
## Definition 2.15 (Grænseværdi i flere dimensioner)
Grænseovergangen er det samme som i 1D, bortset fra... :: at vi bruger vektorer i stedet for punkterne x, b, og a. Og vi bruger norm i stedet for numerisk værdi $||f(\vec{x})-\vec{b}||<\epsilon$ og $||\vec{x}-\vec{a}||<\delta$.

# §2.4 Sætninger om Grænseovergang
## Sætning 2.27 (Koordinatvis grænseovergang)
Lad $f = (f_1,...,f_{m}):A\to \mathbb{R}^{m}$ være en afbildning defineret på $A \subset \mathbb{R}^{k}$ og a er et randpunkt på A og $b =(b_{1},...,b_{m})\in \mathbb{R}^{m}$. Ved grænseovergangen vil det gælde at... :: $f(\vec{x})\to \vec{b} \Leftrightarrow (f_{1}(\vec{x})\to b_{1},...,f_{m}(\vec{x})\to b_{m})$.


# §2.5 Variationer af grænseværdibegrebet 1D
## Definition (Etsidede grænser)
Lad $I \subset \mathbb{R}$ være vore interval. $f:I \to \mathbb{R}^{m}$ og $a \in I$. Hvis vi er givet et epsilon kan vi finde to grænser, nemlig... :: $f(x)\to \vec{b}$ for $x \to a^{+}$ hvilket betyder at man går mod a fra den højre side. Vi definerer $x \in (a, a+\delta)$. Vi finder også $f(x)\to \vec{c}$ for $x \to a^{-}$, fra den venstre side, x bliver $x \in (a- \delta, a)$.

# §2.6 Størrelsesordener


[^1]: Advarsel: Man kan ikke bruge $a \leq x \leq b \Rightarrow |a| \leq |x| \leq |b|$. Brug denne: $a \leq x \leq b \Rightarrow |x| \leq |a|+|b|$