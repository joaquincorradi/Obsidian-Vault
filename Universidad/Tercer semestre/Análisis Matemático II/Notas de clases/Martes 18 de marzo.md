# Límite y continuidad
### Entorno alrededor de un punto
En el caso de una función de dos variables el entorno es un disco abierto. Todos los puntos que están en el interior del círculo está en el entorno (la distancia entre el centro y el punto debe ser menor al radio $\delta$).
En caso de que el punto central no se tome se lo denomina entorno reducido.
Un punto cualquiera es un punto de acumulación cuando todo entorno reducido del mismo tiene puntos del conjunto. Por eso, puede serlo incluso, si está en la frontera del entorno.
Los campos escalares van de $\mathbb{R}^m \rightarrow \mathbb{R}$, estudiaremos las que van de $\mathbb{R}^2\rightarrow \mathbb{R}$.

### Definición de límite
$x\in \mathbb{R}^m$
$x_{0}=(x_{0}^1, x_{0}^2, \dots,x_{0}^m)$ punto de acumulación del dominio de $f(x):\mathbb{R}^m\rightarrow \mathbb{R}$
$\lim_{ x \to x_{0} }=L\iff\forall\varepsilon>0\exists\delta>0/0<||x-x_{0}||<\delta\implies |f(x)-L|<\varepsilon$

- Desigualdad triangular: La norma de la suma de dos vectores es menor o igual a la suma de las normas de ambos vectores. $||x+y||\leqslant||x||+||y||$
- El valor absoluto de cualquier coordenada de un vector siembre va a ser menor o igual que la norma de ese vector.. Por ejemplo: $x=(1,2)$, $||x||=\sqrt{ 1^2+2^2 }=\sqrt{ 5 }$, $|x_{1}|<\sqrt{ 5 }$, $|x_{2}|<\sqrt{ 5 }$ 
- Desigualdades más usadas en orden de la diapositiva $3, 4, 6, 7$

Verificar un límite por definición es encontrar una relación entre $\varepsilon$ y $\delta$. Debe cumplir la relación que para un $\varepsilon>0$ el $\delta>0$, por ejemplo el caso de $\varepsilon=\sqrt{ 1+\delta }$, ya que $\delta$ puede ser 


