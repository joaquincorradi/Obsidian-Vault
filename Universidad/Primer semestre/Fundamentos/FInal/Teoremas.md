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

**Demostración:**
$f$ presenta un máximo local en $c$ y suponemos que es derivable en $x=c$, entonces
$$f'(c)=\lim_{ h \to 0^+ } \frac{f(c+h)-f(c)}{h}=\lim_{ h \to 0^- } \frac{f(c+h)-f(c)}{h}$$
Pero $f(c)$ es un máximo local y es más grande que cualquier valor de la cercanía. Entonces,
$$\lim_{ h \to 0^+ } \frac{f(c+h)-f(c)\to\leqslant 0}{h\to\geqslant 0}\to\leqslant 0$$
y,
$$\lim_{ h \to 0^+ } \frac{f(c+h)-f(c)\to\leqslant 0}{h\to\leqslant 0}\to\geqslant 0$$
Entonces,
$$\begin{gather}
f'(c)\leqslant 0 \\
f'(c)\geqslant 0
\end{gather}$$
Por lo tanto $f'(c)=0$, es decir, la derivada en $c$ vale cero.

### Teorema de Rolle
### Teorema de Lagrange
### Teorema de Cauchy
