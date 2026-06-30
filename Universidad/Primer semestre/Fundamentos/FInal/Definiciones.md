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
#### Definición formal de límite
$$\lim_{ x \to c } f(x)=L$$
si para todo número $\varepsilon>0$ existe un $\delta > 0$ tal que, si
$$0<|x-a|<\delta$$
entonces
$$|f(x)-L|<\varepsilon$$
![[Pasted image 20260629195401.png|393]]
- La condición $0<|x-a|<\delta$ (notación de entorno reducido de centro en $a$ y radio $\delta$) significa que $x$ está a distancia menor que $\delta$ de $a$, pero distinto de $a$ ($x$ se acerca a $a$, pero no lo toca).
- $a$ **debe ser un punto de acumulación**, si no lo fuera, no habría puntos del dominio arbitrariamente cerca de $a$, y entonces no podrías "acercarte" a $a$.
#### Indeterminación
Se entiende por **indeterminación de un límite** una forma algebraica que, por sí sola, **no permite saber cuál es el valor del límite**. No quiere decir automáticamente que el límite no exista; quiere decir que hay que **transformar la expresión** para poder decidirlo.
#### Límites notables
**Trigonométricos:**
$$
\begin{gather}
\lim_{ x \to 0 } \frac{\sin(x)}{x}=1 \\
\lim_{ x \to 0 } \frac{\tan(x)}{x}=1
\end{gather}
$$

**Exponenciales:**
$$
\begin{gather}
\lim_{ x \to \infty } \left( 1+\frac{1}{x} \right)^x=e \\
\lim_{ x \to 0 } (1+x)^{\frac{1}{x}}=e
\end{gather}
$$

---

### Continuidad
#### Definición
Una función $f$ es continua en un punto $a$ perteneciente a su dominio si y sólo si:
1. $\exists f(a)$
2. $\exists \lim_{ x \to a }f(x)$
3. $\lim_{ x \to a }f(x)=f(a)$
#### Clasificación
$$
   \mathrm{Funci \acute{o} n}
   \left \{
      \begin{array}{l}
         \mathrm{continua}
         \\
         \\
         \mathrm{discontinua}
         \left \{
            \begin{array}{l}
               \mathrm{evitable} \\
               \mathrm{inevitable}
               \left \{
                  \begin{array}{l}
                     \mathrm{de \; 1^a \; especie}
                     \left \{
                        \begin{array}{l}
                           \mathrm{de \; salto \; finito} \\
                           \mathrm{de \; salto \; infinito} \\
                        \end{array}
                     \right .
                     \\
                     \mathrm{de \; 2^a \; especie}
                  \end{array}
               \right .
               \\
            \end{array}
         \right .
      \end{array}
   \right .
$$

---

### Derivada
#### Recta tangente
La tangente a una curva en un punto $P(a,f(a))$ es una recta que toca a la curva solo en dicho punto con pendiente
$$m=\lim_{ x \to a } \frac{f(x)-f(a)}{x-a}$$
Si $h=x-a$, en este caso $x=a+h$. Y si $x\to a$, $h\to a-a$, es decir, $h\to 0$, entonces
$$m=\lim_{ h \to 0 } \frac{f(a+h)-f(a)}{h}$$
#### Derivada
La derivada de una función $f$ en un número $x=a$, denotada por $f '(a)$, es
$$f'(a)=\lim_{ h \to 0 } \frac{f(a+h)-f(a)}{h}$$

---

### Aplicaciones de la derivada
#### Máximo/mínimo global
Sea $c$ un número en el dominio $D$ de una función $f$. Entonces $f(c)$ es el 
- valor **máximo global** de $f$ sobre $D$ si $f(c)\geqslant f(x)$ para toda $x$ en $D$. 
- valor **mínimo global** de $f$ sobre $D$ si $f(c)\leqslant f(x)$ para toda $x$ en $D$.
#### Máximo/mínimo local
El número $f(c)$ es un 
- valor **máximo local** de $f$ si $f(c)\geqslant f(x)$ cuando $x$ está cerca de $c$. 
- valor **mínimo local** de $f$ si $f(c)\leqslant f(x)$ cuando $x$ está cerca de $c$.

![[Extrema_example_es.svg|361]]

#### Punto crítico
Un número crítico de una función $f$ es un número $x=c$ en el dominio de $f$ tal que $f'(c)=0$ o $f'(c)$ no existe.
Suele ser un lugar donde la función puede tener un máximo, un mínimo o un cambio de comportamiento, **es una condición necesaria para la existencia de extremos relativos, aunque no suficiente**.
