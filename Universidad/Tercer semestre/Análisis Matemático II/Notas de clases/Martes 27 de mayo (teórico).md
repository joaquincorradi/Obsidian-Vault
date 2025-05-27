Ejemplo:
1. Determinar si los siguientes campos vectoriales son conservativos. De serlo, determinar la función potencial.
	- $F(x,y)=x^2y\vec{i}+xy\vec{j}$:
		$$\begin{gather}
M(x,y)=x^2y, \quad N(x,y)=xy \\
\frac{\partial M}{\partial y}\stackrel{?}{=}\frac{\partial N}{\partial x} \\
\frac{\partial M}{\partial y}=x^2, \quad \frac{\partial N}{\partial x}=y \\
\frac{\partial M}{\partial y}\neq\frac{\partial N}{\partial x}
\end{gather}$$
		Entonces, el campo F no es conservativo.
	- $G(x,y)(3+2xy)\vec{i}+(x^2-3y^2)\vec{j}$:
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

\end{gather}
		$$

