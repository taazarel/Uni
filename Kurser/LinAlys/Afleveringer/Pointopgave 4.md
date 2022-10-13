#aflevering 
#### mws572, Luci Fenger
# 1
Lad $$f(x)=\frac{1}{x}-\frac{\cos{x}}{\sin{x}}$$, for alle $x \in \mathbb{R}$ med $x \neq n \pi, n \in \mathbb{Z}$. 
## a
*Find grænseværdierne $\lim_{x \to 0^{+}}f(x)$, og $\lim_{x \to \pi^{-}}f(x)$ først med og dernæst uden Python (eller tilsvarende).*

$$
\lim_{x \to 0^{+}}f(x)=\frac{1}{x}- \frac{\cos{x}}{\sin{x}}= \frac{\sin{x}-x\cos{x}}{x \sin{x}}= \frac{0}{0}
$$
Vi benytter L'Hôpitals regel.

$$
\begin{array}{c}
g(x)=\sin{x}-x \cos{x} \\
h(x)= \frac{1}{k(x)} \\ 
k(x)=x\sin{x} \\  \\ 
g'(x)=\cos{x}+x \sin{x}-\cos{x} \\ 
h'(x)= \frac{x \cos{x}+\sin{x}}{(x \sin{x})^{2}} \\ 
k'(x)=x \cos{x}+\sin{x} \\ 
\end{array}
$$
$\lim_{x\to0^{+}}f(x)=g'(x)h(x)+g(x)h'(x)$
$=(\cos{x}+x \sin{x}-\cos{x}) \frac{1}{x \sin{x}}+ (\sin{x}-x \cos{x})\frac{x \cos{x}+\sin{x}}{(x \sin{x})^{2}}$
Efter mere beregning af samme slags får vi at grænseværdien er 0 når $x\to0^{+}$.

Nu kan vi finde grænseværdien til den anden grænse,
$$
\lim_{x\to \pi^{-}}h(x)=\frac{1}{x}=\frac{1}{\pi}
$$
$$
lim_{x\to\pi^{-}}g(x)=-\frac{\cos{x}}{\sin{x}}
$$
Da vil $f(x)=h(x)+g(x)$ og vi kan finde grænseværdien således:
$$
\frac{1}{\pi}-\lim_{x \to \pi^{-}}f(x)=- \frac{\cos{\pi}}{\sin{\pi}}= - \frac{1}{0}=\frac{1}{\pi}-(-\infty)=\infty
$$
her vil $\frac{1}{\pi}$ ikke have nogen indflydelse på grænseværdien.
Grænseværdierne er altså, 0 og $\infty$.
## b
*Vis at f er strengt voksende i hvert interval $(n \pi, (n+1)\pi)$. Uligheden $|\sin{x}|<|x|$ for $x \neq0$ kan benyttes uden bevis.*
$$\frac{d}{dx} \frac{1}{x} - \frac{\cos{x}}{\sin{x}}= \frac{d}{dx} \frac{1}{x}- \frac{d}{dx} \frac{\cos{x}}{\sin{x}}$$
Derfor opdeler vi dette i to
$$\frac{d}{dx} \frac{1}{x}=-\frac{1}{x^{2}}$$
$$\frac{d}{dx} \frac{\cos{x}}{\sin{x}}=f(g(x))h(x)$$
Her var - en konstant så vi kan sætte den udenfor.
Hvor $f(x)=\frac{1}{x}$, $g(x)=\sin{x}$ og $h(x)=\cos{x}$.
Så bliver
$$\frac{d}{dx} f(x)=- \frac{1}{\sin^{2}{x}}\cos{x}$$
$$\frac{d}{dx}h(x)=-\sin{x}$$
$$\frac{d}{dx} \frac{\cos{x}}{\sin{x}}=- \frac{1}{\sin^{2}{x}}$$

Så får vi den differentierede funktion:
$$f'(x)=\frac{1}{\sin^{2}{x}} - \frac{1}{x^{2}}$$
Nu kan vi vise at funktionen altid er voksende, da $\frac{1}{\sin^{2}{x}}$ ikke kan blive negativ, og da $|\sin{x}|<|x|$ for $x \neq0$ kan vi se at $f'(x)$ forbliver positiv, da $\frac{1}{sin^{2}x}$ altid vil være større end $\frac{1}{x^{2}}$, givet $x \neq0$, hvilket er tilfældet da vores interval ikke inkluderer 0.

## c
*Bevis at ligningen $f(x)=0$ ikke har nogen løsninger i $(0,\pi)$, og at den har præcis én løsning i $(\pi,2\pi)$. Benyt Python (eller tilsvarende) til at finde en approximation til denne løsning.* 

Som vi så i del a, er grænseværdierne for intervallet $(0,\pi)$ $0^{+}$ og $\infty$. Så vi har altså en funktion som ikke er negativ på noget tidspunkt i dette interval, derfor er det ikke muligt at skære x-aksen, og dermed opfylde kravet $f(x)=0$.

Lad os starte med at finde grænseværdierne til dette interval.
$$\lim_{x\to\pi^{+}}f(x)= \frac{1}{x}- \frac{\cos{x}}{\sin{x}}= \frac{1}{\pi}- \frac{-1}{-0}=-\infty$$
Altså $f(a)<0$,
Herved finder vi
$$\lim_{x\to2\pi^{-}}=\frac{1}{x}- \frac{\cos{x}}{\sin{x}}= \frac{1}{2\pi}- \frac{-1}{0}=\infty$$
Altså $f(b)>0$

I intervallet $(\pi,2\pi)$ har vi altså grænseværdier som er negativ ved $\pi^{+}$ og positiv ved $2\pi^{-}$ derfor kan vi konkludere med hjælp af skæringssætningen at $f(c)=0$ mindst 1 gang i dette interval. 
Fordi funktionen er strengt voksende, MÅ den kun ramme $f(x)=0$, 1 gang. Derfor er der præcis 1 løsning i intervallet $(\pi, 2\pi)$.

# 2
En funktion $f:\mathbb{R}\to \mathbb{R}$ Defineres ved 

$$
f(x)=
\left[
\begin{array}{cc}
\frac{1-x^{2}}{(x-1)(x-3)} & x \in(-\infty;1)U(3;\infty) \\ 
x & x \in [1,3]
\end{array}
\right]
$$
## a
*Benyt Python (eller tilsvarende) til at tegne et udsnit af grafen for f, der giver et retvisende og oplysende billede af funktionens overordnede opførsel.*
![[pointopgave 4 2.2.a.png]]
## b
*Er f differentiabel i $x=1$? Begrund dit svar uden brug af et computerprogram.*

Det ser det ud som på plottet, men vi kan finde ud af det ved at tjekke grænseværdierne af funktionerne i punktet.

$\lim_{x\to1}f(x)=x=1$ og $\lim_{x\to1}f(x)=\frac{1-x^{2}}{(x-1)(x-3)}=\frac{0}{0}$ Så vi bruger altså L'Hôpitals regel.
$$\lim_{x\to1}f(x)=\frac{1-x^{2}}{(x-1)(x-3)}= \frac{0-2x}{(1-0)(x-3)+(x-1)(1-0)}= \frac{-2x}{(x-3)+(x-1)}$$
$$= \frac{-2x}{2x-4}= \frac{-2}{-2}=1$$
Da grænseværdierne for begge funktioner er 1 i $x=1$, og da begge funktioner er kontinuere og differentiable, så må f være differentiabel i $x=1$.

# 3
*Maxwell-Boltzmann fordelingen for en (ædel)gas er sandsynlighedsfordelingen for molekylernes hastighed og er givet ved funktionen
$$
f(v)=4\pi\left(\frac{m}{2\pi kT}\right)^{\frac{3}{2}}v^{2}e^{\frac{-mv^2}{2kT}},
$$
hvor m er gassens molekylmasse, k er Boltzmanns konstant, og T temperaturen og $v \geq0$ er molekylernes fart.
Vi betragter her en heliumsgas og du skal nedenfor bruge værdierne
$$
\left[
\begin{array}{}
m=6,65*10^{-27}kg \\ k=1,38*10^{-23} \frac{m^{2}kg}{s^{2}K} \\ c=3,00*10^{8} \frac{m}{s}
\end{array}
\right]
$$

## a
*Tegn ved brug af Python (eller tilsvarende) hastighedsfordelingen for en heliumsgas ved temperaturene $T=273 K$ og $T=\frac{mc^{2}}{k}$ hvor c er lysets hastighed i vakuum.

 ![[fv1 2.png]]
Her er funktionen $f_{1}(v)$ hvor $T=273K$ hvor x-aksen er hastigheden målt i $\frac{m}{s}$.
![[fv2 1.png]]
Her er funktionen $f_{2}(v)$ hvor $T= \frac{mc^{2}}{k}$, x-aksen er hastigheden. OBS: akserne er skaleret i dette plot.

## b
*Bestem den mest sandsynlige fart $v_{max}$ som funktion af temperaturen T. Brug gerne Python til at checke resultatet, men besvarelsen skal være regnet igennem i hånden.*

$f(v)=C_{1}v^{2}e^{C_{2}v^{2}}$, hvor $C_{1}=4\pi\left(\frac{m}{2\pi kT}\right)^{\frac{3}{2}}$ og $C_{2}=\frac{-m}{2kT}$ 
hvilket vil sige at vi har to funktioner som vi kan differentiere gennem produktreglen.

$h(v)=C_{1}v^{2}$ og $g(v)=e^{k(v)}$ hvor $k(v)=C_{2}v^{2}$

Vi kan finde differentialerne til disse

$\begin{array}{c}h'(v)=2C_{1}v \\ g'(v)=e^{C_{2}v^{2}}2C_{2}v \\ k'(v)=2C_{2}v\end{array}$ 

$f'(v)=h'(x)g(x)+h(x)g'(x)=2C_{1}ve^{C_{2}v^{2}}+ C_{1}v^{2}e^{C_{2}v^{2}}2C_{2}v$

For at finde ekstremum finder vi v når $f'(c)=0$.

$2C_{1}ve^{C_{2}v^{2}}=-C_{1}v^{2}e^{C_{2}v^{2}}2C_{2}v$

$1=- C_{2}v^{2} \Rightarrow v_{max}=\pm\frac{1}{\sqrt{-C_{1}}}$.  

Vi kan her indsætte vores variable konstanter igen.

$$v_{max}=\pm \frac{1}{\sqrt{- \left(\frac{-m}{2kT}\right) }}=\pm \frac{1}{\sqrt{\frac{m}{2kT}}}$$
Her har vi altså $v_{max}$ til T da dette er en variabel. Disse enheder passer, og vi kan tjekke efter ved at indsætte $T=273K$.
$v_{max}(273)=261,869 \frac{m}{s}$ hvilket er realistisk da det er mindre end både lydens og lysets hastighed. 
## c 
*Bestem ligeledes middelfarten givet ved $\int_{0}^{\infty}vf(v)dv$. Du er velkommen til at udregne integraler symbolskt i Python (eller tilsvarende)*

![[pointopgave 4.3.c.png]]
Vi finder middelfarten til at være dette gennem at integrere symbolsk i Python.