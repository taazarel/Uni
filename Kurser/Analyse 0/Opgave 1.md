![[Opgave 1 2023-02-17 13.56.36.excalidraw]]

## Opgave 3.a
$$g(x)=\sinh\frac{x}{e^{x}}= \frac{\frac{e^{x}-e^{-x}}{2}}{e^{x}}\space x \in \mathbb{R}\space x \to \infty$$
$g(x)\to \frac{1}{2}$

$$|g(x)-b|< \epsilon \Rightarrow |\frac{1}{2}- \frac{e^{-x}}{2e^{x}}- \frac{1}{2}|=|- \frac{e^{-x}}{2e^{x}}|=| \frac{1}{2e^{2x}}|< \epsilon $$
$$\Rightarrow 2e^{2x}> \frac{1}{\epsilon } \Rightarrow x > \frac{\log(\frac{1}{2\epsilon })}{2} = K$$
Vælg $K = max \{\frac{\log(\frac{1}{2\epsilon })}{2}, \frac{1}{2} \}$

## Opgave 3.b
$$h(x)= \frac{\tanh(x)-1}{e^{-2x}}\space x \in \mathbb{R}\space x \to \infty $$
$h(x)\to -2$

$$|h(x)-b|=| \frac{-2e^{2x}}{e^{2x}+1}-2|<\epsilon \Rightarrow | \frac{-2e^{2x}+2e^{x}+2}{e^{2x}+1}|=| \frac{2}{e^{2x}+1}|< \epsilon $$
$$\Rightarrow |\frac{e^{2x}+1}{2}|> \frac{1}{\epsilon}\Rightarrow 2x + \log(1)> \log\left(\frac{2}{\epsilon}\right) \Rightarrow x > \frac{\log(\frac{2}{\epsilon})}{2}=K $$
Vælg $K = max \{\frac{\log(\frac{2}{\epsilon})}{2}, 1\}$

## Opgave 3.c
$$k(x)= \frac{1}{x}+ \log\left(\frac{x}{1+x}\right)\space x>0 \space x \to \infty $$
Gæt $k(x)\to 0$
$y = \frac{x}{1+x}$
$$\frac{y-1}{y}\leq \log(y) \text{ for } x \in \mathbb{R}$$
indsæt y
$$\frac{\frac{x}{1+x}-1}{\frac{x}{1+x}} \leq \log\left(\frac{x}{1+x}\right) \Rightarrow 1- \frac{1+x}{x}=1- \frac{1}{x}+1=- \frac{1}{x} \leq \log\left(\frac{x}{1+x}\right)$$
$$|\log\left(\frac{x}{1+x}\right)|\leq \frac{1}{x}$$
$$| \frac{1}{x} + \log\left(\frac{x}{1+x}\right)| \leq \frac{2}{x} < \epsilon \Rightarrow x > \frac{2}{\epsilon }=K$$

Vælg $K = \frac{2}{\epsilon}$.

## Opgave 3.d
Vi har allerede påvist dette i 3.c $$|\log\left(\frac{x}{1+x}\right)|\leq \frac{1}{x}$$
Altså at talværdien af logaritmen altid er mindre end $\frac{1}{x}$, hvilket er den anden del af $k(x)$. Derfor må $k(x)= \frac{1}{x}+ \log(\frac{x}{1+x})$ være positiv for alle $\frac{1}{x}> 0$ hvilket det er når $x >0$. (QED)

## Opgave 1.d
$$\cosh\left(\frac{x+y}{2}\right)= \frac{e^{\frac{x}{2}}e^{\frac{y}{2}}+e^{\frac{-x}{2}}e^{\frac{-y}{2}}}{2}$$
$$\sinh\left(\frac{x-y}{2}\right)= \frac{e^{\frac{x}{2}}e^{\frac{-y}{2}}-e^{\frac{-x}{2}}e^{\frac{y}{2}}}{2}$$
$$2\cosh\left(\frac{x+y}{2}\right)\sinh\left(\frac{x-y}{2}\right)= \frac{e^{x}-e^{y}+e^{-y}-e^{-x}}{2}$$

$$\sinh(x)-\sinh(y) = \frac{e^{x}-e^{-x}}{2} - \frac{e^{y}-e^{-y}}{2}=\frac{e^{x}-e^{y}+e^{-y}-e^{-x}}{2}$$
Begge sider er ens, altså må $\sinh(x)-\sinh(y)=2\cosh\left(\frac{x+y}{2}\right)\sinh\left(\frac{x-y}{2}\right)$.

$$\cosh(x)-\cosh(y)= \frac{e^{x}+e^{-x}}{2}- \frac{e^{y}+e^{-y}}{2} = \frac{e^{x}+e^{-x}-e^{y}-e^{-y}}{2}$$

$$\sinh\left(\frac{x+y}{2}\right)= \frac{e^{\frac{x}{2}}e^{\frac{y}{2}}-e^{\frac{-x}{2}}e^{\frac{-y}{2}}}{2}$$

$$2\sinh\left(\frac{x+y}{2}\right)\sinh\left(\frac{x-y}{2}\right)= \frac{e^{x}-e^{y}-e^{-y}+e^{x}}{2}$$
Er det samme på begge sider, derfor er $\cosh(x)-\cosh(y)=2\sinh\left(\frac{x+y}{2}\right)\sinh(\frac{x-y}{2})$

For $0 \leq x < y$ 
$$\cosh(y)-\cosh(x) = \frac{e^{y}+e^{-y}-e^{x}-e^{-x}}{2}= \frac{e^{y}-e^{x}}{2} + \frac{e^{-y}-e^{-x}}{2}$$
$$e^{y}-e^{x}\geq 1+y-1-x = y-x > 0 \Rightarrow y >x$$
$$e^{-y}-e^{-x}= \frac{1}{e^{y}-e^{x}}\geq 1-y - 1+x = x-y<0 \Rightarrow -y<-x$$
Begge sider er negative, lad os tage talværdien.
$$\Rightarrow | \frac{1}{e^{y}-e^{x}}|\leq |x-y|=|y-x| \leq |e^{y}-e^{x}|$$
Herved har vi bevist at $\cosh$ er strengt voksende for $[0, \infty )$.

$y<x \leq 0 \Rightarrow 0 \leq -x < -y$.
$$\cosh(x)=\cosh(-x)<\cosh(-y)=\cosh(y)$$
Altså er $\cosh$ strengt aftagende på $(-\infty, 0]$

Lad $x < y$. $\sinh(y)-\sinh(x)= \frac{e^{y}-e^{x}}{2}+ \frac{e^{-x}-e^{-y}}{2}$
$e^{y}-e^{x}>0$ da exp er en strengt voksende funktion.
Den venstre del er også positiv da $x < y \Rightarrow -x > -y$. Derfor vil $e^{-x}-e^{-y}>0$ da exp er strengt voksende.

Fordi begge sider er positive er $\sinh(y)-\sinh(x)>0$ for alle $x, y \in \mathbb{R}$ som opfylder $x < y$.

# Opgave 1.b

$\cosh(x)\geq 1$ for alle $x \in \mathbb{R}$.
Ved punkterne hvor $x \neq 0$ er $\cosh(x)> 1$. $\cosh(x)= \frac{1}{2}(e^{x}+e^{-x})\geq \frac{1}{2}(1+x+1-x)= 1$. Uligheden finder vi gennem (A.34) og (A.35).
Det eneste tidspunkt at $e^{x}=e^{-x}$ er ved $x=0$. ved dette punkt bliver $\cosh(0)= \frac{1}{2}(e^{x}+e^{-x})= \frac{1}{2}(1+1)=1$.
Så vi kan se at $\cosh(x)\geq 1$ for alle $x \in \mathbb{R}$.

$$\sinh(x)= \frac{1}{2}(e^{x}-e^{-x})$$
Hvis $x < 0$ så er $e^{x}-e^{-x}<0$ da exp er strengt voksende (Side 458). Vi kunne skrive $y = -x$ og $e^{y}-e^{-y} = e^{-x}-e^{x}<0$ hvilket er sandt da $-x < x$. Her er y blot en måde at vise at x er negativ.
Hvis $x >0$ så er $e^{x}-e^{-x}<0$, da vi ved at exp er voksende, og $-x <x$.
Det eneste sted at $\sinh(x)=0$ er når $e^{x}=e^{-x}$. Derfor må dette være i $x=0$. Vi prøver $\sinh(0)=\frac{1}{2}(e^{0}-e^{0})=0$.

Vi har herved bevist at $\sinh(x) < 0$ ved $x <0$, $\sinh(x) >0$ ved $x >0$ og $\sinh(x)=0$ når $x=0$. 

# Opgave 2
$$|f(x)-1|=|\sqrt{1+x}-1|=| \frac{\sqrt{1+x}-1}{\sqrt{1+x}+1}(\sqrt{1+x}+1)| = | \frac{x}{\sqrt{1+x}+1}|$$
Fordi at nævneren altid vil være større end eller lig med 1, da kvadratroden ikke kan blive negativ, og der står +1, så vil følgende være sandt:
$$| \frac{x}{\sqrt{1+x}+1}| \leq |x| = |x-0| < \epsilon = \delta $$
Altså kan vi vælge $\delta = \epsilon$ for $x \in [-1,\infty)$.