#kapitel 
Vi kender alle definitionen for gennemsnittet, men der er også andre måder at estimere en mest "Typisk værdi". Vi har... :: Medianen, Typetallet (Det tal som fremgår mest) og den geometriske middelværdi $G(x)=(x_{1}x_{2}...x_{N})^{\frac{1}{N}}\Rightarrow log (G(x))= \frac{1}{N} \sum^{N}_{j=1}log(x_{j})-log(\vec{x})$
<!--SR:!2023-02-23,4,272-->
Varians bliver beskrevet som hvor sandsynligt det er for et datapunkt at afvige fra middelværdien. Vi definerer varians som... :: $V(x)= \frac{1}{N} \sum_{j=1}^{N}(x_{j}-\vec{x})^{2}$ (2.5)
<!--SR:!2023-02-23,4,272-->
Standardafvigelsen/spredningen er... :: kvadratroden af varians $\sigma =\sqrt{V(x)}= \sqrt{\frac{1}{N} \sum_{j=1}^{N}(x_{j}-\vec{x})^{2}}$[^1]
<!--SR:!2023-02-23,4,272-->
Covarians er sammenhæng mellem data, om de er afhængige eller uafhængige af hinanden. Vi bruger dette meget ofte i fysik og definerer... :: $$cov(x,y)=\frac{1}{N} \sum_{i}(x_{i}-\vec{x})(y_{i}-\vec{y})$$
<!--SR:!2023-02-23,4,272-->
Correlation er endnu bedre end covariansen til at bestemme sammenhæng mellem datapunkter. Vi skriver correlation som... :: $\rho(x,y)= \frac{cov(x,y)}{\sigma_{x}\sigma_{y}}$[^2]
<!--SR:!2023-02-18,4,270-->



[^1]: Antallet af punkter som er indenfor spredningen er ca 68% $P(|\vec{x}-x_{j}|<\sigma )=0.68$
[^2]: Dette giver et tal mellem 1 og -1.