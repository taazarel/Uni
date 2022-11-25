# 8.1
$$\left[
\begin{array}{ccc|c}
i & (1+i) &   & 1+3i \\ 
1 & (1-i) & 1 & 2-i \\ 
  & (3+i) & 1 & 5
\end{array}
\right] $$


# 8.2
## a
For en matrix $X=[x_{ij}]\in \mathbb{M}_{2,2}$ definerer vi $\langle A,B \rangle=Tr(A^{t}B)$.

$$\left[
\begin{array}{cc}
1 & 2 \\ 0 & 7
\end{array}
\right]
\left[
\begin{array}{cc}
3 & 4 \\ 0 & 5
\end{array}
\right] =\left[
\begin{array}{cc}
3 & 14 \\ 0 & 35
\end{array}
\right] $$
Vi finder sporet til denne matrice
$$Tr(A^{t}B)=Tr\left[
\begin{array}{cc}
3 & 14 \\ 0 & 35
\end{array}
\right] =3+35=38$$

## b
Vis at $\langle , \rangle$ opfylder aksiom 1 for indre produkt [Messer Definition 4.1]
$$\langle \left[
\begin{array}{cc}
0 & 0  \\ 0 & 0
\end{array}
\right],\left[
\begin{array}{cc}0 & 0 \\  0 & 0
\end{array}
\right]  \rangle=0+0=0$$
$$\langle \left[
\begin{array}{cc}
-1 & 2 \\ 3 & -4
\end{array}
\right],\left[
\begin{array}{cc}
-1 & 2 \\ 3 & -4
\end{array}
\right] \rangle = Tr(\left[
\begin{array}{cc}
-1 & 3 \\ 2 & -4
\end{array}
\right]\left[
\begin{array}{cc}
-1 & 2 \\ 3 & -4
\end{array}
\right])$$
$$= Tr(\left[
\begin{array}{cc}10 & -14 \\ -14 & 20
\end{array}
\right])=30$$
Dette vil altså altid blive positivt da $x_{11},x_{22}$ altid vil stå i anden, og derfor blive positive. Det indre produkt bliver altid $\langle A,A \rangle \geq 0$ og når $\langle A,A \rangle =0$ så er $$A=\left[
\begin{array}{cc}0 & 0 \\ 0 & 0
\end{array}
\right] $$
Derfor opfylder operationen aksiom 1.
## c
$$||U_{2}||=\left[
\begin{array}{cc}1 & 0 \\ 1 & 0
\end{array}
\right] \left[
\begin{array}{cc}1 & 1  \\ 0 & 0
\end{array}
\right] =\left[
\begin{array}{cc} 1 & 1 \\ 1 & 1
\end{array}
\right] =\sqrt{2}$$
$$||U_{3}||=\left[
\begin{array}{cc}0 & 0 \\ 1 & 1
\end{array}
\right] \left[
\begin{array}{cc}0 & 1 \\ 0 & 1
\end{array}
\right] =\left[
\begin{array}{cc}0 & 0 \\ 0 & 2
\end{array}
\right] = \sqrt{2}$$
$$||U_{1}||=\sqrt{Tr\left(\left[
\begin{array}{cc}1 & 1 \\ 0 & 0
\end{array}
\right]\left[
\begin{array}{cc}1 & 0  \\ 1 & 0
\end{array}
\right]\right)} =\sqrt{Tr\left[
\begin{array}{cc}2 & 0 \\ 0 & 0
\end{array}
\right]}=\sqrt{2}$$
$$E_{1}=\frac{1}{\sqrt{2}}\left[
\begin{array}{cc}1 & 0 \\ 1 & 0
\end{array}
\right] =\left[
\begin{array}{cc} \frac{1}{\sqrt{2}} & 0 \\ 
\frac{1}{\sqrt{2}} & 0 
\end{array}
\right] $$
$$V_{2}=U_{2}-\langle U_{2},E_{1}\rangle E_{1}$$
$$\langle U_{2},E_{1}\rangle=Tr\left(\left[
\begin{array}{cc}
1 & 0 \\ 
1 & 0
\end{array}
\right]\left[
\begin{array}{cc} 
\frac{1}{\sqrt{2}} & 0 \\ 
\frac{1}{\sqrt{2}} & 0
\end{array}
\right] \right)=Tr\left(\left[
\begin{array}{cc}
\frac{1}{\sqrt{2}} & 0 \\ 
\frac{1}{\sqrt{2}} & 0
\end{array}
\right]\right)= \frac{1}{\sqrt{2}}$$
$$\frac{1}{\sqrt{2}}\left[
\begin{array}{cc}
\frac{1}{\sqrt{2}} & 0 \\ 
\frac{1}{\sqrt{2}} & 0
\end{array}
\right] =\left[
\begin{array}{cc}
\frac{1}{2} & 0 \\ \frac{1}{2} & 0
\end{array}
\right] $$
$$V_{2}=\left[
\begin{array}{cc}
1 & 1  \\  0 & 0
\end{array}
\right]-\left[
\begin{array}{cc}
\frac{1}{2} & 0  \\ \frac{1}{2} & 0
\end{array}
\right]  =\left[
\begin{array}{cc}
\frac{1}{2} & 1 \\ \frac{-1}{2} & 0
\end{array}
\right] $$
$$||V_{2}||=\sqrt{Tr\left(\left[
\begin{array}{cc}
\frac{1}{2} & \frac{-1}{2} \\ 1 & 0
\end{array}
\right]\left[
\begin{array}{cc}
\frac{1}{2} & 1 \\ \frac{-1}{2} & 0
\end{array}
\right]\right)}=\sqrt{Tr\left(\left[
\begin{array}{cc}
\frac{1}{2} & \frac{1}{2} \\ \frac{1}{2} & 1
\end{array}
\right]\right)}=\sqrt{\frac{3}{2}} $$
$$E_{2}= \frac{1}{\sqrt{\frac{3}{2}}}\left[
\begin{array}{cc}
\frac{1}{2} & 1 \\ \frac{-1}{2} & 0
\end{array}
\right] =\left[
\begin{array}{cc}
\frac{1}{2\sqrt{\frac{3}{2}}} &  
\frac{1}{\sqrt{\frac{3}{2}}} \\ 
\frac{-1}{2\sqrt{\frac{3}{2}}} & 0
\end{array}
\right]$$
$$V_{3}=U_{3}-\langle U_{3},E_{1}\rangle E_{1}-\langle U_{3},E_{2}\rangle E_{2}$$
$$\langle U_{3},E_{1}\rangle =Tr\left(\left[
\begin{array}{cc}
0 & 0 \\ 
1 & 1
\end{array}
\right]
\left[
\begin{array}{cc}
\frac{1}{\sqrt{2}} & 0 \\ 
\frac{1}{\sqrt{2}} & 0
\end{array}
\right] \right)=Tr\left(\left[
\begin{array}{cc}
0 & 0 \\ 
\frac{2}{\sqrt{2}} & 0
\end{array}
\right] \right)= 0$$
$$E_{1}\langle U_{3},E_{1}\rangle= \left[
\begin{array}{cc}
0 & 0  \\ 
0 & 0
\end{array}
\right] $$
$$\langle U_{3},E_{2}\rangle =Tr\left(\left[
\begin{array}{cc}
0 & 0 \\ 
1 & 1
\end{array}
\right] 
\left[
\begin{array}{cc}
\frac{1}{2\sqrt{\frac{3}{2}}} &  
\frac{1}{\sqrt{\frac{3}{2}}} \\ 
\frac{-1}{2\sqrt{\frac{3}{2}}} & 0
\end{array}
\right] \right)=Tr\left(\left[
\begin{array}{cc}
0 & 0 \\ 
0 & \frac{1}{\sqrt{\frac{3}{2}}}
\end{array}
\right] \right)= \frac{1}{\sqrt{\frac{3}{2}}}$$
$$\langle U_{3},E_{2}\rangle E_{2}= \frac{1}{\sqrt{\frac{3}{2}}}\left[
\begin{array}{cc}
\frac{1}{2\sqrt{\frac{3}{2}}} &  
\frac{1}{\sqrt{\frac{3}{2}}} \\ 
\frac{-1}{2\sqrt{\frac{3}{2}}} & 0
\end{array}
\right] =\left[
\begin{array}{cc}
\frac{1}{3} & \frac{2}{3} \\ 
\frac{-1}{3} & 0
\end{array}
\right]$$
$$V_{3}=\left[
\begin{array}{cc}
0 & 1 \\ 
0 & 1
\end{array}
\right] -\left[
\begin{array}{cc}
0 & 0  \\ 0 & 0
\end{array}
\right] 
-\left[
\begin{array}{cc}
\frac{1}{3} & \frac{2}{3} \\ 
\frac{-1}{3} & 0
\end{array}
\right]=\left[
\begin{array}{cc}
\frac{-1}{3} & \frac{1}{3} \\ 
\frac{1}{3} & 1
\end{array}
\right]  $$
$$||V_{3}||=\sqrt{Tr\left(\right)}$$

# 8.3
## a

## b
