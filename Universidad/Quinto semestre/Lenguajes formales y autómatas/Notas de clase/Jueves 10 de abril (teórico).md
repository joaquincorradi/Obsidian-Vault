## Teorema de Kleene ($ER^\Sigma\equiv AF^\Sigma$)
1. (ida) Si $e\in ER^\Sigma$, entonces $\exists M \in AFN\lambda^\Sigma$ tal que $L(e)=L(M)$.
2. (vuelta) Si $M\in ANF^\Sigma$, entonces $\exists e\in ER^\Sigma$ tal que $L(e)=L(M)$.

### Demostración (1):
Casos base:
	Si $e=\varnothing$, tomamos $M:\rightarrow q_{0}$ y $L(M)=\varnothing=L(\varnothing)=L(e)$.
	Si $e=\lambda$, tomamos $M:\rightarrow q_{0}$ (aceptación) y $L(M)=\{\lambda\}=L(\sigma)=L(e)$.
Casos recursivos:
	Si $e=e_{1}+e_{2}$ con $e_{1}e_{2}\in ER^\Sigma$ tal que $HI\exists M_{1}M_{2}\in AFN\lambda^\Sigma$ tal que $L(M_{1})=L(e_{1})$ tal que podemos tomar $M=(Q,\Sigma,q_{0},F,\Delta)$ tal que,
	$$
	\begin{gather}
Q=Q_{1}\cup Q_{2}\cup\{q_{0}\},\ q_{0}\not\in Q_{1}Q_{2} \\
F=F_{1}\cup F_{2} \\
\Delta=\Delta_{1}\cup \Delta_{2}\cup \{ ((q_{0},\lambda),\{q_{1},q_{2}\}) \}
\end{gather}
	$$
	Claramente $M$ es un $AFN\lambda$ y
	$$L(M)=L(M_{1})\cup L(M_{2})=L(e_{1})\cup L(e_{2})=L(e_{1}+e_{2})=L(e)$$
	Si $e=e_{1},e_{2}$ con $e_{1}e_{2}\in ER^\Sigma$ tal que podemos tomar $M=(Q,\Sigma,q_{0},F,\Delta)$ tal que,
	$$
	\begin{gather}
Q=Q_{1}\cup Q_{2} \\
q_{0}=q_{1} \\
F=F_{2} \\
\Delta=(\Delta_{1}\cup \Delta_{2})-\{ ((q,\lambda),\Delta_{1}(q,\lambda)):q\in F_{1} \}\cup\{ ((q,\lambda),\Delta_{1}(q,\lambda)\cup\{q_{2}\}):q\in F_{1} \} \\
L(M)=L(M_{1}),L(M_{2})=L(e_{1}),L(e_{2})=L(e_{1},e_{2})=L(e)
\end{gather}
	$$
	
### Demostración (2):
Si $e=e_{1}^\star$ con $e_{1}\in ER^\Sigma$ tal que $HI\exists M_{1}M_{2}$ tal que $L(M_{1})=L(e_{1})$ tal que podemos tomar $M=(Q,\Sigma,q_{0},F,\Delta)$ tal que,