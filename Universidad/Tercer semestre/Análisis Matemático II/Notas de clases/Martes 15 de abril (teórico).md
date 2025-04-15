# Extremos de funciones de varias variables
### Máximo
$$
\begin{gather}
f(x_{0}+\Delta x)-f(x_{0})<0\to \Delta f<0 \\
f(x)=f(x_{0})+\frac{1}{1!}f'(x_{0})(x-x_{0})+\frac{1}{2!}f''(x_{0})^2+\frac{1}{3!}f'''(x_{0})(x-x_{0})^3+\dots +\frac{1}{m!}f^n(x_{0})(x-x_{0})^m+R_{n} \\
\Delta f=f(x)-f(x_{0})=f'(x_{0})(x-x_{0})+\frac{1}{2!}f''(x_{0})(x-x_{0})^2+\dots
\end{gather}
$$
### Mínimo
$$
\begin{gather}
f(x_{0}+\Delta x)-f(x_{0})>0\to \Delta f>0 \\
\Delta f=f(x)-f(x_{0})=f'(x_{0})(x-x_{0})+\frac{1}{2!}f''(x_{0})(x-x_{0})^2+\dots
\end{gather}
$$

Si la primer derivada no nula es de orden par y negativa hay máximo, en cambio, si la primer derivada es de orden par y positiva tengo un mínimo. 

$$
\begin{gather}
f(x,y)=f(x,y)+\frac{1}{1!}\left[ \frac{\partial f}{\partial x}(x_{0},y_{0})(x-x_{0})+\frac{\partial f}{\partial y}(x_{0},y_{0})(y-y_{0}) \right]+ \\
+\frac{1}{2!}\left[ \frac{\partial ^2 f}{\partial x^2}(x_{0},y_{0})(x-x_{0})^2+\frac{\partial ^2 f}{\partial x \partial y}(x_{0},y_{0})(y-y_{0})+\frac{\partial ^2 f}{\partial y}(x_{0},y_{0})(y-y_{0})^2+\dots \right]
\end{gather}
$$

Condición necesaria para la existencia de extremos:
$$
\begin{gather}
\vec{\nabla}f(x_{0},y_{0})=\overline{0} \\
\frac{\partial f}{\partial x}=0,\ \frac{\partial f}{\partial y}=0
\end{gather}
$$
En funciones de varias variables se le llama máximo o mínimo locales cuando es en un sólo punto.

- Teorema (condición necesaria para la existencia de extremos) (**final**)