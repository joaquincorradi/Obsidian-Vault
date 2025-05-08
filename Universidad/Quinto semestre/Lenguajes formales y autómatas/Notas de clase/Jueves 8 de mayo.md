Definición: una gramática regular de paso único (GRPU) es una gramática tal que todas sus producciones son de la forma:
$$
\begin{gather}
A\longrightarrow aB \\
A\longrightarrow B \ \ \text{con} \ A,B\in V \ \text{y} \ \alpha\in\Sigma \\
A\longrightarrow \lambda
\end{gather}
$$
$$
GRPU^\Sigma=\{ G:G \ \text{es} \ GRPU \ \text{con símbolos terminales} \ \Sigma \}
$$
Teorema ($GR^\Sigma\equiv GRPU^\Sigma$)
1. (ida) Si $G\in GRPU^\Sigma$, entonces $\exists G'\in GR^\Sigma$ tal que $L(G')\equiv L(G)$.
	No requiere demostración ya que es trivial, una $GRPU$ es una $GR$.
2. (vuelta) Si $G\in GR^\Sigma$, entonces $\exists G'\in GRPU^\Sigma$ tal que $L(G')\equiv L(G)$.
	Si $(A\longrightarrow a_{1},\dots,a_{n}B)\in P$ con $k\geqslant 2$, hacemos en $P'$:
	$$\begin{gather}
	A\longrightarrow B_{1} \\
	B_{1}\longrightarrow a_{1}B_{1} \\
	B_{2}\longrightarrow a_{2}B_{2} \\
	\vdots \\
	B_{k}\longrightarrow a_{k}B
	\end{gather}$$
	Si $(A\longrightarrow a_{1},\dots,a_{k})\in P$ con $k\geqslant 1$:
	$$
\begin{gather}
A\longrightarrow B_{1} \\
B_{1}\longrightarrow a_{1}B_{1} \\
B_{2}\longrightarrow a_{2}B_{2} \\
\vdots \\
B_{k}\longrightarrow a_{k}B_{k+1} \\
B_{k+1}\longrightarrow \lambda
\end{gather}
	$$

Un lenguaje es regular si es generado por una $GR$.

Teorema ($GRPU^\Sigma\equiv AFN\lambda^\Sigma$):
1. (ida) Si $G\in GRPU^\Sigma$, entonces $\exists M\in AFN\lambda^\Sigma$ tal que $L(G)\equiv L(M)$.
	Sea $G=(V,\Sigma,P,S)$, entonces tomamos $M=(Q,\Sigma,q_{0},F,\Delta)$ con:
	$$
	\begin{gather}
Q=V \\
q_{0}=S \\
F=\{ A\in V:(A\to \lambda)\in P \} \\
\Delta(A,a)=\{ B\in V:(A\to aB)\in P \} \\
\Delta(A,\lambda)=\{ B\in V:(A\to B)\in P \}
\end{gather}
	$$
2. (vuelta) Si $G\in AFN\lambda^\Sigma$, entonces $\exists G\in GRPU^\Sigma$ tal que $L(M)\equiv L(G)$.
	Sea $M=(Q,\Sigma,q_{0},F,\Delta)$, entonces tomamos $G=(V,\Sigma,P,S)$ tal que:
	$$
	\begin{gather}
V=Q \\
S=q_{0} \\
P=\{ q\to aq':q'\in \Delta(q,a) \}\cup \{ q\to q':q'\in \Delta(q,\lambda) \}\cup\{ q\to \lambda:q\in F \}
\end{gather}
	$$

---
# Lenguajes no regulares

Ejemplo de lenguaje no regular:
$$
\begin{gather}
\Sigma=\{ a,b \} \\
L_{1}=\{ a^mb^m:m\geqslant 0 \}\not\in LR^\Sigma \ \text{y} \ \neq a^\star b^\star
\end{gather}
$$
*En este caso necesita memoria.*
Otros ejemplo (palíndromos, espejos):
$$
\begin{gather}
L_{2}=\{ \alpha \in \Sigma^\star:\alpha=\alpha^R \}\not\in LR^\Sigma \\
L_{3}=\{ \alpha \alpha:\alpha\in \Sigma^\star \} \not\in LR^\Sigma
\end{gather}
$$
## Propiedades
Lema *pumping*: $\forall L\in LR^\Sigma$, $\exists n\in \mathbb{N}$, llamada constante de bombeo, tal que si $\alpha\in L$ con $|\alpha|\geqslant h$ entonces $\alpha$ se puede descomponer de la siguiente manera: $\alpha=\alpha_{1},\alpha_{2},\alpha_{3}$ tal que:
1. $|\alpha_{1}\alpha_{2}|\neq h$
2. $\alpha_{2}\neq \lambda$
3. $\alpha_{1},\alpha_{2},\alpha_{3}\in L:\forall i \geqslant 0$

Demostración *pumping*: si $L\in LR^\Sigma$ tal que $\exists M=(Q,\Sigma,q_{0},F,\delta)AFD$ tal que $L(M)=L$, y sea $h=|Q|$. Si $\alpha\in L$ y $\alpha\geqslant h$, entonces existe un estado que es visitado dos veces. Sea $q$ ??? un estado repetitivo. Por lo tanto, $\alpha$ se puede descomponer en la cinta de entrada de siguiente manera...


Para probar que $L\not\in LR^\Sigma$, hacemos:
1. Suponemos $L\in LR^\Sigma$ y sea $