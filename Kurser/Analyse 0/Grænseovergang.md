#kapitel 
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



## Definition (Grænseværdi 1D)
Lad $f : I \backslash \{ a\}\to \mathbb{R}$ hvor $a \in I$ er et indre punkt i intervallet I, og lad $b \in \mathbb{R}$. Hvis det gælder at $\forall \epsilon > 0 \exists \delta >0$ : $|f(x)-b| < \epsilon$ for alle $x \in I \backslash \{ a\}$ med $|x-a|< \delta$. Så vil f have b som "grænseværdi" i "grænseovergangen" $x \to a$ og dette skrives som... ::: $f(x)\to b$ for $x \to a$


[^1]: Advarsel: Man kan ikke bruge $a \leq x \leq b \Rightarrow |a| \leq |x| \leq |b|$. Brug denne: $a \leq x \leq b \Rightarrow |x| \leq |a|+|b|$