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
Dette er det samme som før, så denne er bevist.

$$\cosh(x)-\cosh(y)= \frac{e^{x}+e^{-x}}{2}- \frac{e^{y}+e^{-y}}{2} = \frac{e^{x}+e^{-x}-e^{y}-e^{-y}}{2}$$

$$\sinh\left(\frac{x+y}{2}\right)= \frac{e^{\frac{x}{2}}e^{\frac{y}{2}}-e^{\frac{-x}{2}}e^{\frac{-y}{2}}}{2}$$

$$2\sinh\left(\frac{x+y}{2}\right)\sinh\left(\frac{x-y}{2}\right)= \frac{e^{x}-e^{y}-e^{-y}+e^{x}}{2}$$
Er det samme som før, så den anden formel er også bevist.

For $0 \leq x < y$ gælder det at $$\cosh(y)-\cosh(x)= \frac{e^{y}+e^{-y}-e^{x}-e^{-x}}{2}\Rightarrow \frac{e^{y}-e^{x}}{2} +\frac{e^{-y}-e^{-x}}{2}$$
$$$$