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
1. Normalizar el vector dirección $\mathbf{u}$ para convertirlo en vector unitario (con módulo $1$):
	$$\hat{\mathbf{u}}=\frac{\mathbf{u}}{\|\mathbf{u}\|} \ \text{con} \ \|\mathbf{u}\|=\sqrt{ u_{1}^2+u_{2}^2+\dots+u_{k}^2 }$$
2. Calcular las derivadas parciales de $f$.
3. Calcular el gradiente en el punto $x_{0}$ dado por:
	$$$$