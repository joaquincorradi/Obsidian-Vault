# Repaso unidad 3
- Variable aleatoria: $2$-upla que asocia un número real con un elemento del espacio muestral.
- Espacio muestral continuo: un espacio muestral que contiene un número finito de posibilidades, o una serie interminable con tantos elementos como números enteros existen.
- Espacio muestral continuo: un espacio muestral que contiene un número infinito de posibilidades, igual al número de puntos en un segmento de recta.
- Distribución de probabilidad: el conjunto de pares ordenados $(x, f (x))$ es una función de probabilidad, una función de masa de probabilidad o una distribución de probabilidad de la variable aleatoria discreta $X$ si, para cada resultado x posible,
	1. $f(x)\geqslant 0$
	2. $\sum_{x}f(x)=1$
	3. $P(X=x)=f(x)$
- La función de la distribución acumulativa $F(x)$ de una variable aleatoria discreta $X$ con distribución de probabilidad $f(x)$ es 
	$$F(x)=P(X\leqslant x)=\sum_{t\leqslant x}f(t),\ -\infty <x<\infty$$
- La combinación total de patentes en Argentina es:
	$$26^2\times10^3\times26^2=26^4\times10^3=456.976.000$$
---
# Unidad 4
## Esperanza matemática
Es el promedio de todos los posibles resultados de una variable aleatoria.
### Media o valor esperado (esperanza)
Sea $X$ una variable aleatoria con distribución de probabilidad $f(x)$. La media o valor esperado de $X$ es
$$\mu=E(X)=\sum_{x}xf(x)$$
si $X$ es discreta, y
$$\mu=E(X)=\int_{-\infty}^\infty xf(x)dx$$
si $X$ es continua.

Sea $X$ una variable aleatoria con distribución de probabilidad $f(x)$. El valor esperado de la variable aleatoria $g(X)$ es
$$\mu_{g(X)}=E[g(X)]=\sum_{x}f(x)g(x)$$
si $X$ es discreta, y
$$\mu_{g(X)}=E[g(X)]=\int_{-\infty}^\infty f(x)g(x)dx$$
si $X$ es continua.
### Varianza de $X$
Sea $X$ una variable aleatoria con distribución de probabilidad $f(x)$ y media μ. La varianza de $X$ es
$$\sigma^2=E[(X-\mu)^2]=\sum_{x}(x-\mu)^2f(x)$$
si $X$ es discreta, y
$$\sigma^2=E[(X-\mu)^2]=\int_{-\infty}^\infty (x-\mu)^2f(x)dx$$
si $X$ es continua.
La raíz cuadrada positiva de la varianza, $\sigma$, se llama desviación estándar de $X$.
### Varianza de una variable aleatoria
La varianza de una variable aleatoria $X$ es
$$\sigma^2=E(X^2)-\mu^2$$
### Media o valor esperado de $X, Y$
Sean $X$ y $Y$ variables aleatorias con distribución de probabilidad conjunta $f(x, y)$. La media o valor esperado de la variable aleatoria $g(X, Y)$ es
$$\mu_{g(X,Y)}=E[g(X,Y)]=\sum_{x}\sum_{y}g(x,y)f(x,y)$$
si $X$ y $Y$ son discretas, y
$$\mu_{g(X,Y)}=E[g(X,Y)]=\int_{-\infty}^\infty\int_{-\infty}^\infty g(x,y)f(x,y)dxdy$$
si $X$ y $Y$ son continuas.