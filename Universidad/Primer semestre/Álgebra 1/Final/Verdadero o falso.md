Determinar si las siguientes afirmaciones son verdaderas o falsas. Justificar en ambos casos.
1. Si $A_{3\times 3}$ y $B_{3\times 3}$ tales que $AB=0$, entonces se debe cumplir que $A=0$ o $B=0$.
	**FALSO.** en general matrices no nulas pueden tener producto nulo. Por ejemplo, existen matrices $A\neq 0$ y $B\neq 0$ tales que $AB=0$:
$$
A \times B = 
\begin{bmatrix} 1 & 1 \\ 0 & 0 \end{bmatrix} 
\begin{bmatrix} 0 & 1 \\ 0 & -1 \end{bmatrix} = 
\begin{bmatrix} (1)(0)+(1)(0) & (1)(1)+(1)(-1) \\ (0)(0)+(0)(0) & (0)(1)+(0)(-1)
\end{bmatrix} = \begin{bmatrix} 0 & 0 \\ 0 & 0 \end{bmatrix}
$$
2. Dado el sistema de ecuaciones lineales no homogéneo $A_{n\times n}\cdot X_{n\times 1}=H_{n\times 1}$ y $A$ es inversible, entonces el sistema tiene una solución única.
	**VERDADERO.** Si $A$ es invertible, se puede multiplicar a ambos lados por $A^{−1}$, y queda
	$$X=A^{-1}H$$
	Por lo tanto, la solución existe y es única.
3. Si un sistema de ecuaciones lineales tiene dos soluciones diferentes entonces el sistema tiene infinitas soluciones.
	**VERDADERO.** Un sistema de ecuaciones lineales solo puede tener cero, una o infinitas soluciones. Si se sabe que tiene dos soluciones distintas, se descartan automáticamente la incompatibilidad (cero) y la solución única (una), por lo que obligatoriamente tiene infinitas soluciones.
4. Si se conocen los tres lados, los ángulos se obtienen por el teorema del seno.
	**FALSO.** Con los tres lados, el método directo **es el teorema del coseno**, no el del seno. El teorema del seno relaciona lados y ángulos opuestos, pero para aplicarlo hace falta conocer al menos un ángulo o algún dato adicional. 
5. Si el coseno de un ángulo es negativo, el ángulo pertenece al primer o segundo cuadrante.
	**FALSO.** El coseno es negativo en el segundo y tercer cuadrante, no en el primero y segundo.”
	
	![[Pasted image 20260713190700.png|376]]
	
6. Dada una matriz $A\in K^{m\times n}$, el $\operatorname{rg}(A)>m$.
	**FALSO.** El rango de una matriz nunca puede superar el número de filas, ni el número de columnas. Siempre se cumple:
	$$\operatorname{rg}(A)\leqslant m\qquad y \qquad \operatorname{rg}(A)\leqslant n$$
7. En un sistema de ecuaciones lineales una incógnita principal es aquella que corresponde a una columna principal en la matriz de coeficientes.
	**VERDADERO.** Las incógnitas principales corresponden a las columnas principales o pivote de la matriz de coeficientes
8. $B$ es equivalente por filas a $A$ cuando $A$ y $B$ son cuadradas.
	**FALSO.** Ser cuadradas no implica equivalencia por filas. La equivalencia por filas requiere que tengan el mismo tamaño y que una se obtenga de la otra por operaciones elementales por filas.
9. La razón trigonométrica que relaciona un ángulo con los dos catetos es el coseno.
	
10. La longitud de un arco se obtiene multiplicando el radio por el ángulo en radianes.
11. Un radian es la medida del radio.