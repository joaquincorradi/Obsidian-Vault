## Teorema de Kleene ($ER^\Sigma\equiv AF^\Sigma$)
1. (ida) Si $e\in ER^\Sigma$, entonces $\exists M \in AFN\lambda^\Sigma$ tal que $L(e)=L(M)$.
2. (vuelta) Si $M\in ANF^\Sigma$, entonces $\exists e\in ER^\Sigma$ tal que $L(e)=L(M)$.

### Demostración (1):
Casos base:
	Si $e=\varnothing$, tomamos $M:\rightarrow q_{0}$ y $L(M)=\varnothing=L(\varnothing)=L(e)$.
	Si $e=\lambda$, tomamos $M:\rightarrow q_{0}$ (aceptación) y $L(M)=\{\lambda\}=L(\sigma)=L(e)$.
Casos recursivos:
	Si $e=e_{1}+e_{2}$ con $e_{1}e_{2}\in ER^\Sigma$ tal que
