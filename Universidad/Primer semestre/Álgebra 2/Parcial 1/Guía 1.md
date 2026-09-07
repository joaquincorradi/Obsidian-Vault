## El punto de la recta $L$ más próximo al punto $P$
$$
\begin{gather}
P=(2,-1,3) \\
L:\frac{x}{2}=\frac{y+2}{-2}=z+2
\end{gather}
$$
1. Pasar la recta $L$ a la ecuación vectorial y paramétricas y obtener el vector director $\vec{v}$:
$$L:
\begin{cases}
x=2t \\ y=-2-2t \\ z=-2+t
\end{cases}
$$
$$
L:(x,y,z)=(0,-2,-2)+t(2,-2,1)
$$
$$
\vec{v}=(2,-2,1)
$$
2. Construir un plano $\pi$ perpendicular a la recta $L$ que contiene al punto $P$. El vector normal $\vec{n}$ de $\pi$ va ser el vector $\vec{v}$:
$$
\begin{align}
\pi:Ax+By+Cz&=D \\
2x-2y+z&=D \\
\end{align}
$$
	Reemplazar $x$, $y$ y $z$ por el punto $P$:
	$$
	2(2)-2(-1)+(3)=D=9
	$$
	Y así obtenemos el plano $\pi$:
	$$
	\pi:2x-2y+z=9
	$$
3. Calcular la intersección entre el plano $\pi$ y la recta $L$ que será el punto $Q$:
	Reemplazar $x$, $y$ y $z$ por los valores de las ecuaciones paramétricas de la recta $L$:
	$$
	\begin{align}
2(2t)-2(-2-2t)+(-2+t)&=9 \\
t&=\frac{7}{9}
\end{align}
	$$
	Reemplazo el valor de $t$ en las ecuaciones paramétrica de $L$:
	$$
	\begin{cases}
x=2\left( \frac{7}{9} \right)=\frac{14}{9} \\
y=-2-2\left( \frac{7}{9} \right)=-\frac{32}{9} \\
z=-2+\left( \frac{7}{9} \right)=-\frac{11}{9}
\end{cases}
	$$
	$$
	\boxed{Q=\left( \frac{14}{9},-\frac{32}{9},-\frac{11}{9} \right)}
	$$
4. Calcular la distancia entre el punto $P$ y la recta $L$:
	$$
	\begin{align}
\operatorname{dist}(P,L)&=\operatorname{dist}(P,Q) \\
&=\sqrt{ \left( 2-\frac{14}{9} \right)^2+\left( -1+\frac{32}{9} \right)^2+\left( 3+\frac{11}{9} \right)^2 }
\end{align}
	$$
	$$
	\boxed{\operatorname{dist}(P,L)=\operatorname{dist}(P,Q)=\frac{\sqrt{ 221 }}{3}\ \mathrm{u}\approx 4,96\ \mathrm{u}}
	$$
## El punto del plano $\pi$ más próximo al punto $P$
$$
\begin{gather}
P=(1,1,1) \\
\pi:2x-y+z=0
\end{gather}
$$
1. Obtener el vector $\vec{n}$ del plano $\pi$:
	$$
	\vec{n}=(2,-1,1)
	$$
2. Construir una recta $L$ perpendicular al plano $\pi$ que contiene al punto $P$. El vector normal $\vec{n}$ de $\pi$ va a ser igual al vector director $\vec{v}$ de la recta $L$:
	$$
	L:(x,y,z)=(1,1,1)+t(2,-1,1)
	$$
	$$
	L:
	\begin{cases}
x=1+2t \\
y=1-t \\
z=1+t
\end{cases}
	$$
3. Calcular la intersección entre el plano $\pi$ y la recta $L$ que será el punto $Q$:
	Reemplazar $x$, $y$ y $z$ por los valores de las ecuaciones paramétricas de la recta $L$:
	$$
	\begin{align}
2(1+2t)-(1-t)+(1+t)&=0 \\
t&=-\frac{1}{3}
\end{align}
	$$
	Reemplazo el valor de $t$ en las ecuaciones paramétrica de $L$:
	$$
	\begin{cases}
x=1+2\left( \frac{1}{3} \right)=\frac{1}{3} \\
y=1-\left( \frac{1}{3} \right)=\frac{4}{3} \\
z=1+\left( \frac{1}{3} \right)=\frac{2}{3}
\end{cases}
	$$
	$$
	\boxed{Q=\left( \frac{1}{3}, \frac{4}{3}, \frac{2}{3} \right)}
	$$
4. Calcular la distancia entre el punto $P$ y el plano $\pi$:
	$$
	\begin{align}
\operatorname{dist}(P,\pi)&=\operatorname{dist}(P,Q) \\
&=\sqrt{ \left( 1-\frac{1}{3} \right)^2+\left( 1-\frac{4}{3} \right)^2+\left( 1-\frac{2}{3} \right)^2 }
\end{align}
	$$
	$$
	\boxed{\operatorname{dist}(P,\pi)=\operatorname{dist}(P,Q)=\frac{\sqrt{ 6 }}{3}\ \mathrm{u}\approx 0,82\ \mathrm{u}}
	$$
## Ángulo entre vectores
$$
\begin{align}
\cos(\theta)&=\frac{\vec{u}\cdot \vec{v}}{\lvert \vec{u} \rvert\lvert \vec{v} \rvert} \\
\theta&=\arccos\left( \frac{\vec{u}\cdot \vec{v}}{\lvert \vec{u} \rvert\lvert \vec{v} \rvert} \right)
\end{align}
$$

## Ángulo agudo entre rectas
$$
\begin{align}
\cos(\theta)&=\frac{\lvert\vec{u}\cdot \vec{v}\rvert}{\lvert \vec{u} \rvert\lvert \vec{v} \rvert} \\
\theta&=\arccos\left( \frac{\lvert\vec{u}\cdot \vec{v}\rvert}{\lvert \vec{u} \rvert\lvert \vec{v} \rvert} \right)
\end{align}
$$
