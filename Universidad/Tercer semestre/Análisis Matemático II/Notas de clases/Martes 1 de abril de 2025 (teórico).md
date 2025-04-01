## Diferenciación
En dos variables, se llama funciones diferenciable en un punto cuando, cerca de ese punto, yo podía reemplazar a la función por una recta aproximante llamada recta tangente.
Entonces, podemos decir, que la recta tangete es una buena aproximación de la función en el punto.
Si la recta tangente existe la función es diferenciable.
Buena aproximación significa 

**Condición de diferenciabilidad:**
$\lim_{ x \to a }\frac{f(x)-(f(x_{0})+f'(x_{0})(x-x_{0}))}{(x-a)}=0$
Si el límite da cero la función es diferenciable en el punto $a$.

Si se toma un punto culaquiera en una superfice se puede tomar un punto y crear un plano tangente.

Matriz jacobiana. 
$\mathbf{J}_{f}=\begin{bmatrix} \frac{\partial f}{\partial x}(x_{0},y_{0}) & \frac{\partial f}{\partial y}(x_{0},y_{0}) \end{bmatrix}$

**Se pide en el final demostrar que si una función es diferenciable entonces continua.**

El límite se usa cuando las derivadas parciales no sean continuas, ya que si lo son, entonces es diferenciable y es suficiente para saberlo.

Ejemplo:
$f(x,y)=\begin{cases}\frac{x^2y}{x^2+y^2} & \text{si} (x,y) \neq (0,0) \\ 0 & \text{si} (x,y) = (0,0)\end{cases}$
$\\lim_{ (x,y) \to (0,0) } \frac{f(x,y)-f(x_{0}, y_{0})-\mathbf{D}_{(0,0)}f(x-x_{0},y-y_{0})}{\sqrt{ x^2+y^2 }}$
$\lim_{ (x,y) \to (0,0) }=\frac{\frac{x^2y}{x^2+y^2}-0- \begin{bmatrix} 0 & 0 \end{bmatrix} \begin{bmatrix} x-0 \\ y-0 \end{bmatrix}}{\sqrt{ x^2+y^2 }}$
$\dots$

## Derivada direccional
