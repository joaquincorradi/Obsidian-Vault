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
P=\{ q\to aq':q'\in \Delta(q,a) \}
\end{gather}
	$$