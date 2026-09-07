## Subespacios presentados de forma implícita
$$
\begin{gather}
V=\mathbb{R}^3 \\
W=\{(x,y,z)\mid x+2y+z=0\}=\{(x,y,z)\mid x=-2y-z\}
\end{gather}
$$
1. **Conjunto generador:** como el subespacio ya está caracterizado hay que obtener un conjunto generador:
	$$
	\begin{align}
(-2y-z,y,z)&=(-2y,y,0)+(-z,0,z) \\
&=\alpha(-2,1,0)+\beta(-1,0,1)
\end{align}
	$$
	$$
	\boxed{W=\langle(-2,1,0),(-1,0,1)\rangle}
	$$
2. **Base:**
	$$
	\alpha(-2,1,0)+\beta(-1,0,1)=(0,0,0)
	$$
	 $$
	 \begin{gather}
\left[\begin{array}{@{}cc|c@{}} -2 & -1 & 0 \\ 1 & 0 & 0 \\ 0 & 1 & 0 \end{array}\right] \\
\vdots \\
\left[\begin{array}{@{}cc|c@{}} 1 & 0 & 0 \\ 0 & 1 & 0 \\ 0 & 0 & 0 \end{array}\right]
\end{gather}
	 $$
	 Se puede observar entonces que el conjunto generador hallado ya es **linearmente independiente**, por lo tanto también es una base: 
	 $$
	 \boxed{\mathcal{B}_{W}=\{ (-2,1,0),(-1,0,1) \}}
	 $$
	 $$
	 \boxed{\operatorname{dim}(W)=2}
	 $$
## Subespacios presentados de forma paramétrica
$$
\begin{gather}
V=\mathbb{R}^3 \\
W=\langle (-1,2,-2),(2,-1,-1),(3,-3,1) \rangle=\{ \alpha(-1,2,-2),\beta(2,-1,-1),\gamma(3,-3,1)mid \}
\end{gather}
$$
1. **Caracterizar:** 
	