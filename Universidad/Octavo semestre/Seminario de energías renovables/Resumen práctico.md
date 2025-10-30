# Costo nivelado de energía (LCOE)
Permite comparar el costo promedio de producir electricidad durante toda la vida útil de un proyecto. Representa cuánto cuesta generar $1 \ \mathrm{MWh}$ de energía, considerando todos los costos y el total de energía producida en la vida útil del proyecto. Permite comparar diferentes tecnologías en igualdad de condiciones.
$$\mathrm{LCOE}=\frac{\mathrm{CAPEX}+\sum^{lsp}_{i=1}\left( \frac{\mathrm{OPEX}}{(1+r)^i} \right)}{\sum^{lsp}_{i=1}\left( \frac{\mathrm{MWh}}{(1+r)^i} \right)}$$
- El numerador suma todos los costos: 
	- $\mathrm{CAPEX}$: inversión inicial
	- $\mathrm{OPEX}$: gastos operativos
- El denominador suma toda la energía producida durante la vida del proyecto.

# Potencia eólica
Cuánta energía puede obtenerse del viento al pasar por un área barrida por las palas del aerogenerador
$$P=\frac{1}{2}\rho Av^3$$
Siendo:
- $P$: potencia del viento en $\mathrm{w}$.
- $\rho$: densidad del aire en $\frac{kg}{m^3}$.
- $A$: área barrida por las palas en $\mathrm{m}^2$ ($\pi R_{rotor}^2$).
- Velocidad del viento en $\mathrm{\frac{m}{s}}$.

Cuanto mayor es el área del rotor y la velocidad del viento, más energía puede generar el aerogenerador.

# Límite de Betz
Establece el máximo teórico de eficiencia para un aerogenerador. Un aerogenerador no puede capturar más del $59,3\%$ de la energía cinética del viento.

# Distribución de Weibull
Permite representar cómo se distribuyen las velocidades del viento en un lugar determinado durante un período.
El parámetro de forma $k$ determina la forma de la distribución:
- $k<1$ (lugar con predominio de vientos muy débiles y pocas ráfagas fuertes):
	- La curva está muy sesgada hacia la izquierda.
	- Hay muchas probabilidades de vientos bajos.
	- La probabilidad cae rápidamente al aumentar la velocidad.