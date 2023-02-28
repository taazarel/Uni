#kapitel 
# §4.1 Differentiabilitet i et punkt
## Definition
En funktion $f:I \subset \mathbb{R} \to \mathbb{R}^{m}$ er differentiabel i $a \in I$ med differentialkvotient $f'(a) = c$, hvis... :: $$\frac{f(x)-f(a)}{x-a}\to c \text{ for }x \to a, \space x \in I \Rightarrow \frac{\Delta f}{\Delta x} \to c$$. Her skrives $\Delta f = f(x)-f(a)=f(a+\Delta x)-f(a)$ og $\Delta x = x-a$.[^1]

# §4.2 Middelværdisætningen
## Rolles sætning
Givet en differentiabel funktion som er differentiabel i $x \in (a,b)$ hvis vi så har $f(a)=0, f(b) = 0$. Findes... :: et punkt $\xi \in (a,b)$ så $f'(\xi)=0$. Altså må der være et sted hvor f antager middelværdien.

## Middelværdisætningen
Givet en differentierbar funktion f i $x \in (a,b)$ så findes et punkt $\xi \in (a,b)$ der gør at vi kan finde... :: $f'(\xi )= \frac{f(b)-f(a)}{b-a}$. Hvilket betyder at der skal være mindst ét punkt som har den samme værdi som hældningen fra a til b.
<!--SR:!2023-03-04,4,270-->

# §4.3 Taylors formel for funktioner af én variabel
## Højere ordens differentiablilitet
### $C^{1}$ definition.
En funktion er c1 hvis den... :: er differentiabel i hvert punkt på sit domæne og hvis $f'$ er kontinuert.

## Definition 4.24
For en n gange differentiabel funktion $f: I \to \mathbb{R}$ og et givet punkt $a \in I$. Så kaldes følgen af alle de differentierede... :: Taylorpolynomiet og skrives som $$P_{n}(x)=f(a) + \frac{f'(a)}{1!}(x-a) +...+ \frac{f^{n}(a)}{n!}(x-a)^{n} = \sum_{i=0}^{n} \frac{f^{i}(a)}{i!}(x-a)^{i}$$[^2]
## Udvidet Rolles Sætning (4.28)
Vi har funktionen $g: I \to \mathbb{R}$ som er n gange differentiabel i $I \subset \mathbb{R}$. Vi har to punkter $a,b \in I, \space a \neq b$. Når $g(a)=g'(a)=...=g^{n-1}(a)=g(b)=0$ Siger Rolles udvidede sætning... :: der findes et tal $\xi$ mellem a og b hvor $g^{n}(\xi ) = 0$. 
<!--SR:!2023-03-04,4,270-->

## Taylors formel med restled (4.29)
Givet at rolles sætning er opfyldt kan vi... :: skrive Taylors formel med restled. $$f(b)=f(a)+ \frac{f'(a)}{1!}(b-a) +...+ \frac{f^{n-1}(a)}{(n-1)!}(b-a)^{n-1} + \frac{f^{n}(\xi )}{n!}(b-a)^{n}$$[^3]
<!--SR:!2023-03-04,4,270-->


[^1]: Der er en alternativ formulering for vektorer: $\Delta f = c \Delta x + \epsilon(\Delta x)\Delta x$.
[^2]: Rigtig god for fysik! Taylorpolynomiet har denne egenskab: $p^{n}(a) = f^{n}(a)$.
[^3]: Restleddet kan også skrives som et integral $$\frac{1}{(n-1)!}\int_{a}^{b} f^{n}(t)(b-t)^{n-1}dt$$, men dette kræver at f er $C^{n}$, ikke kun at f er n gange differentiabel.