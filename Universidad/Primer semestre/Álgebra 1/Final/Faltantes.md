## Combinación lineal de matrices
Una combinación lineal de matrices consiste en multiplicar varias matrices del mismo tamaño por escalares y sumar los resultados.
Si se tienen matrices $A_{1}, A_{2},\ldots,A_{n}$ y escalares $k_{1}, k_{2},\ldots,k_{n}$ entonces una combinación lineal es:
$$k_{1}A_{1}+k_{2}A_{2}+\cdots +k_{n}A_{n}$$
## Similitudes y diferencias del producto punto y cruz
**Similitudes:**
	- Ambos usan dos vectores como entrada.
	- Ambos se calculan a partir de las componentes de los vectores.
	- Ambos dependen del ángulo entre ellos.
	- Ambos sirven para estudiar relaciones geométricas entre vectores.
Diferencias:
	- El producto punto da un número real (escalar) y el producto cruz da un vector.
	- El producto punto mide cuánto apuntan en la misma dirección; el cruz mide un vector perpendicular a ambos.
	- El producto punto vale $0$ cuando los vectores son **perpendiculares** y el producto cruz vale el vector nulo cuando los vectores son **paralelos**.
## Responder
¿Cuál de las siguientes ecuaciones es una ecuación lineal en las variables $x, y, z, w$ y por qué?
1. $x+y-z=w^2$
2. $\frac{x+y-z}{w}=2$
3. $\sqrt{ x+y-z }=2w$
4. $\frac{x+y-z}{2}=w$
**Respuesta correcta: 4**
Para que una ecuación sea considerada lineal en múltiples variables, **todas las incógnitas deben estar elevadas a la primera potencia**, **no deben multiplicarse ni dividirse entre sí**, y **no pueden estar sujetas a operaciones como raíces, logaritmos o funciones trigonométricas**.
- **Ecuación 1:** ‭$x+y-z=w^2$‬‭‬‭‬‭‬
	No es lineal porque la variable ‭$w$‬ está elevada a una potencia distinta de uno (al cuadrado).
-  **Ecuación 2:** ‭$\frac{x+y-z}{w}=2$‬‭‬
	No es lineal porque la variable ‭$w$‬ se encuentra en el denominador, lo que implica una división por una variable (equivalente a ‭$w^{-1}$‬).
- **Ecuación 3:** ‭$\sqrt{x+y-z}=2w$‬‭‬
	No es lineal porque las variables ‭$x, y, z$‬‭‬ ‭‬‭‬ ‭‬se encuentran dentro de una raíz cuadrada, lo cual representa exponentes fraccionarios (‭$(x+y-z)^{\frac{1}{2}}$‬‭‬‭‬‭‬‭‬).
## Completar
1. Una matriz es un ___ dispuestos en filas y ___ . Si una matriz $A$ se representa como $A_{2\times 3}$ significa que tiene ____.
2. Sea la matriz $\left[\begin{array}{@{}cccccc|c@{}} a_{11} & a_{12} & \cdots & a_{1r} & \cdots & a_{1n} & b_1 \\ 0 & a_{22} & \cdots & a_{2r} & \cdots & a_{2n} & b_2 \\ \vdots & \vdots & \vdots & \vdots & \ddots & \vdots & \vdots \\ 0 & 0 & \cdots & a_{rr} & \cdots & a_{rn} & b_r \end{array}\right]$ asociada al sistema resolvente, se concluye que el sistema es ___ . Las variables (o incógnitas) principales corresponden a las ___ en la matriz ___ . Las variables que pueden tomar valores arbitrarios se llaman ___ .
3. En el ___ las funciones trigonométricas son positivas. En particular la función $4\sin(2\theta-1)+3$, el $4$ representa la ___ ___ , el $3$ representa el ___ , el periodo es ___ y el ángulo de fase vale ___ .
4. Un vector es 