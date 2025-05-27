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
\vec{\nabla}\times\mathbb{F}=\left( \frac{\partial R}{\partial y}-\frac{\partial Q}{\partial z} \right)\vec{i}+\left( \frac{\partial P}{\partial z}-\frac{\partial R}{\partial x} \right)\vec{j}+\left( \frac{\partial Q}{\partial x}-\frac{\partial P}{\partial y} \right)\vec{k}
\end{gather}
	$$
	- $\mathbb{F}(x,y,z)=(x^3y,\ 3z+x,\ y+z)$
		$$
		\vec{\nabla}\times\mathbb{F}=(1-3)\vec{i}+(0-0)\vec{j}+(1-x^3)\vec{k}
		$$