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
$$(D_{e_{i}})(x)=\lim_{ t \to 0 } \frac{1}{t}(f(x_{1},x_{2},\dots,x_{i}+t))$$