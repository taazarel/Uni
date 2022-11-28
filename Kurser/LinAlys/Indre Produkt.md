#forelæsning 
Begyndelsesdato: 07:54   10-11-2022   Uge-45
# Forelæsning
W er en operation $\langle ,\rangle$, som hedder det indre produkt, og givet er $\vec{v},\vec{w}\in V$, vi bruger W på vektorerne og får... :: $\langle \vec{v},\vec{w}\rangle\in \mathbb{R}$.
<!--SR:!2022-12-24,26,290-->
Liste af aksiomer:
For alle $\vec{v}\in V:\langle \vec{v},\vec{v}\rangle\geq 0$ og hvis $\langle \vec{v},\vec{v}\rangle=0$ så får vi... :: $\vec{v}=\vec{0}$ (i)
<!--SR:!2022-12-15,24,301-->
For alle $\vec{v},\vec{w}\in V$ er $\langle \vec{v},\vec{w}\rangle=$.... :: $\langle \vec{w},\vec{v}\rangle$.  (ii)
<!--SR:!2022-11-30,15,290-->
For alle $\vec{v},\vec{w}\in V$, $r \in \mathbb{R}$ er $\langle r \vec{v},\vec{w}\rangle=$... :: $r\langle \vec{v},\vec{w}\rangle$ (iii)
<!--SR:!2022-12-01,16,297-->
For alle $\vec{v},\vec{w},\vec{x}\in V$ er $\langle \vec{v}+\vec{w},\vec{x}\rangle=$.... :: $\langle \vec{v},\vec{x}\rangle+\langle \vec{w},\vec{x}\rangle$ (iv)
<!--SR:!2022-11-30,15,290-->
Givet $\vec{v},\vec{w}\in V$ og at vi har $\langle \vec{v},\vec{w}\rangle$ får vi... :: $\vec{v_{1}}\vec{w_{1}}+...+\vec{v_{n}}\vec{w_{n}}\in \mathbb{R}$ (v)[^1]
<!--SR:!2022-12-01,16,297-->

## Definition af Standard indre produktet
Hvis vi har $f,g [a,b]\to \mathbb{R}$ så kan vi tage deres indre produkt... :: $\langle f,g\rangle=\int_{a}^{b} f(t)g(t)dt \in \mathbb{R}$.[^2]
<!--SR:!2022-12-15,24,277-->

## Sætning
Lad $\langle , \rangle$ være et indre produkt på V Da er $\langle \vec{v},\vec{0} \rangle=$... :: $0$ for alle $\vec{v}$
<!--SR:!2022-11-30,15,297-->
Indre produkt rum betyder... :: et vektorrum V og et indre produkt.
<!--SR:!2023-01-17,50,297-->
Vi kan vise afstanden til $\vec{0}\in \mathbb{R}^{2}$ som... :: $\sqrt{\vec{v_{1}}^{2}+\vec{v_{2}}^{2}}=\sqrt{v \cdot v}$
<!--SR:!2022-12-16,25,301-->
Vi kan vise afstanden til $\vec{0}\in \mathbb{R}^{n}$ som... :: $\sqrt{\vec{v_{1}}^{2}+...+\vec{v_{n}}^{2}}=\sqrt{\vec{v}\cdot \vec{v}}$.
<!--SR:!2022-12-03,18,305-->
Vi definerer afstanden til $\vec{0}\in \mathbb{R}^{n}$ som $||\vec{v}||=$... :: $\sqrt{\vec{v}\cdot \vec{v}}$ Hvis dette er et indre produkt i V, så bliver det til$\sqrt{\langle \vec{v},\vec{v} \rangle}\geq 0$.[^3]
<!--SR:!2022-11-30,15,290-->
Vi definerer vinklen mellem $\vec{v},\vec{w}\in \mathbb{R}^{n}$ som... :: $\vec{v}\cdot \vec{w}=||\vec{v}||\cdot ||\vec{w}||\cos{\theta }\Rightarrow$ $\frac{\vec{v}\cdot \vec{w}}{||\vec{v}||\cdot ||\vec{w}||}=\cos{\theta }\Rightarrow \theta =\cos^{-1}{\left(\frac{\langle\vec{v},\vec{w}\rangle}{||\vec{v}||\cdot ||\vec{w}||}\right)}$.[^4]
<!--SR:!2022-12-06,15,281-->
Hvis $\langle \vec{v},\vec{w}\rangle=0$ så kaldes vektorerne... :: ortogonale på hinanden.[^5]
<!--SR:!2022-12-21,23,290-->
Pythagoras i vektorrumet som har indre produkter er... :: $||\vec{v}-\vec{w}||=||\vec{v}||^{2}+||\vec{w}||^{2}-2\langle \vec{v},\vec{w}\rangle$ hvor $\langle \vec{v},\vec{w}\rangle =||\vec{v}||\cdot ||\vec{w}||cos(\theta )$[^6]
<!--SR:!2022-12-14,23,257-->

Ortogonalproduktet af $\vec{w}\text{ på }\vec{v}$ er... :: $\frac{\langle \vec{v},\vec{w}\rangle}{\langle \vec{v},\vec{v}\rangle}\vec{v}$
<!--SR:!2022-12-17,26,301-->

# Fodnoter
[^1]: Dette er det samme som prikproduktet af $\vec{v}\cdot \vec{w}$.
[^2]: Herefter kan vi benytte aksiomerne på dette integral.
[^3]: Dette kaldes også normen af $\vec{v}\in V$.
[^4]: Vi skal tjekke at $||\vec{v}||,||\vec{w}||\neq 0$. Ellers er theta ikke defineret.
[^5]: dette betyder at nulvektoren $\vec{0}$ er ortogonal på alting.
[^6]: Vi kan bruge dette ved enhedscirklen ved at definere $||\vec{v}||,||\vec{w}||=1$