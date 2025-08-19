# Diferenciación
$F:\mathbb{R}^n\to \mathbb{R}^m,V\in T_{x}(\mathbb{R}^n)$ y $(D_{V}F)(x)=\lim_{ t \to 0 } \frac{1}{t}(F(x+tv)-F(x))$
$(D_{V}F)(x)=(dF)(V)$

### Propiedades de $D_{V}F$
1. $D_{V}(F+G)=D_{V}F+D_{V}G$
2. $D_{V_{1}+V_{2}}F=D_{V_{1}}F+D_{V_{2}}F$
3. $D_{V}(F\times G)=(D_{V}F)G+F(D_{V}G)$
4. $D_{V}(F\times G)=(D_{V}F)\times G+F\times(D_{V}G)$
5. $D_{fV}F=fD_{V}F \ \ (f:\mathbb{R}^n\to\mathbb{R})$
6. $\left( D_{V} \frac{1}{f}F \right) \frac{1}{f^2}((D_{V}F)f-(D_{V}f)F) \ \ (f:\mathbb{R}^n\to \mathbb{R})$
7. $D_{V}f^g$

### Derivadas parciales
Tenemos una función $f:\mathbb{R}^n \to \mathbb{R}$ y $B={e_{11}, e_{2},\dots,e_{n}}$ la base canónica de $\mathbb{R}^n$
$$(D_{e_{i}})(x)=\lim_{ t \to 0 } \frac{1}{t}(f(x_{1},x_{2},\dots,x_{i}+t,\dots,x_{n})-f(x_{1,x_{2},\dots,x_{n}}))=\lim_{ t \to 0 } \frac{f(x_{i})}{}$$
Este límite, cuando existe, se denomina derivada parcial de $f$ respecto de la variable $x$, en el punto $\mathbf{x}=(x_{1},x_{2},\dots)$ y la denotaremos $\frac{\partial f}{\partial x_{i}}$.

Sea $f:\mathbb{R}^n \to \mathbb{R}^m$, esto es, $F=(F_{1},F_{2},\dots)$ y sea $F$ diferenciable, entonces la aplicación lineal de F $(dF)_{x}(V)=(D_{V})F(x)$ para todo $\mathbf{x}\in D(F)$.
Sean $B=\{e_{1},e_{2\},\dots}$ y $B'=\{ \tilde{e}_{1},\tilde{e}_{2},\dots \}$ las bases canónicas de $\mathbf{R}^n$ y $\mathbf{R}^m$ respectivamente, entonces $F=\sum_{i=1}^mF_{i}\tilde{e}_{i}$, de modo que $(dF)_{x}(e_{j})=(D_{e_{j}}F)(\mathbf{x})=\left( D_{e_{j}}\left( \sum_{i=1}^m F_{i}\tilde{e_{i}} \right) \right)(\mathbf{x})$ esto es igual a $\sum_{i=1}^m D_{e_{j}}F_{i}\tilde{e_{i}}(\mathbf{x})=\sum_{i=1}^m(D_{e_{j}}F_{i})(\mathbf{x})\tilde{e}_{i}+\sum_{i=1}^m F_{i}(x)(D_{e_{j}})(x)=\sum_{i=1}^m \frac{\partial F_{i}}{\partial x_{i}}$, ($D_{e_{j}}\tilde{e}_{i}=0$ ya que $\tilde{e}_{i}$ es constante).
Esto indica que la matriz con entradas $\frac{\partial F_{i}}{\partial x_{j}}(x)$ es la matriz de $(dF)_{\mathbf{x}}$ respecto de las bases canónicas de $\mathbf{R}^n$ y $\mathbf{R}^m$ respectivamente. Dicha matriz se denomina jacobiana y la denotamos $J_{F}$, esto es $e_{ij}(J_{F})=\frac{\partial F_{i}}{\partial x_{j}}$.

### Regla de la cadena
**Teorema (regla de la cadena)**: sean $F:\mathbf{R}^n\to \mathbf{R}^m$y $G:\mathbf{R}^m\to \mathbf{R}^p$ tal que $Im(F)\subset D(G)$ y asumimos que $F$ y $G$ son diferenciables. Entonces $G\circ F$ es diferenciables y 

**Demostración**: sea $\mathbf{x}\in D(F)$ y $h\neq 0$, entonces $(G\circ F)(\mathbf{x}+h)=G(F(\mathbf{x}+h))=G(F(\mathbf{x})+(dF)_{\mathbf{x}})(h)+\varphi_{x}(h)$; si $F(x)=y$ y $(dF)_{x}(h)+\varphi_{x}(h)=k$, tenemos $(G\circ F)(\mathbf{x}+h)=G(y+k)=G(y)+(dG)_{y}(k)+\alpha_{y}(k)=G(F(x))+(dG)_{y}()$ 