# Conceptos topológicos
Los puntos van a ser n-uplas (vectores) de números reales.
A cada punto del espacio se le puede asignar un vector que parte desde le origen coordenadas.
El conjunto de dominios es N y el conjuntos de llegadas es P:
- n=1 y p=1 la función se denomina función escalar de variable real, por ejemplo $y=f(x)$
- n=1 y p > 1 la función se denomina función  vectorial de variable real, por ejemplo $f(t)=f_{1}(t), f_{2}(t),m f_{3}(t)$ y va de r en r3
- n>1 y p=1 la función se denomina campo escalar, por ejemplo $f(t)=(2t^2, 3t, e^t)$
- n>1 y p>1 la función se denomina campo vectorial.
$F(x,y)=(3x^2y, 2xy)$ va de r2 en r2
$F(x,y,z)=(zxy^2, 3hx, 3zxy)$ va de r3 en r3

- Distancia: el concepto de distancia es similar al de la recta real en donde se definía como el valor absoluto: $d(p,q)=|q-p|$. A partir de R3 se define como la norma o módulo del vector, es decir, su valor numérico.  Ahora se calcula a partir de la raíz de los catetos al cuadrados.
- Conjunto abierto: el disco abierto de radio $r$ y de centro $x_0$ denotado como $B_r(x_0)=||x-x_0|| < r$.
Se puede graficar siempre que $m+m\leqslant3$ ($R^m\rightarrow R^m$)

# Dominio e imagen de una función
Dominio son todos aquellos valores que pertenecen al conjunto de partida que hacen que la función tenga sentido. Para determinar el dominio de la función es más fácil a veces encontrar los puntos que no pertencen:
Por ejemplo:
Determinar el dominio y la imagen de la siguiente función.
$f:R^2\rightarrow R$ se puede graficar el domino porque estoy en R2 y se puede graficar la función
$f(x,y)=\sqrt{25-x^2-y^{2}}$
Para que se cumpla la función $25-x^2-y^{2}\geqslant_{0}$
Entonces $Dom_{f}=\{ (x,y)\in R / x^2+y^2 \leqslant 25 \}$
La ecuación de un circulo es $x^2+y^2 \leqslant a^2$ 
La imagen de la función es $\mathrm{Im}_{f} = [0,5]$ 

Otro ejemplo:
$h:R^2\rightarrow R^3$ No se puede graficar la función porque m+m es mayor a 3
$h(x,y)=(\sqrt{ 1-x^2-y^2 }, 0, 1)$ la coordenada que cambia es la $h_1$, 
Para definir el dominio de una función de tres coordenadas que son tres funciones se debe buscar la intersección de los tres dominios. En este caso dos coordenadas son fijas.
$Dom_{h}(x,y)=Dom_{f}(x,y)$ 
$Dom_{f}(x,y)=\{(x,y)\in R /x^2+y^2 \leqslant 1\}$
$\mathrm{Im}_{f(x,y)} =\{ (x,y,z)\in R^3 / 0\leqslant x \leqslant 1, y=0 \land z=1 \}$ 

# Representación gráfica de funciones
Las gráficas de funciones de dos variables siempre van a ser superficies. 
Por ejemplo $f(x,y)=x^2+y^2$ es un paraboloide.

Una curva de nivel se obtiene igualando a la función en un valor constante $x=C$ para el caso de $R^2$.  $x=C$ es un plano paralelo. Con esto uno puede tener información de la función.

# Límites

