Definición: una gramática regular de paso único (GRPU) es una gramática tal que todas sus producciones son de la forma:
$$
\begin{gather}
A\longrightarrow \alpha B \\
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
	Si $A\longrightarrow$