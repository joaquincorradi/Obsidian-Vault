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
Es decir, $f$ es continua en $a$.

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
Por lo tanto $\boxed{f'(c)=0}$, es decir, la derivada en $c$ vale cero.
### Teorema de Rolle (*a la misma altura / tres hipótesis*)
*Idea clave: si empieza y termina a la misma altura, alguna tangente interior tiene que ser horizontal.*

**Enunciado:** si $f$ es una función que satisface las siguientes tres hipótesis:
1. $f$ es continua sobre el intervalo cerrado $[a,b]$.
2. $f$ es derivable sobre el intervalo abierto $(a, b)$.
3. $f(a)=f(b)$
entonces hay un número $c$ en $(a, b)$ tal que $f'(c)=0$.

![[Captura de pantalla 2026-06-27 a la(s) 7.48.18 p. m..png]]

**Demostración:** *pendiente*
### Teorema de Lagrange (*dos hipótesis*)
*Idea clave: una tangente interior tiene la misma pendiente que la secante del intervalo.*

**Enunciado:** si $f$ es una función que satisface las siguientes dos hipótesis:
1. $f$ es continua sobre el intervalo cerrado $[a,b]$.
2. $f$ es derivable sobre el intervalo abierto $(a, b)$.
entonces existe un número $x=c$ en $(a, b)$ tal que
$$f'(c)= \frac{f(b)-f(a)}{b-a}$$
**Demostración:**
Sea $h$ definida como la diferencia entre $f$ y la función cuya gráfica es la recta secante AB:
$$h(x)=f(x)-\left[ f(a)+\frac{f(a)-f(b)}{a-b} \right]$$
### Teorema de Cauchy
