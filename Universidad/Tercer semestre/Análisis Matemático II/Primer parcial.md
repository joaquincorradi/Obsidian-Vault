# Regla de la cadena y composición
1. Identificar las funciones y sus dimensiones: 
	$$\vec{g}:\mathbb{R}^n\to\mathbb{R}^m,\ \vec{f}:\mathbb{R}^m\to \mathbb{R}^p\Rightarrow \vec{f}\circ \vec{g}:\mathbb{R}^n\to \mathbb{R}^p$$
2. Calcular la matriz jacobiana de $\vec{g}$, $\mathbf{J}_{\vec{g}}(\mathbf{x})$, una matriz $(m\times n)$.
3. Calcular la matriz jacobiana de $\vec{f}$, $\mathbf{J}_{\vec{f}}(\mathbf{u})$, una matriz $(p\times m)$.
4. Evaluar $\vec{g}$ en el punto dado $\mathbf{x_{0}}$, $\vec{g}(\mathbf{x_{0}})=(\mathbf{u_{0}})$ y evaluar luego $\mathbf{J}_{\vec{g}}(\mathbf{x_{0}})$.
5. Evaluar $\vec{f}$ en el punto $\vec{g}(\mathbf{x_{0}})=(\mathbf{u_{0}})$, y evaluar luego $\mathbf{J}_{\vec{f}}(\vec{g}(\mathbf{x_{0}}))=\mathbf{J}_{\vec{f}}(\mathbf{u_{0}})$.
6. Multiplicar las dos matrices:
	$$\mathbf{J}_{\vec{f}\circ \vec{g}}(\mathbf{x_{0}})=\mathbf{J}_{\vec{f}}(\vec{g}(\mathbf{x_{0}}))\times \mathbf{J}_{\vec{g}}(\mathbf{x_{0}})$$
# Derivada direccional
1. Normalizar el vector dirección $\mathbf{v}$ para convertirlo en vector unitario (con módulo $1$):
	$$\hat{\mathbf{u}}=\frac{\mathbf{v}}{\|\mathbf{v}\|} \ \text{con} \ \|\mathbf{v}\|=\sqrt{ v_{1}^2+v_{2}^2+\dots+v_{k}^2 }$$
2. Calcular las derivadas parciales de $f$.
3. Calcular el gradiente en el punto $x_{0}$ dado por:
	$$\nabla f(\mathbf{x_{0}})=\left( \frac{\partial f}{\partial x_{i}}(\mathbf{x_{0}}),\dots,\frac{\partial f}{\partial n_{i}}(\mathbf{x_{0}}) \right)$$
4. Calcular la derivada haciendo el producto punto:
	$$\mathbf{D}_{\mathbf{\hat{u}}}f(\mathbf{x_{0}})=\nabla f(\mathbf{x_{0}})\cdot\hat{\mathbf{u}}$$
5. Interpretar el resultado:
	- Si $\mathbf{D}_{\mathbf{\hat{u}}}f(\mathbf{x_{0}})>0$ entonces: en el punto $\mathbf{x_{0}}$ la función $f$ crece a razón de $\mathbf{D}_{\mathbf{\hat{u}}}f(\mathbf{x_{0}})$ unidades por cada unidad que se avanza en la dirección del vector $\mathbf{v}$.
	-  Si $\mathbf{D}_{\mathbf{\hat{u}}}f(\mathbf{x_{0}})<0$ entonces: en el punto $\mathbf{x_{0}}$ la función $f$ decrece a razón de $\mathbf{D}_{\mathbf{\hat{u}}}f(\mathbf{x_{0}})$ unidades por cada unidad que se avanza en la dirección del vector $\mathbf{v}$.
# Extremos
1. Calcular las derivadas parciales.
2. Encontrar los puntos críticos resolviendo el sistema de ecuaciones, siendo cada solución un punto crítico:
	$$
	\begin{cases}
\frac{\partial f}{\partial x}=0 \\
\frac{\partial f}{\partial y}=0
\end{cases}
	$$
3. Calcular las derivadas segundas:
	$$\frac{\partial^2f}{\partial x^2},\ \frac{\partial^2f}{\partial y^2},\ \frac{\partial^2f}{\partial x\partial y}$$
4. Formar la matriz hessiana:
	$$\mathbf{H}_{f}=
	\begin{bmatrix}
\frac{\partial^2f}{\partial x^2} & \frac{\partial^2f}{\partial x\partial y} \\
\frac{\partial^2f}{\partial y\partial x} & \frac{\partial^2f}{\partial y^2}
\end{bmatrix}
	$$
5. 
