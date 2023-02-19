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
