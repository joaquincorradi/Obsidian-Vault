# Integrales de línea (directa y Green)
1. Identificar $P(x,y)$ y $Q(x,y)$. Escribir la integral como$\oint_{C}P(x,y)dx+Q(x,y)dy$.
2. Verificar la orientación de $C$. *“Positivamente orientada”* significa contrarreloj.
- Cálculo directo:
	1. Descomponer la frontera $C$ en tramos suaves $C_{1},C_{2},\dots$
	2. Para cada tramos $C_{i}$:
		1. Elegir una parametrización $\mathbf{r}_{i}(t)=(x_{i}(t),y_{i}(t)),t\in[a_{i},b_{i}]$, recorriendo contrareloj.
		2. Calcular $dx=x'_{i}(t)dt,\ dt=y'_{i}(t)dt$
		3. Sustituir en 
			$$\int_{C_{i}}Pdx+Qdy=\int_{a_{i}}^{b_{i}}[P(x_{i},y_{i})x'_{i}(t)+Q(x_{i},y_{i})y'_{i}(t)]$$
	3. Sumar las integrales de todos los tramos.
- Teorema de Green:
	1. Calcular $\frac{\partial Q}{\partial x}-\frac{\partial P}{\partial y}$.
	2. Describir la región $D$ encerrada por $C$ mediante límites para $x$ e $y$.
	3. Escribir
		$$\oint_{C}Pdx+Qdy=\iint_{D}\left( \frac{\partial D}{\partial x}-\frac{\partial P}{\partial y} \right)dA=\int_{x=x_{min}}^{x_{max}}\int_{y=y_{min}}^{y_{max}}\left( \frac{\partial Q}{\partial x}-\frac{\partial P}{\partial P} \right)dydx$$
	4. Resolver la integral doble

# Optimización con restricción
1. Identificar $f(x,y)$ y la restricción $g(x,y)=0$ 
2. Construir el Lagrangiano: $\mathcal{L}(x,y,\lambda)=f(x,y)-\lambda g(x,y)$.
3. Calcular derivadas parciales:
	- $\frac{\partial \mathcal{L}}{\partial x}=\frac{\partial f}{\partial x}-\lambda \frac{\partial g}{\partial x}$