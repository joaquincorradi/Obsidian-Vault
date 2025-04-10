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
Si $e=e_{1}^\star$ con $e_{1}\in ER^\Sigma$ tal que $HI\exists M_{1}=(Q_{1}, \Sigma, q_{1}, F_{1},\Delta_{1})AFN?$ tal que $L(M_{1})=L(e_{1})$ tal que podemos tomar $M=(Q,\Sigma,q_{0},F,\Delta)$ tal que,
$$
\begin{gather}
Q=Q_{1}\cup\{q_{0}\},\ q_{0}\not\in Q_{1} \\
F=F_{1}\cup\{q_{0}\} \\
\Delta=\Delta_{1}-\{((q,\lambda),\Delta_{1}(q,\lambda)):q\in F_{1}\}\cup \{((q,\lambda),\Delta_{1}(q,\lambda)\cup \{q_{0}\}):q\in F_{1}\}\cup\{((q,\lambda),\{q_{1}\})\}
\end{gather}
$$
Claramente $M$ es un $AFN\lambda$ y $L(M)=(L(M_{1}))^\star=(L(e_{1}))^\star=L_{e}$

*Foto ejemplo*

### Demostración (2):
Sea $M=(Q,\Sigma,q_{0},F,\Delta)$ con $Q=\{q_{0},\dots,q_{n}\}$, entonces  ref????? $M_{i}=(Q,\Sigma,q_{i},F,\Delta)$ con $i=0,\dots,n$ y $L(M_{i})=X_{i}$ y $X_{0}=L(M)$.
Notar que cada $X_{i}$ se puede escribir de la siguiente manera,
$$
X_{i}=
\begin{cases}
\sum_{q_{i}\in \Delta(q,a)}aX_{i},\ q_{i}\not\in F \\
\sum_{q_{i}\in \Delta(q,a)}aX_{i}+\lambda,\ q_{i}\in F
\end{cases}
$$
Entonces tenemos un sistema de $n+1$ ecuaciones y $n+1$ incógnitas.
- Lema Ardon: si $A,B\subseteq \Sigma^\star$ 

