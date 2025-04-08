## Regla de la cadena
Teorema (regla de la cadena): $f\circ g$ debe ser diferenciable.
Cómo obtener el diferencial de una función???
Ejemplo
$$
\begin{gather} \\
f(u,v,w)=u^2+v^2-w, f:\mathbb{R}^3 \rightarrow \mathbb{R}\\
g(x,y,z)=(x^2y,y^2,e^{-xz}), g:\mathbb{R}^3 \rightarrow \mathbb{R}^3\\
\end{gather} \\
$$
Se pide $D(f\circ g)$
$$
\mathbf{D}_{f}=
\begin{bmatrix}  
\frac{\partial f}{\partial u} & \frac{\partial f}{\partial v} & \frac{\partial f}{\partial w}\\
\end{bmatrix}=
\begin{bmatrix}  
2u & 2v & -1\\
\end{bmatrix}
$$
$$
\mathbf{D}_{g}=
\begin{bmatrix}  
\frac{\partial g_{1}}{\partial x} & \frac{\partial g_{1}}{\partial y} & \frac{\partial g_{1}}{\partial z}\\  
\frac{\partial g_{2}}{\partial x} & \frac{\partial g_{2}}{\partial y} & \frac{\partial g_{2}}{\partial z}\\
\frac{\partial g_{3}}{\partial x} & \frac{\partial g_{3}}{\partial y} & \frac{\partial g_{3}}{\partial z} 
\end{bmatrix} = 
\begin{bmatrix}  
2xy & x^2 & 0\\ 
0 & 2y & 0\\
-ze^{xz} & 0 & -ze^{xz}  
\end{bmatrix}
$$
Entonces,
$$
\mathbf{D}_{f}(\mathbf{u})\cdot \mathbf{D}_{g}(\mathbf{x})=
\begin{bmatrix}  
\frac{\partial \math\mathbf{}{\partial x} & 2v & -1\\
\end{bmatrix}
$$