## Teorema del seno
**Enunciado:** dado un triángulo $ABC$ cualquiera, siendo $\alpha$, $\beta$, $\gamma$ los ángulos, y $a$, $b$, $c$ los lados respectivamente opuestos a estos ángulos entonces:
$$\frac{a}{\sin(\alpha)} =\frac{b}{\sin(\beta)} =\frac{c}{\sin(\gamma)}$$
![[Ley_de_los_senos.svg|292]]


**Demostración:** dado un triangulo $ABC$ con lados $a$, $b$, $c$ y ángulos internos opuestos $\alpha$, $\beta$, $\gamma$, trazo dos alturas: $h_{b}$ desde el vértice $B$ hasta el lado opuesto $b$ y $h_{c}$ desde el vértice $C$ hasta el lado opuesto $c$. De esta forma divido al triángulo principal en dos triángulos rectángulos más pequeños.

![[tds.png|440]]

- Con $h_{b}$ obtengo: 
$$
\begin{gather}
\sin(\alpha)=\frac{h_{b}}{c}\to \sin(\alpha)\cdot c=h_{b} \\
\sin(\gamma)=\frac{h_{b}}{a}\to \sin(\gamma)\cdot a=h_{b}
\end{gather}
$$
Entonces,
$$
\begin{gather}
\sin(\alpha)\cdot c=\sin(\gamma)\cdot a \\
\boxed{\frac{a}{\sin(\alpha)}=\frac{c}{\sin(\gamma)}}
\end{gather}
$$
- Con $h_{c}$ obtengo:
$$
\begin{gather}
\sin(\beta)=\frac{h_{c}}{a}\to \sin(\beta)\cdot a=h_{c} \\
\sin(\alpha)=\frac{h_{c}}{b}\to \sin(\alpha)\cdot b=h_{c}
\end{gather}
$$
Entonces,
$$
\begin{gather}
\sin(\beta)\cdot a=\sin(\alpha)\cdot b \\
\boxed{\frac{a}{\sin(\alpha)}=\frac{b}{\sin(\beta)}}
\end{gather}
$$
Es decir,
$$
\boxed{\frac{a}{\sin(\alpha)} =\frac{b}{\sin(\beta)} =\frac{c}{\sin(\gamma)}}
$$
Q.E.D.

---
## Teorema del coseno
**Enunciado:** dado un triángulo $ABC$ cualquiera, siendo $\alpha$, $\beta$, $\gamma$ los ángulos, y $a$, $b$, $c$ los lados respectivamente opuestos a estos ángulos entonces:
$$
\begin{align}
a^2 &= b^2 + c^2 - 2bc\cos(\alpha) \\
b^2 &= a^2 + c^2 - 2ac\cos(\beta) \\
c^2 &= a^2 + b^2 - 2ab\cos(\gamma)
\end{align}
$$

![[svgviewer-png-output.png|305]]

**Demostración:** dado un triangulo $ABC$ con lados $a$, $b$, $c$ y ángulos internos opuestos $\alpha$, $\beta$, $\gamma$.
- Caso 1: triángulo acutángulo
Por el teorema de Pitágoras, la longitud $c$ es calculada así:
$$c^2=h^2+u^2\to h^2=c^2-u^2\tag{1}$$
Pero, la longitud $h$ también se calcula así:
$$
\begin{align}
b^2&=h^2+(a-u)^2 \\
b^2-(a-u)^2&=h^2\tag{2}
\end{align}
$$
E igualando $(1)$ y $(2)$:
$$
\begin{align}
c^2-u^2&=b^2-(a-u)^2 \\
c^2-u^2&=b^2-(a^2-2au+u^2) \\
c^2\cancel{-u^2}&=b^2-a^2+2au\cancel{-u^2}
\end{align}
$$
$$\boxed{c^2=b^2-a^2+2au}\tag{3}$$
Por otro lado, por definición de coseno, se tiene:
$$
\begin{align}
\cos(\gamma)&=\frac{a-u}{b} \\
b\cos(\gamma)&=a-u \\
-a+b\cos(\gamma)&=-u \\
\end{align}
$$
$$\boxed{u=a-b\cos(\gamma)}\tag{4}$$
Ahora sustituyo $(4)$ en $(3)$ y obtengo:
$$
\begin{align}
c^2&=b^2-a^2+2a(a-b\cos(\gamma)) \\
c^2&=b^2-a^2+2a^2-2ab\cos(\gamma) \\
\end{align}
$$
$$\boxed{c^2=a^2+b^2-2ab\cos(\gamma)}$$
Q.E.D.


---

## Teorema de Rouché–Frobenius
## Unicidad de la inversa de una matriz