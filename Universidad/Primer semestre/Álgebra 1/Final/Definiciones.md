## * Matriz
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
diagonal principal valen $1$ y el resto de los elementos son $0$.
$$
I_n = \begin{bmatrix}
1 & 0 & \cdots & 0 \\
0 & 1 & \cdots & 0 \\
\vdots & \vdots & \ddots & \vdots \\
0 & 0 & \cdots & 1 \\\end{bmatrix}
$$
#### Matriz traspuesta
Dada una matriz cualquiera $A\in M_{m\times n}$, su traspuesta es otra matriz $A^t\in M_{n\times m}$ cuyas filas son las columnas de $A$ dispuestas en el mismo orden.
$$
\begin{bmatrix}
      a & b  \\
      c & d  \\
      e & f  \\
   \end{bmatrix}^t
   =
   \begin{bmatrix}
      a & c & e \\
      b & d & f \\
\end{bmatrix}
$$
#### * Matriz simétrica
