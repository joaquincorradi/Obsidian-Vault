# Optimización con restricción
1. Identificar $f(x,y)$ y la restricción $g(x,y)=0$ 
2. Construir el Lagrangiano: $\mathcal{L}(x,y,\lambda)=f(x,y)-\lambda g(x,y)$.
3. Calcular derivadas parciales:
	- $\frac{\partial \mathcal{L}}{\partial x}=\frac{\partial f}{\partial x}-\lambda \frac{\partial g}{\partial x}$
	-  $\frac{\partial \mathcal{L}}{\partial y}=\frac{\partial f}{\partial y}-\lambda \frac{\partial g}{\partial y}$
	-  $\frac{\partial \mathcal{L}}{\partial \lambda}=g(x,y)$
4. Resolver el sistema de ecuaciones:
	$$\begin{cases}
\frac{\partial f}{\partial x}-\lambda \frac{\partial g}{\partial x}=0 \\
\frac{\partial f}{\partial y}-\lambda \frac{\partial g}{\partial y}=0 \\
g(x,y)=0
\end{cases}$$
5. Evaluar $f(x_{i},y_{i})$ en cada solución candidata $(x_{i},y_{i})$.
6. Comparar los valores de $f$para decidir cuáles son máximos y cuáles mínimos.
# Integrales de línea (directa y Green)

1. Calcular $\frac{\partial Q}{\partial x}-\frac{\partial P}{\partial y}$.
2. Describir la región $D$ encerrada por $C$ mediante límites para $x$ e $y$.
3. Escribir
		$$\oint_{C}Pdx+Qdy=\iint_{D}\left( \frac{\partial D}{\partial x}-\frac{\partial P}{\partial y} \right)dA=\int_{x=x_{min}}^{x_{max}}\int_{y=y_{min}}^{y_{max}}\left( \frac{\partial Q}{\partial x}-\frac{\partial P}{\partial P} \right)dydx$$
4. Resolver la integral doble

