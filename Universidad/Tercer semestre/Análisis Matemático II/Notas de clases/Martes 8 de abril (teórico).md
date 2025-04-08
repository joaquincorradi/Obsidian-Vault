## Regla de la cadena
Teorema (regla de la cadena): $f\circ g$ debe ser diferenciable.
Cómo obtener el diferencial de una función???
El dominio de uno tiene que coincidir con la imagen de otro y ese es el orden, por ejemplo
$f:\mathbb{R}^2 \rightarrow \mathbb{R}^2$ y $g:\mathbb{R}^2 \rightarrow \mathbb{R}^3$ se debe hacer $g\circ f$.

Ejemplo 1:
$$
\begin{gather} \\
f(u,v,w)=u^2+v^2-w, f:\mathbb{R}^3 \rightarrow \mathbb{R}\\
g(x,y,z)=(x^2y,y^2,e^{-xz}), g:\mathbb{R}^3 \rightarrow \mathbb{R}^3\\
\mathbf{x}=(x,y,z); \mathbf{u}=(u,v,w)
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
\frac{\partial \mathbf{z}}{\partial x} & \frac{\partial \mathbf{z}}{\partial y} & \frac{\partial \mathbf{z}}{\partial z}\\
\end{bmatrix}
$$
$$
\begin{gather}
\frac{\partial \mathbf{z}}{\partial x}=4uxy+ze^{-xz}=4x^3y^2+ze^{-xz}\\
\frac{\partial \mathbf{z}}{\partial y}=2ux^2+4vy=2x^4y+4y^3\\
\frac{\partial \mathbf{z}}{\partial z}=xe^{-xz}
\end{gather}
$$
$$
\mathbf{D}_{f}(\mathbf{u})\cdot \mathbf{D}_{g}(\mathbf{x})=
\begin{bmatrix}  
4x^3y^2+ze^{-xz} & 2x^4y+4y^3 & xe^{-xz}\\
\end{bmatrix}
$$

Ejemplo 2:
Calcular $g\circ f$ en $(1,1)$ aplicando la regla de la cadena (se valua el punto en el segundo componente de la composición, en este caso la $f$):
$$
\begin{gather}
f(x,y)=(x^2+1,y^2);f:\mathbb{R}^2 \rightarrow \mathbb{R}^2 \\
g(u,v)=(u+v,u,v^2);g:\mathbb{R}^2 \rightarrow \mathbb{R}^3 \\
\mathbf{x}=(x,y)
\end{gather}$$
$$
\begin{gather}
\mathbf{D}(g\circ f)=\mathbf{D}_{x}g\cdot\mathbf{D}_{x}f \\
\mathbf{x}_{0}=(1,1) \\
\mathbf{y}_{0}=(2,1)
\end{gather}
$$
$$
\mathbf{D}_{\mathbf{y}}g=
\begin{bmatrix}  
\frac{\partial g_{1}}{\partial x} & \frac{\partial g_{1}}{\partial y}\\  
\frac{\partial g_{2}}{\partial x} & \frac{\partial g_{2}}{\partial y}\\
\frac{\partial g_{3}}{\partial x} & \frac{\partial g_{3}}{\partial y}
\end{bmatrix} = 
\begin{bmatrix}  
1 & 1\\  
1 & 0\\
0 & 2v
\end{bmatrix}
$$
$$
\mathbf{D}_{\mathbf{y}_{0}}g=\mathbf{D}g(2,1)=
\begin{bmatrix}  
1 & 1\\  
1 & 0\\
0 & 2
\end{bmatrix}
$$
$$
\mathbf{D}_{\mathbf{x}}f=
\begin{bmatrix}  
\frac{\partial f_{1}}{\partial x} & \frac{\partial f_{1}}{\partial y} \\  
\frac{\partial f_{2}}{\partial x} & \frac{\partial f_{2}}{\partial y}
\end{bmatrix} = 
\begin{bmatrix}  
2x & 0 \\  
0 & 2y
\end{bmatrix}
$$
$$
\mathbf{D}f(1,1)=
\begin{bmatrix}  
2 & 0 \\  
0 & 2
\end{bmatrix}
$$

Ejemplo 3:
$$
\begin{gather}
z=\ln{x^2+y^2} \\
x=t^2, y=t^{-2} \\
\frac{dz}{dt}
\end{gather}
$$
Entonces
$$
\begin{gather}
f(x,y)=\ln{x^2+y^2} \\
g(t)=(t^2,t^{-2})
\end{gather}
$$
$$
\begin{align}
\frac{dz}{dt}&=\\partial fvec{\nabla}f\cdot \dot{g}(t) \\
&=\begin{bmatrix}
\frac{\partial f}{\partial x} & \frac{\partial f}{\partial y}
\end{bmatrix} \cdot \begin{bmatrix}
\frac{\partial f}{\partial x} & \frac{\partial f}{\partial y}
\end{bmatrix}
\end{align}
$$
