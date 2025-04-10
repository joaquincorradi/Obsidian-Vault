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
---
# Unidad 4
## Esperanza matemática
### Media o valor esperado
Sea $X$ una variable aleatoria con distribución de probabilidad $f(x)$. La media o valor esperado de $X$ es
$$\mu=E(X)=\sum_{x}xf(x)$$
si $X$ es discreta, y
$$\mu=E(X)=\int_{-\infty}^\infty xf(x)dx$$
si $X$ es continua.
