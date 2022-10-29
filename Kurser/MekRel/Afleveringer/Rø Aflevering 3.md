# 1
**Notat: Jeg bruger $x^{´}$ som prikker, det er det nærmeste jeg kan komme i $\LaTeX$**

Vi har den totale længde af snoren som $l=a(t)+b(t)+d(t)$
Dette kan differentieres i forhold til tiden.$0=a^´(t)+b^{´}(t)+d^{´}(t)$.
Her kan vi isolere $a^{´}(t)=-(b^{´}(t)+d^{´}(t))$ og differentiere igen til at finde det geometriske bånd:
$$\ddot a(t)=-\ddot b(t)-\ddot d(t)$$
(**Note: fandt ud af hvordan man skrev prikker, bruger det fra nu af**)
# 2
Den kinetiske energi er givet ved: $$K=\frac{1}{2}m_{1}v^{2}_{1}+ \frac{1}{2}m_{2}v_{2}^{2}\Rightarrow \frac{1}{2}m_{b}(-\dot a(t)-\dot d(t))^{2}+ \frac{1}{2}M_{a}(\dot a(t))^{2}$$
# 3
Den potentiale energi er givet ved: $$U=m_{1}gh_{1}+m_{2}gh_{2}\Rightarrow m_{b}g(h-b(t))+M_{a}g(h-a(t))\Rightarrow m_{b}g(h-(l-a(t)-d(t)) +M_{a}g(h-a(t))$$
$$\Rightarrow U=m_{b}g(h+a(t)+d(t)-l)+M_{a}g(h-a(t))$$
Dette er altså den potientielle energi af hele systemet.
Vi kan se her at $U(t)$ hvilket betyder at vi ikke har impulsbevarelse.

# 4
3. $L=\frac{1}{2}m_{b}(-\dot a(t)-\dot d(t))^{2}+ \frac{1}{2}M_{a}(\dot a(t))^{2}-m_{b}g(h+a(t)+d(t)-l)+M_{a}g(h-a(t))$
4. $$\frac{dU}{dx}=m_{b}g \delta a(t)+m_{b}g \delta d(t) -M_{a}g \delta a(t)\Rightarrow 2m_{b}g-M_{a}g$$
5. $$\frac{dK}{d \dot x}=-m_{b}\dot a-m_{b}\dot d+M_{a}\dot a$$
6. $$\frac{d}{dt}\left(\frac{dK}{d \dot x}\right)=M_{a}\ddot a-m_{b}\ddot a-m_{b}\ddot d$$
7. $$\frac{d}{dt}\left(\frac{dK}{d \dot x}\right)=\frac{dU}{dx}\Rightarrow M_{a}\ddot a-m_{b}\ddot a-m_{b}\ddot d=2m_{b}g-M_{a}g$$
Nu kan vi finde:$$(M_{a}-m_{b})\ddot a-m_{b}\ddot d=2m_{b}g-M_{a}g \Rightarrow \ddot a=\frac{2m_{b}g-M_{a}g+m_{b}\ddot d}{M_{a}-m_{b}}$$
Her har vi et udtryk for $\ddot a$ som er beskrevet kun ved funktioner af $m_{b}\text{ og }M_{a}$.
# 5
Hvis $\dot d=0$ så bliver $$\ddot a= \frac{2m_{b}g-M_{a}g}{M_{a}-m_{b}} \Rightarrow g 2$$

