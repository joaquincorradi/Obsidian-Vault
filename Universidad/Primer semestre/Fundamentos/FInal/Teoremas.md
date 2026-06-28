# Continuidad:
### Teorema del valor intermedio (TVI)
*Idea clave: una función continua no salta valores.*

**Enunciado**: Si $f$ es continua en $[a,b]$ y $k$ está entre $f(a)$ y $f(b)$ entonces existe al menos un $c\in[a,b]$ tal que $f(c)=k$.
### Teorema de Bolzano
*Idea clave: caso particular de TVI*

**Enunciado:** Si $f$ es continua en $[a,b]$ y $f(a)<0<f(b)$ entonces existe al menos un $c\in[a,b]$ tal que $f(c)=0$. 

---

# Derivada:
### Regla de la cadena

### Teorema "derivabilidad implica continuidad”
**Enunciado:** si $f$ es derivable en $x=a$, entonces $f$ es continua en $x=a$. 

**Demostración:** 
Queremos demostrar que $\lim_{ x \to a }f(x)=f(a)$.
$f$ es derivable en $x=a$, entonces
$$f'(a)=\lim_{ x \to a } \frac{f(x)-f(a)}{x-a}$$
Para relacionar lo dado con lo desconocido, divido y multiplico $f(x)-f(a)$ por $x-a$:
$$\begin{gather}
\frac{f(x)-f(a)}{x-a}=\frac{f(x)-f(a)}{x-a},\qquad x\neq a \\
f(x)-f(a)=\frac{f(x)-f(a)}{x-a}({x-a}),\qquad x\neq a
\end{gather}$$
De este modo, si usamos la ley del producto:
$$\begin{align}
\lim_{ x \to a }[f(x)-f(a)]&=\lim_{ x \to a }\frac{f(x)-f(a)}{x-a}\lim_{ x \to a }({x-a}) \\
&=f'(a)\cdot 0 \\
\end{align}$$
$$\boxed{\lim_{ x \to a }[f(x)-f(a)]=0}$$
Para utilizar lo que acabo de demostrar, comienzo con $f(x)$ y sumo y resto $f(a)$:
$$\begin{align}
\lim_{ x \to a }f(x)&=\lim_{ x \to a }[f(x)-f(a)]+f(a) \\
&=\lim_{ x \to a }[f(x)-f(a)]+\lim_{ x \to a }f(a) \\
&=0+f(a)
\end{align}$$
$$\boxed{\lim_{ x \to a }f(x)=f(a)}$$
Es decir, $f$ es continua en $a$. Q.E.D.

### Teorema de Fermat
**Enunciado:** Si $f$ tiene un máximo o un mínimo local en $x=c$, **y además** $f'(c)$ existe, entonces $f'(c)=0$.

![[Captura de pantalla 2026-06-27 a la(s) 9.00.22 p. m..png|348]]

**Demostración:**
Suponemos $f$ definida en $(a,b)$ presenta un máximo local en $c\in(a,b)$ y suponemos que existe $f'(c)$, entonces
$$f'(c)=\lim_{ h \to 0^+ } \frac{f(c+h)-f(c)}{h}=\lim_{ h \to 0^- } \frac{f(c+h)-f(c)}{h}$$
Pero $f(c)$ es un máximo local y es más grande que cualquier valor de la cercanía, es decir, $f(x)\geqslant f(x)+h$ y, por consiguiente, $f(c+h)-f(c)\leqslant 0$. Entonces,
$$\lim_{ h \to 0^+ } \frac{f(c+h)-f(c)}{h}\leqslant 0$$
y,
$$\lim_{ h \to 0^+ } \frac{f(c+h)-f(c)}{h}\geqslant 0$$
Entonces,
$$\begin{gather}
f'(c)\leqslant 0 \\
f'(c)\geqslant 0
\end{gather}$$
Por lo tanto $\boxed{f'(c)=0}$, es decir, la derivada en $c$ vale cero. Q.E.D.
### Teorema de Rolle (*a la misma altura / tres hipótesis*)
*Idea clave: si empieza y termina a la misma altura, alguna tangente interior tiene que ser horizontal.*

**Enunciado:** si $f$ es una función que satisface las siguientes tres hipótesis:
1. $f$ es continua sobre el intervalo cerrado $[a,b]$.
2. $f$ es derivable sobre el intervalo abierto $(a, b)$.
3. $f(a)=f(b)$
entonces hay un número $x=c$ en $(a, b)$ tal que $f'(c)=0$.

![[Captura de pantalla 2026-06-27 a la(s) 7.48.18 p. m..png]]

**Demostración:** *pendiente*
### Teorema de Lagrange (*dos hipótesis*)
*Idea clave: una tangente interior tiene la misma pendiente que la secante del intervalo.*

**Enunciado:** si $f$ es una función que satisface las siguientes dos hipótesis:
1. $f$ es continua sobre el intervalo cerrado $[a,b]$.
2. $f$ es derivable sobre el intervalo abierto $(a, b)$.
entonces existe un número $x=c$ en $(a, b)$ tal que
$$f'(c)= \frac{f(b)-f(a)}{b-a}$$

![[Captura de pantalla 2026-06-28 a la(s) 5.57.48 p. m..png|552]]

**Demostración:**
Sea $h$ definida como la diferencia entre $f$ y la función cuya gráfica es la recta secante AB:
$$h(x)=f(x)-\left[ f(a)+\frac{f(b)-f(a)}{b-a}(x-a) \right]$$
Primero, debemos verificar que h satisface las tres hipótesis del teorema de Rolle. 
1. La función $h$ **es continua** sobre $[a,b]$ porque es la suma de $f$ y una función polinomial de primer grado, ambas continuas.
2. La función $h$ **es derivable** sobre $(a, b)$ porque $f$ y la función polinomial de primer grado son derivables.
3. Y
$$\begin{gather}
h(a)=f(a)-\left[ f(a)+\cancelto{0}{\frac{f(b)-f(a)}{b-a}(a-a)} \right]=0 \\
h(b)=f(b)-\left[ f(a)+\frac{f(b)-f(a)}{\cancel{b-a}}(\cancel{b-a}) \right]=0
\end{gather}$$
por lo tanto, $h(a)=h(b)$.
Dado que $h$ satisface las tres hipótesis del teorema de Rolle entonces existe un número $x=c$ en $(a, b)$ tal que $h'(c)=0$, entonces se tiene:
$$
\begin{gather}
h'(x)=f'(x)-\frac{f(b)-f(a)}{b-a} \\
h'(c)=f'(c)-\frac{f(b)-f(a)}{b-a}=0
\end{gather}
$$
Así que
$$\boxed{f'(c)=\frac{f(b)-f(a)}{b-a}}$$
Q.E.D.

![[Captura de pantalla 2026-06-28 a la(s) 5.55.48 p. m..png|286]]
### Teorema de Cauchy (*tres hipótesis*)
*Idea clave: es una generalización de Lagrange.*

**Enunciado:** si $f$ y $g$ son funciones que satisface las siguientes tres hipótesis:
1. $f$ y $g$ son continuas sobre el intervalo cerrado $[a,b]$.
2. $f$ y $g$ son derivables sobre el intervalo abierto $(a, b)$.
3. $g'(x)\neq 0$ en $(a,b)$.
entonces hay un número $x=c$ en $(a, b)$ tal que
$$\frac{f'(c)}{g'(b)}=\frac{f(b)-f(a)}{g(b)-g(a)}$$

**Demostración:**
Sea $h$
$$h(x)=[g(b)-g(a)] \cdot [f(x)-f(a)] - [f(b)-f(a)] \cdot [g(x)-g(a)]$$

Primero, debemos verificar que h satisface las tres hipótesis del teorema de Rolle. 
1. La función $h$ **es continua** sobre $[a,b]$ porque es la suma de dos funciones continuas multiplicadas por una constante.
2. La función $h$ **es derivable** sobre $(a, b)$ porque es la suma de dos funciones diferenciables multiplicadas por una constante.
3. Y
$$
\begin{gather}
h(a)=\cancelto{0}{[g(b)-g(a)] \cdot [f(a)-f(a)]} - \cancelto{0}{[f(b)-f(a)] \cdot [g(a)-g(a)]}=0 \\
h(b)=\cancel{[g(b)-g(a)] \cdot [f(b)-f(a)]} \cancel{- [f(b)-f(a)] \cdot [g(b)-g(a)]}=0
\end{gather}
$$
por lo tanto, $h(a)=h(b)$.
Dado que $h$ satisface las tres hipótesis del teorema de Rolle entonces existe un número $x=c$ en $(a, b)$ tal que $h'(c)=0$, entonces se tiene:
$$
\begin{gather}
h'(x)=[g(b)-g(a)] \cdot f'(x) - [f(b)-f(a)] \cdot [g(x)-g(a)]
\end{gather}
$$