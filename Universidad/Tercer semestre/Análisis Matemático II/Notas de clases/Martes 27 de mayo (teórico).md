*Ejemplo 1*:
1. Determinar si los siguientes campos vectoriales son conservativos. De serlo, determinar la función potencial.
	*a)* $F(x,y)=x^2y\vec{i}+xy\vec{j}$:
		$$\begin{gather}
M(x,y)=x^2y, \quad N(x,y)=xy \\
\frac{\partial M}{\partial y}\stackrel{?}{=}\frac{\partial N}{\partial x} \\
\frac{\partial M}{\partial y}=x^2, \quad \frac{\partial N}{\partial x}=y \\
\frac{\partial M}{\partial y}\neq\frac{\partial N}{\partial x}
\end{gather}$$
		Entonces, el campo F no es conservativo.
	
	*b)* $G(x,y)(3+2xy)\vec{i}+(x^2-3y^2)\vec{j}$:
		$$
		\begin{gather}
M(x,y)=3+2xy,\quad N(x,y)=x^2-3y^2 \\
\frac{\partial M}{\partial y}\stackrel{?}{=}\frac{\partial N}{\partial x} \\
\frac{\partial M}{\partial y}=2x,\quad \frac{\partial N}{\partial x}=2x \\
\frac{\partial M}{\partial y}=\frac{\partial N}{\partial x}
\end{gather}
		$$
		$G$ es conservativa y $\mathbb{F}=\vec{\nabla}f\to f$ es una función potencial.
		Ahora se realiza el cálculo de la función potencial:
		$$
		\begin{gather}
\vec{\nabla}f=\frac{\partial f}{\partial x}\vec{i}+\frac{\partial f}{\partial y}\vec{j}=\left( \frac{\partial f}{\partial x}, \frac{\partial f}{\partial y} \right) \\
\frac{\partial f}{\partial x}=3+2xy \; \text{(1)},\quad \frac{\partial f}{\partial y}=x^2-3y^2 \; \text{(2)} \\
F(x,y)=(3+2xy)\vec{i}+(x^2-3y^2)\vec{j}=\frac{\partial f}{\partial x}\vec{i}+\frac{\partial f}{\partial y}\vec{j}
\end{gather}
		$$
		De la expresión $\text{(1)}$, integramos con respecto de $x$:
		$$
		\begin{gather}
f(x,y)=\int(3+2xy)dx \\
f(x,y)=3x+x^2y+g(y)
\end{gather}
		$$
		Calculamos $g(y)$. Derivamos $f(x,y)$ respecto de $y$:
		$$
		\begin{gather}
\frac{\partial f}{\partial y}=x^2+g'(y) \\
\cancel{x^2}-3y^2=\cancel{x^2}+g'(y) \\
g'(y)=-3y^2 \\
\int-3y^2dy=-y^3+C
\end{gather}
		$$
		Entonces, una función potencial es $f(x,y)=3x+x^2y-y^3+C$.


*Ejemplo 2*:
2. Determinar si los siguientes campos vectoriales son conservativos. De serlo, determinar la función potencial.
	Recordar que:
	$$
	\begin{gather}
rot\mathbb{F}=\vec{\nabla}\times\mathbb{F}=\overline{0} \\
\vec{\nabla}=\frac{\partial}{\partial x}\vec{i}+\frac{\partial}{\partial y}\vec{j}+\frac{\partial}{\partial z}\vec{k} \\
\vec{\nabla}\times\mathbb{F}=\left( \frac{\partial R}{\partial y}-\frac{\partial Q}{\partial z} \right)\vec{i}+\left( \frac{\partial P}{\partial z}-\frac{\partial R}{\partial x} \right)\vec{j}+\left( \frac{\partial Q}{\partial x}-\frac{\partial P}{\partial y} \right)\vec{k}=0\vec{i}+0\vec{j}+0\vec{k}
\end{gather}
	$$
	*a)* $\mathbb{F}(x,y,z)=(x^3y,\ 3z+x,\ y+z)$
		$$
		\vec{\nabla}\times\mathbb{F}=(1-3)\vec{i}+(0-0)\vec{j}+(1-x^3)\vec{k}
		$$

	*b)* $\mathbb{G}(x,y,z)=(y^2,\ 2xy+e^{3z},\ 3ye^{3z})$
		$$
\vec{\nabla}\times\mathbb{F}=(3e^{3z}-3e^{3z})\vec{i}+(0-0)\vec{j}+(2y-2y)\vec{k}
		$$
		$\mathbb{G}$ es conservativa y $\mathbb{G}=\vec{\nabla}f=\frac{\partial f}{\partial x}\vec{i}+\frac{\partial f}{\partial y}\vec{j}+\frac{\partial f}{\partial z}\vec{k}$.
		Entonces,
		$$\begin{gather}
\frac{\partial f}{\partial x}=y^2,\;\text{(1)}\quad\frac{\partial f}{\partial y}=2xy+e^{3z},\;\text{(2)}\quad \frac{\partial f}{\partial z}=3ye^{3z}\;\text{(3)} \\
f(x,y,z)=\int y^2dx \\
f(x,y,z)=y^2x+g(y,z) \\
\frac{\partial f}{\partial y}=2xy+g_{y}(y,z) \\
\cancel{2xy}+e^{3z}=\cancel{2xy}+g_{y}(y,z)
\end{gather}$$
		Por lo tanto,
		$$
		\begin{gather}
g_{y}(y,z)=e^{3z}\to \int e^{3z}dy=e^{3z}y+h(z) \\
f(x,y,z)=y^2x-e^{3z}y+h(z) \\
\frac{\partial f}{\partial z}=3e^{3z}y+h'(z) \\
\cancel{3ye^{3z}}=\cancel{3ye^{3z}}+h'(z) \\
h'(z)=0 \Rightarrow h=k
\end{gather}
		$$
		Finalmente $f(x,y,z)=y^2x+e^{3z}y+k$.

---

Aplicación del teorema fundamental de las integrales de línea (**se suele pedir la demostración en el final**)

---
*Ejemplo 4*:
Use el teorema de Green para calcular la siguiente integral de línea:
$$
\oint_{C}(2y+\sqrt{ 9+x^3 })
$$