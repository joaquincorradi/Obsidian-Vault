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
Dada una matriz cualquiera $A\in M_{m\times n}$, su traspuesta es otra matriz $A^\textsf{t}\in M_{n\times m}$ cuyas filas son las columnas de $A$ dispuestas en el mismo orden.
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
#### $\star$ Matrices equivalentes por fila
Dos matrices son equivalentes si es posible transformar una en la otra aplicando una cantidad finita de operaciones elementales de fila.
#### Matriz escalonada por filas (MEF)
Una matriz se dice escalonada por filas si:
1. Todas las filas nulas (si los hay) están en la parte inferior de la matriz.
#### $\star$ Matriz escalonada reducida por filas (MERF)


