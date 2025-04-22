Ejemplo 1:
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
-3+3y^2=0\to y^2=1 \to y=\pm 1 \\
\mathbf{x}_{3}=(1,1) \\
\mathbf{x}_{4}=(1,-1)
\end{gather}
$$
Tenemos,
$$
\begin{gather}
f_{xx}=6x-6,f_{yy}=6x-6,f_{xy}=f_{yx}=6y \\
\det \mathbf{H}(x,y)=f_{xx}f_{yy}-f_{xy}^2=(6x-6)^2-36y^2
\end{gather}
$$
Entonces,
$$
\begin{gather}
\det \mathbf{H}(0,0)=36>0, \ f_{xx}(0,0)=-6 \Rightarrow \text{máx} \\
\det \mathbf{H}(2,0)=36>0, \ f_{xx}(2,0)=6 \Rightarrow \text{mín} \\
\det \mathbf{H}(1,1)=-36<0 \Rightarrow \text{silla} \\
\det \mathbf{H}(1,-1)=-36<0 \Rightarrow \text{silla}
\end{gather}
$$

Ejemplo 3 (de final):
$$
f(x,y)=
\begin{cases}
\frac{xy}{x^2+y^2}, \ & \text{si} \ (x,y)\neq(0,0) \\
0, & \text{si} \ (x,y)=(0,0)
\end{cases}
$$
*a.* Calcular las derivadas parciales en $(0,0)$.
*b.* Analizar las continuidad en $(0,0)$.
*c.* La función ¿es diferenciable en $(0,0)$?
*d.* Dar la derivada direccional en la dirección $\left( \frac{1}{\sqrt{ 2 }}, \frac{1}{\sqrt{ 2 }} \right)$

*a.* Ver condición necesaria
$$
\begin{gather}
\frac{\partial f}{\partial x}(0,0)=\lim_{ t \to 0 } \frac{f(0+t,0)-f(0,0)}{t}=0 \\
\frac{\partial f}{\partial y}(0,0)=\lim_{ t \to 0 } \frac{f(0+t,0)-f(0,0)}{t}=0
\end{gather}
$$
*(Si un límite no es finito la función no es diferenciable, sin embargo todavía no se puede asegurar que lo sea).*
*(Justificar por qué los límites dan cero en el parcial. Puede ser con texto escrito).*
Entonces,
$$
\begin{gather}
f(0,0)=0, \ f(t,0)=\frac{t \cdot 0}{t^2+0^2}=0 \\
f(0,t)=\frac{0 \cdot 0}{0^2+t^2}
\end{gather}
$$
*b.* Usar al menos tres caminos, y en caso de haber un exponente a la cuarta en el denominador se puede usar un ???? para tratar de demostrar que no existe.
$$
\begin{gather}
L_{1}=\lim_{ x \to 0 } \left( \lim_{ y \to 0 } \frac{xy}{x^2+y^2}  \right)=0 \\
L_{2}=\lim_{ y \to 0 } \left( \lim_{ x \to 0 } \frac{xy}{x^2+y^2}  \right)=0 \\
y=mx \to L_{3}=\lim_{ x \to 0 } \frac{x(mx)}{x^2+(mx)^2}=\lim_{ x \to 0 } \frac{mx^2}{x^2(1+m^2)}=\frac{m}{1+m^2}  
\end{gather}
$$
En $L_{3}$ no existe el límite porque depende de $m$ por lo tanto no es continua porque no existe el límite. Al no ser continua no es diferenciable (*c.*)

*d.* Al no ser diferenciable, para calcular la derivada direccional se debe aplicar la definición de derivada direccional, en el caso contrario se usa el gradiente.
$$
\begin{gather}
\frac{\partial f}{\partial \vec{u}}(x_{0},y_{0})=\lim_{ t \to 0 } \frac{f(x_{0}+tu_{1}),f(y_{0}+tu_{2})-f(x_{0},y_{0})}{t}  \\
\frac{\partial f}{\partial \vec{u}}=\lim_{ t \to 0 }\frac{f(0+tu_{1}),f(0+tu_{2})-f(0,0)}{t} \\
 
\end{gather}
$$