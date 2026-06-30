### Funciones
#### Transformaciones
**Desplazamiento vertical y horizontal ($c>0$):**
- $y=f(x)\pm c$ : **desplaza verticalmente** $c$ unidades hacia arriba/abajo la gráfica.
- $y=f(x+c)$ : **desplaza horizontalmente** $c$ unidades a la derecha/izquierda la gráfica.

![[Captura de pantalla 2026-06-29 a la(s) 6.23.20 p. m..png|408]]

**Alargamientos($c>1$):**
- $y=cf(x)$ : **alarga verticalmente** la gráfica por un factor de $c$.
- $y=f(cx)$ : **comprime horizontalmente** la gráfica por un factor de c.

**Reflexiones vertical y horizontal ($c>1$):**
- $y=-f(x)$ : **refleja** la gráfica sobre el eje $x$.
- $y=f(-x)$ : **refleja** la gráfica sobre el eje $y$.

![[Captura de pantalla 2026-06-29 a la(s) 6.42.47 p. m..png|400]]

#### Inyectividad
Una función se dice inyectiva si nunca toma el mismo valor dos veces:
$$f(x_{1})=f(x_{2})\implies x_{1}=x_{2}$$

#### Sobreyectividad
Una función sobreyectiva es una función cuya imagen es igual a su codominio.

#### Biyectividad
Una función es biyectiva si es a la vez inyectiva y sobreyectiva.

---
### Límite
#### Entorno reducido
Es el conjunto de puntos del intervalo abierto $(a-\delta,a+\delta)$ del cual se **excluye** el punto $a$ (el centro).

#### Punto de acumulación
Si $S$ es un conjunto de puntos de la recta real, un punto $a$ es de acumulación si y sólo si a todo entorno reducido de centro $a$ pertenece por lo menos un elemento de $S$ (el entorno reducido debe tener un elemento que sea de $S$).


$$\lim_{ x \to c } f(x)=L$$
si para todo número $\varepsilon>0$ existe un $\delta > 0$ tal que, si
$$0<|x-a|<\delta$$
entonces
$$|f(x)-L|<\varepsilon$$
![[Pasted image 20260629195401.png|393]]
La condición $0<|x-a|<\delta$ (notación de entorno reducido de centro en $a$ y radio $\delta$) significa que $x$ está a distancia menor que $\delta$ de $a$, pero distinto de $a$ ($x$ se acerca a $a$, pero no lo toca).
$a$ **debe ser un punto de acumulación**, si no lo fuera, no habría puntos del dominio arbitrariamente cerca de $a$, y entonces no podrías "acercarte" a $a$.

#### Indeterminación
Se entiende por **indeterminación de un límite** una forma algebraica que, por sí sola, **no permite saber cuál es el valor del límite**. No quiere decir automáticamente que el límite no exista; quiere decir que hay que **transformar la expresión** para poder decidirlo.