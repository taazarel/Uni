#forelæsning 
Begyndelsesdato: 13:18   06-10-2022   Uge-40
# Grafer
$f(x_{1},x_{2},...,x_{n})$ bliver til en graf $(f)=\{(x_{1},...,x_{n},f(x_{1},...,x_{n}))|(x_{1},...,x_{n}\in D_{f}) \}\subseteq \mathbb{R}^{n+1}$ 

# Niveaumængden
$N_{c}=\{(x_{1},...,x_{n})\in D_{f}|f(x_{1},...,x_{n})=c \} \subseteq \mathbb{R}^{n}$ , hvor $n=2, (x,y)$ niveaukurve, eller $n=3,(x,y,z)$ niveauflade, men de er begge en niveaumængde.

# Funktioner af flere variable til at beskrive geometriske objekter
### Eksempel: Cirkel
![[Repræsentation af funktioner af flere variable 2022-10-06 13.27.08.excalidraw]]
Niveaukurve for $f(x,y)=x^{2}+y^{2}, N_{1}(f)$.

På samme måde er niveaukurven for:
$f(x)=\sqrt{1-x^{2}}$ hvor $y=f(x)$ dvs $x^{2}+y^{2}=1$ er en halvcirkel

# Kordinatsystemer
Disse er smarte da man kan fjerne en variabel ved at vælge det rigtige koordinatsystem.
- Kartetiske: (x,y), (x,y,z)
- Polære koordinater i planen: $(r,\theta)$ 
- Cylinderkoordinater i rummet: $(r,\theta,z)$
- Kuglekoordinater i rummet: $(\rho,\theta,\phi)$  

## Polære koordinater:
$-\infty <x<\infty$ og $-\infty <y<\infty$.
Hvis $r \geq 0$ og $0\leq \theta < 2\pi$.
Så bliver $x=r \cos{\theta}$ og $y=r\sin{\theta}$, hvor $r=\sqrt{x^{2}+y^{2}}$ og $\tan{\theta}=\frac{y}{x}$.

### Eksempel
$f(x,y)=\sin{x^{2}+y^{2}}$
$g(r,\theta)=f(x,y)$
$=f(rcos \theta,rsin \theta)$
$= sin(r^{2}cos^{2}(\theta) + r^{2}sin^{2}(\theta))$  
$=sin(r^{2})$ 

## Cylinderkoordinater
![[Repræsentation af funktioner af flere variable 2022-10-06 13.59.15.excalidraw]]
$f(x,y,z)=g(r,\theta,z)$
$x=rcos \theta$
$y=rsin \theta$
$z=z$

## Kuglekoordinater i rummet
![[Repræsentation af funktioner af flere variable 2022-10-06 14.02.38.excalidraw]]
$f(x,y,z)=g(\rho,\theta,\phi)$
$\rho=\sqrt{x^{2}+y^{2}+z^{2}}$
$0\leq \rho<\infty$
$0\leq \theta<2\pi$
$0\leq \phi<\pi$

$x=\rho sin(\phi)cos(\theta)$
$y=\rho sin(\phi)sin(\theta)$
$z=\rho cos(\phi)$

### Eksempel
$f(x,y,z)=\frac{x^{2}}{z^{2}}+ \frac{y^{2}}{x^{2}}$ 
$$
g(\rho,\theta,\phi)= \frac{\rho^{2}sin^{2}(\phi)cos^{2}\theta}{\rho^{2}cos^{2}(\phi)} + \frac{\rho^{2}sin^{2}(\phi)sin^{2}(\theta)}{\rho^{2}sin^{2}(\phi)cos^{2}(\theta)}
$$
$=tan^{2}(\phi)cos^{2}(\theta)+tan^{2}(\theta)$ 

# Topologiske begreber
$A \in \mathbb{R}^{n}$. ![[Repræsentation af funktioner af flere variable 2022-10-25 08.02.38.excalidraw]]
Hvor randen af $A: \delta A = \delta A$
og punkterne:
- $R \in \delta A, R \notin A$ 
- $S \in \delta A, S \in A$
- $Q,T \notin \delta A, Q,T \notin A$
- $P \in A, P \notin \delta A$ P er et indre punkt
Det indre af $A=A^{o}=A/\delta A$ $=\{\vec{x}\in \vec{A}|\vec{x}\notin \delta A\}$
Afslutningen af $A=\vec{A}=A\cup \delta A= \{\vec{x}\in \mathbb{R}^{n}|\vec{x}\in A$  eller $\vec{x}\in \delta A\}$ 
Husk komplementærmængden $CA=\mathbb{R}^{n}\backslash A=\{\vec{x}\in \mathbb{R}^{n}|\vec{x}\notin A\}$
Bemærk: $\delta A = \delta (CA)$ 


## Definition 2.13 og 2.14[^1]
(Om Åbne mængder og lukkede=afsluttede mængder)
$A \subseteq R^{n}$ kaldes åben hvis den kun har indre punkter, dvs. $A=A/\delta A$ 
$A \subseteq \mathbb{R}^{n}$ kaldes lukket eller afsluttet hvis $A=\vec{A}=A\cup \delta A$.

## Definition (Isoleret punkt)
$\vec{a}\in A$ kaldes isoleret hvis. $\vec{a}\notin \overrightarrow{A/{\vec{a}}}$

## Definition (Fortætningspunkt)
$\vec{a}\in \mathbb{R}^{n}$ er et fortætningspunkt(akkumulationspunkt) hvis $\vec{a}$ ikke er et isoleret punkt for $\vec{A}$.

## Definition (Randpunkt)
$A \subseteq \mathbb{R}^{n}$ da er $\vec{a}\in \mathbb{R}^{n}$ et randpunkt for A hvis der for alle $\delta>0$ gælder at $\{\vec{x}\in \mathbb{R}^{n}|||\vec{x}-\vec{a}||<\delta\}\cap A \neq Ø$ og $\{\vec{x}\in \mathbb{R}^{n}|||\vec{x}-\vec{a}||<\delta\}\cap CA \neq Ø$ 

### Eksempel
$\mathbb{Q} \subset \mathbb{R}$ derfor $\delta \mathbb{Q}=\mathbb{R}$

## Sætning 2.15 (Indre punkter)
Husk de indre punkter i A udgør det indre $A/\delta A$ 
$A \subseteq \mathbb{R}^{n}$, og $\vec{a }\in \mathbb{R}^{n}$ er et indre punkt for A, hvis og kun hvis der findes et $\delta>0$ så $\{\vec{x}\in \mathbb{R}^{n}|||\vec{x}-\vec{a}||<\delta\}\subset A$ 

## Definition 2.16 (Begrænset mængde)
$A \subseteq \mathbb{R}^{n}$ siges at være begrænset hvis der findes et $\mathbb{R}>0$ så $A \subseteq\{\vec{x}\in \mathbb{R}^{n}|||\vec{x}||<\mathbb{R}\}$
Ikke afgørende at kuglen har centrum i $\vec{o}$.



[^1]: De eneste to mængder som er både åbne og lukkede i $\mathbb{R}^{n}$ er Ø tommængden og $\mathbb{R}^{n}$ selv.
