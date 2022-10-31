#forelæsning
# Partiel integration/delvis integration

$$\int_{}^{}u(x)v'(x)dx=u(x)v(x)-\int_{}^{}u'(x)v(x)dx$$
## Bevis
Vi vil vise at a$$u(x)v(x)=\int_{}^{}u(x)v'(x)dx+\int_{}^{}u'(x)v(x)dx\Rightarrow \int_{}^{}u(x)v'(x)+u'(x)v(x)dx$$
Dvs uv er en stamfunktion til $uv'+u'v$ altså produktreglen for differentiering: $(uv)'=uv'+u'v$.

# Taylors formel med rentled
Hvis
$$f,f',f'',...,f^{n+1}$$ er kontinuert på [a,b], da vil (1)
$$f(b)=\frac{T_{n}f(b)+1}{n!}\int_{a}^{b}t^{n+1}(t)(b-t)^{n}dt$$
hvor (2)
$$T_{n}f(b)=f(a)+f'(a)(b-a)+\frac{1}{2}f''(a)(b-a)^{2}+ \frac{1}{3!}f^{(3)}(a)(b-a)+...$$
$$+f^{(n)}\frac{f^{(n)}(a)}{n!}(b-a)^{n}$$
antag at vi har vist $(1)_{n}$ altså taylors formel for n. Vi vil vise den for n+1:
Betragt
$$\int_{a}^{b}f^{n+1}(t)(b-t)^{n}dt$$
Her kan vi bruge partiel integration med
	$u(t)=f^{n+1}(t)$
	$v'(t)=(b-t)^{n}$
	 $$v(t)=\int_{}^{}(b-t)^{n} dt=\frac{-1}{n+1}(b-t)^{n+1}$$
	 Nu kan vi indsætte ifølge partiel integration
	 $$\int_{a}^{b}f^{n+1}(t)(b-t)^{n}dt=[f^{n+1}(t)(\frac{-1}{n+1})]-\int_{a}^{b}f^{n+1}(t)(\frac{-1}{n+1})(b-t)^{n+1}dt$$
	 $$\Rightarrow 0-\left(f^{n+1}(a)\left(\frac{-1}{n+1}(b-a)^{n+1}\right)\right)+ \frac{1}{n+1} \int_{a}^{b}f^{n+1}(t)b(-t)^{n+1}dt$$
	 $$\Rightarrow \frac{1}{n+1}f^{n+1}(a)(b-a)^{n+1}+ \frac{1}{n+1}\int_{a}^{b}f^{n+2}(t)(b-t)^{n+1}dt$$
	Indsæt i $(1)_n$ 
	$$=f(a)+f'(a)(b-a)+...+ \frac{f^{n}(a)}{n!}(b-a)^{n}+ \frac{1}{(n+1)!}f^{n+1}(a)(b-a)^{n+1}+ \frac{1}{(n+1)!}\int_{a}^{b}f^{n+2}(t)(b-t)^{n+1}dt$$

# En reel [[Funktioner af flere variable|funktion af flere variable]]
$f:a\rightarrow \mathbb{R}$ , $A=D_{f}$, $A\subseteq \mathbb{R}^{n}$ , Hvis n=2, har vi 2 variable $f(x,y)\in \mathbb{R}$ og hvis det er 3 har vi 3 dimensioner $f(x,y,z)\in \mathbb{R}$.
For funktioner af n=1 variabel der tog vi ofte $D_{f}=[a,b]$ et interval (linje).
For $n>1$ variable vil definitionsmængderne ofte være indviklede, såsom en cirkel med huller, eller $A\subseteq\mathbb{R}^{2}$, $A=\{(x,y)\in\mathbb{R}|x^{2}+y^{2}\leq1\}$.

## Def 1.5 (Niveaukurve)
Vi kan betragte funktioner med flere variabler langs en plan, dette kaldes en niveaukurve:
$f(x,y),n=2$ hvor $N_{c}=\{(x,y)\in{A}|f(x,y)=c \}$ 
$f:A\rightarrow \mathbb{R}, A\subseteq \mathbb{R}^{2}$  for n generelt gælder det at $N_{c}=\{(x_{1},...,x_{n})\in D_{f}|f(x_{1},...,x_{n})=c \}$.

Vi kan betragte funktioner langs linjer$(\vec{x}+r\vec{v})$ ved at fjerne et givent antal variabler. Når vi ser langs linjen kaldes det en "Kontur" for f.
	Her er en kontur for f(x):
	$g(r)=f(x_{1}+rv_{1},...,x_{n}+rv_{n})$ Hvor $x_{n}+rv_{n}$ er en parameterfremstilling for en linje.

  

Niveaukurve