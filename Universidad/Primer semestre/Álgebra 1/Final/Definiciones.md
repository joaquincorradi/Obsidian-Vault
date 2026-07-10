*$\star$: aparecen en finales.*
## $\star$ Matriz
Una matriz $A$ de $m\times n$ es un arreglo rectangular de $mn$ números dispuestos en $m$ filas y $n$ columnas.
$$
A = \begin{bmatrix}
a_{11} & a_{12} & \cdots & a_{1n} \\
a_{21} & a_{22} & \cdots & a_{2n} \\
\vdots  & \vdots  & \ddots & \vdots \\
a_{m1} & a_{m2} & \cdots & a_{mn} \\ \end{bmatrix}_{ m\times n}
$$
Los elementos de $A$ se denotan por $a_{ij}$ aparece. El subíndice $i$ indica la fila donde se ubica el elemento y $j$ la columna.
#### Matriz fila
Se llama matriz fila a toda matriz de orden $1\times n$.
$$
A = \begin{bmatrix}
a_{11} & a_{12} & \cdots & a_{1n} \\ \end{bmatrix}_{ 1\times n}
$$
#### Matriz columna
Se llama matriz fila a toda matriz de orden $m\times 1$.
$$
A = \begin{bmatrix}
a_{11} \\
a_{21} \\
\vdots \\
a_{m1} \\ \end{bmatrix}_{ m\times 1}
$$
#### Matriz cuadrada
Se llama matriz cuadrada a toda matriz que tiene la misma cantidad de filas que de columnas.
#### Diagonal principal
La diagonal principal de una matriz cuadrada la forman los elementos $a_{ij}$ en los cuales $i=j$.
#### Matriz identidad
La matriz identidad de orden $n$ es una matriz cuadrada en la cual todos los elementos de la
diagonal principal valen uno y el resto de los elementos son cero.
$$
I_n = \begin{bmatrix}
1 & 0 & \cdots & 0 \\
0 & 1 & \cdots & 0 \\
\vdots & \vdots & \ddots & \vdots \\
0 & 0 & \cdots & 1 \\\end{bmatrix}
$$
#### Matriz traspuesta
Dada una matriz cualquiera $A$ de ${m\times n}$, su traspuesta es otra matriz $A^\textsf{t}$ de ${n\times m}$ cuyas filas son las columnas de $A$ dispuestas en el mismo orden.
$$
\begin{bmatrix}
      a & b  \\
      c & d  \\
      e & f  \\
   \end{bmatrix}^\textsf{t}
   =
   \begin{bmatrix}
      a & c & e \\
      b & d & f \\
\end{bmatrix}
$$
#### $\star$ Matriz simétrica
Una matriz es simétrica si es una matriz cuadrada, la cual tiene la característica de ser igual a su traspuesta.
$$A \text{ es simétrica} \iff A = A^\textsf{t}$$
Por ejemplo:
$$
\begin{bmatrix}
    1 & 7 & 3 \\
    7 & 4 & 5 \\
    3 & 5 & 2
  \end{bmatrix}
$$
#### $\star$ Matriz triangular superior
Una matriz triangular superior es una matriz cuadrada donde todos los elementos situados por debajo de su diagonal principal son cero.
$$
A = \begin{bmatrix}
a_{11} & a_{12} & a_{13} \\
0 & a_{22} & a_{23} \\
0 & 0 & a_{33} \\ \end{bmatrix}
$$
#### $\star$ Matriz triangular inferior
Una matriz triangular superior es una matriz cuadrada donde todos los elementos situados por encima de su diagonal principal son cero.
$$
A = \begin{bmatrix}
a_{11} & 0 & 0 \\
a_{21} & a_{22} & 0\\
a_{31} & a_{32} & a_{33} \\ \end{bmatrix}
$$
#### $\star$ Operación elemental de fila
Las operaciones elementales por filas son transformaciones matemáticas que se aplican a las filas de una matriz. Hay tres tipos de operaciones elementales de fila:
1. Intercambiar las posiciones de dos filas: $R_{i}\leftrightarrow R_{j}$.
2. Multiplicar una fila por un escalar distinto de cero: $R_{i}\to kR_{i}$.
3. Sumar un múltiplo de una fila a otra fila: $R_{i}\to kR_{i}+R_{j}$
#### $\star$ Matriz elemental
Una matriz elemental es una matriz cuadrada de $n\times n$ obtenida al aplicar una única operación elemental por filas a la matriz identidad.
#### $\star$ Matrices equivalentes por fila
Dos matrices son equivalentes si es posible transformar una en la otra aplicando una cantidad finita de operaciones elementales de fila.
#### Matriz escalonada por filas (MEF)
Una matriz se dice escalonada por filas si:
1. Todas las filas nulas (si los hay) están en la parte inferior de la matriz.
2. En cada fila no nula, el primer número distinto de cero es $1$.
3. El pivote en cualquier fila está a la derecha del pivote de la fila anterior.
$$
\begin{bmatrix}
1 & a_0 & a_1 & a_2 & a_3 \\
0 & 0 & 1 & a_4 & a_5 \\
0 & 0 & 0 & 1 & a_6 \\
0 & 0 & 0 & 0 & 0
\end{bmatrix}
$$
#### $\star$ Matriz escalonada reducida por filas (MERF)
Una matriz se dice escalonada reducida por filas si:
1. Todas las filas nulas (si los hay) están en la parte inferior de la matriz.
2. En cada fila no nulo, el primer número distinto de cero es 1.
3. El pivote en cualquier fila está a la derecha del pivote de la fila anterior.
4. Cada columna que contiene un pivote tiene ceros en todas sus demás entradas.
$$
\begin{bmatrix}
1 & a_0 & 0 & 0 & a_3 \\
0 & 0 & 1 & 0 & a_5 \\
0 & 0 & 0 & 1 & a_6 \\
0 & 0 & 0 & 0 & 0
\end{bmatrix}
$$
#### $\star$ Rango de una matriz
El rango de una matriz es el número máximo de filas que son linealmente independientes.
#### $\star$ Matrix invertible
Una matriz cuadrada $A$ de $n\times n$ se dice invertible si existe otra matriz cuadrada $B$ de $n\times n$ tal que
$$AB=BA=I$$
Entonces $B$ se llama inversa de $A$ y se denota por $A^{-1}$. Entonces se tiene
$$AA^{-1}=A^{-1}A=I$$
#### Determinante de una matriz
El determinante es un valor numérico asociado a una matriz cuadrada.
- El determinante de una matriz de $2\times 2$:
$$
\operatorname{\det}A = 
   \begin{vmatrix}
      a_{11} & a_{12} \\
      a_{21} & a_{22}
   \end{vmatrix}
   =
     a_{11} a_{22}
   - a_{12} a_{21}
$$
- El determinante de una matriz de $3\times 3$:
$$
\operatorname{\det}A =
\begin{vmatrix}
    a_{11} & a_{12} & a_{13} \\
      a_{21} & a_{22} & a_{23} \\
      a_{31} & a_{32} & a_{33}
\end{vmatrix}
=
(a_{11} a_{22} a_{33} 
   + a_{12} a_{23} a_{31} 
   + a_{13} a_{21} a_{32}) 
   - (a_{31} a_{22} a_{13} 
   + a_{32} a_{23} a_{11} 
   + a_{33} a_{21} a_{12})
$$

---

## $\star$ Vector
Un vector es un segmento de recta dirigido que cuenta con módulo, dirección y sentido. 
Si está determinado por dos puntos $P$ y $Q$, se lo denota $\vec v=\overrightarrow{PQ}$​, donde $P$ es el punto inicial y $Q$ el punto final.

![[Vector_00.svg|437]]

- **Modulo (o magnitud):** es la longitud del vector, y se expresa mediante un número no negativo.
- **Dirección:** es la recta de soporte del vector, o sea, la recta sobre la cual se encuentra el segmento. (horizontal, vertical o un ángulo específico).
- **Sentido:** indica hacia cuál de los dos extremos de la dirección apunta el vector. (positivo o negativo).
#### Clasificación de vectores
- **Vectores equipolentes:** dos vectores fijos se consideran equipolentes si tienen igual módulo, dirección y sentido.
- **Vector fijo:** tienen un determinado punto de aplicación (punto inicial del segmento orientado).
- $\star$ **Vector libre:** segmento dirigido que puede ubicarse en cualquier punto del plano o del espacio, manteniendo siempre su módulo, dirección y sentido.
- **Vector unitario/versor:** vector cuyo módulo es igual a $1$. Se utiliza para representar únicamente la dirección y el sentido de un vector. Si $\vec{v}\neq \vec{0}$, el versor asociado se obtiene dividiendo el vector por su módulo (normalizar):
$$\hat{v}=\frac{\vec{v}}{\left\|\vec{v}\right\|}$$
#### Modulo de un vector
Sea $\vec{v}=(v_{1}, v_{2}, v_{3})$, su módulo es el número real dado por la expresión:
$$\left\|\vec{v}\right\|=\sqrt {v_{1}^2+v_{2}^2+v_{3}^2}$$

#### $\star$ Producto punto (producto escalar, producto interno)
El producto punto de dos vectores $\vec{u}$ y $\vec{v}$, se define por:
$$\vec{u}\cdot \vec{v}=\left\|\vec{u}\right\|\left\|\vec{v}\right\|\cos(\theta)$$
donde $\theta$ es el ángulo entre ambos vectores. El resultado es un **número real**.
En coordenadas, si $\vec{u}=(u_1, \ldots, u_n)$ y $\vec{v}=(v_1, \ldots, v_n)$,
$$\vec{u}\cdot \vec{v}=u_{1}v_{1}+\cdots+u_{n}v_{n}$$
#### Producto cruz (producto vectorial)
El producto punto de dos vectores $\vec{u},\vec{v}\in \mathbb{R}^3$, se define por:

