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
c^2 = a^2 + b^2 - 2ab\cos(\gamma)
$$

![[svgviewer-png-output.png|305]]

**Demostración:** dado un triangulo $ABC$ con lados $a$, $b$, $c$ y ángulos internos opuestos $\alpha$, $\beta$, $\gamma$.
- Caso 1: triángulo acutángulo

![[tdc1.png|438]]

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


- Caso 2: triángulo obtusángulo

![[tdc2.png|509]]

El teorema de Pitágoras establece nuevamente
$$c^2=h^2+u^2\to h^2=c^2-u^2\tag{1}$$
Pero en este caso
$$
\begin{align}
b^2&=h^2+(a+u)^2 \\
b^2-(a+u)^2&=h^2\tag{2}
\end{align}
$$
E igualando $(1)$ y $(2)$:
$$
\begin{align}
c^2-u^2&=b^2-(a+u)^2 \\
c^2-u^2&=b^2-(a^2+2au+u^2) \\
c^2\cancel{-u^2}&=b^2-a^2-2au\cancel{-u^2}
\end{align}
$$
$$\boxed{c^2=b^2-a^2-2au} \tag{3}$$
Por otro lado, por definición de coseno, se tiene:
$$
\begin{align}
\cos(\gamma)&=\frac{a+u}{b} \\
b\cos(\gamma)&=a+u \\
\end{align}
$$
$$\boxed{u=b\cos(\gamma)-a}$$
Ahora sustituyo $(4)$ en $(3)$ y obtengo:
$$
\begin{align}
c^2&=b^2-a^2-2a(b\cos(\gamma)-a) \\
c^2&=b^2-a^2-2ab\cos(\gamma)+2a^2
\end{align}
$$
$$\boxed{c^2=a^2+b^2-2ab\cos(\gamma)}$$
Q.E.D.

---

## Unicidad de la inversa de una matriz
**Enunciado:** si una matriz $A$ es invertible, entonces su inversa es única.
**Demostración:** supongamos que $B$ y $C$ son inversas de $A$. Por definición se tiene:
$$AB=BA=I,\quad\text{y} \quad AC=CA=I$$
Por la ley asociativa de la multiplicación de matrices se tiene que:
$$B(AC)=(BA)C$$
Entonces
$$B=BI=B(AC)=(BA)C=IC=C$$
Por lo tanto $B=C$. Q.E.D.

---

## Inversa del producto
**Enunciado:** si $A$ y $B$ dos matrices invertibles de $n\times n$ entonces $AB$ es invertible y
$$(AB)^{-1}=B^{-1}A^{-1}$$
**Demostración:** $B^{-1}A^{-1}=(AB)^{-1}$ si y sólo si 
$$(B^{-1}A^{-1})(AB)=(AB)(B^{-1}A^{-1})=I$$
Verifico que es inversa de $AB$:
$$(B^{-1}A^{-1})(AB)=B^{-1}(A^{-1}A)B=B^{-1}IB=B^{-1}B=I$$
y
$$(AB)(B^{-1}A^{-1})=A(BB^{-1})A^{-1}=AIA^{-1}=AA^{-1}=I$$
Entonces $B^{-1}A^{-1}$ es inversa de $AB$.

---

## Teorema de Rouché–Frobenius
**Enunciado:** sea el sistema lineal $Ax=H$, con matriz de coeficientes $A$ y matriz ampliada $(A\mid H)$. Entonces el sistema tiene solución si y sólo si 
$$\operatorname{rg}(A)=\operatorname{rg}(A\mid H)$$
Además, si $n$ es el número de incógnitas, entonces:
- si $\operatorname{rg}(A)=\operatorname{rg}(A\mid H)=n$, la solución es única (compatible determinado).
- si $\operatorname{rg}(A)=\operatorname{rg}(A\mid H)<n$, hay infinitas soluciones (compatible indeterminado).
- si $\operatorname{rg}(A)\neq \operatorname{rg}(A\mid H)$, el sistema no tiene soluciones (incompatible).

**Demostración:** sea $Ax=H$ un sistema lineal y consideremos su matriz ampliada $(A\mid H)$. Mediante operaciones elementales por fila podemos llevar $(A\mid H)$ a forma escalonada reducida. Estas operaciones elementales por filas no modifican el conjunto de soluciones ni los rangos de las matrices porque transforman el sistema en otro equivalente, y cada una es reversible.

En una matriz escalonada, el rango equivale a la cantidad de filas no nulas. Al comparar los rangos, tenemos dos escenarios:
1. Si $\operatorname{rg}(A)\neq \operatorname{rg}(A\mid H)$, entonces la única forma de que los rangos difieran es que exista una fila en la matriz escalonada de la forma $\left[\begin{array}{ccc|c} 0 & \cdots & 0 & k \end{array}\right]$ con $k\neq 0$, que representa la ecuación $0=k$, lo cual es un absurdo. Por lo tanto, el sistema no tiene solución.
2. En cambio, si $\operatorname{rg}(A)=\operatorname{rg}(A\mid H)$, no aparece ninguna contradicción y el sistema es compatible.
