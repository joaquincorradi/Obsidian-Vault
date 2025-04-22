Ejemplo de...:
$$
\begin{gather}
f(x,y)=x^3+y^3-3x-12y+20 \\
\vec{\nabla}f(x,y)=\overline{0};\ \vec{\nabla}f(x,y)=\left( \frac{\partial f}{\partial x}, \frac{\partial f}{\partial y} \right) \\
\frac{\partial f}{\partial x}=3x^2-3 \\
\frac{\partial f}{\partial y}=3y^2-12 \\
\begin{cases}
3x^2-3=0 \to x=\pm \sqrt{ 1 } \\
3y^2-12=0 \to y=\pm\sqrt{ 4 }
\end{cases} \\
x_{1}=1;\ x_{2}=-1 \\
y_{1}=2;\ y_{2}=-2
\end{gather}
$$
Los puntos críticos obtenidos son
$$
\begin{gather}
\mathbf{x}_{1}=(1,2) \\
\mathbf{x}_{2}=(1,-2) \\
\mathbf{x}_{3}=(-1,2) \\
\mathbf{x}_{4}=(-1,-2)
\end{gather}
$$
El determinante queda
$$
\begin{gather}
\det \mathbf{H}(x,y)=f_{xx}f_{yy}-f_{xy}^2
\begin{cases}
f_{xx}=6x \\
f_{yy}=6y \\
f_{xy}=f_{yx}=0
\end{cases} \\
\det \mathbf{H}(x,y)=6x6y-0^2=36xy
\end{gather}
$$
Entonces,
$$
\begin{gather}
\det \mathbf{H}(1,2)=72>0 \to f_{xx}(1,2)=6>0 \Rightarrow \text{mín} \\
\det \mathbf{H}(1,-2)=-72<0 \Rightarrow \text{silla} \\
\det \mathbf{H}(-1,2)=-72<0 \Rightarrow \text{silla} \\
\det \mathbf{H}(-1,-2)=72>0 \Rightarrow \text{máx}
\end{gather}
$$

Ejemplo 2:
$$
\begin{gather}
f(x,y)=x^3+3xy^2-3x^2-3y^2+4 \\
\vec{\nabla}f(x,y)=0;\ \vec{\nabla}f(x,y)=\left( \frac{\partial f}{\partial x}, \frac{\partial f}{\partial y} \right) \\
\frac{\partial f}{\partial x}=3x^2+3y^2-6x \\
\frac{\partial f}{\partial y}=6xy-6y \\
\begin{cases}
3x^2+3y^2-6x=0 \ \ (1)  \\
6xy-6y=0 \ \ (2)
\end{cases} \\
\text{de} \ (2) \to 6y(x-1)=0 \\
y=0 \\
x=1 \\
\text{en} \ (1) \to \ \text{para} \ y=0 \ \text{se tiene} \\
3x^2-6x=0 \to x(3x-6)=0 \\
x=0 \\
x=2
\end{gather}
$$
Los puntos críticos obtenidos son
$$
\begin{gather}
\mathbf{x}_{1}=(0,0) \\
\mathbf{x}_{2}=(2,0)
\end{gather}
$$
y,
$$
\begin{gather}
\text{en} \ (1) \to \ \text{para} \ x=1 \ \text{se tiene} \\
3x^2-6x=0 \to x(3x-6)=0 \\
x=0 \\
x=2
\end{gather}
$$