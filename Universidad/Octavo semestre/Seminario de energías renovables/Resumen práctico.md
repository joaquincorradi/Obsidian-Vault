# Costo nivelado de energía (LCOE)
Permite comparar el costo promedio de producir electricidad durante toda la vida útil de un proyecto. Representa cuánto cuesta generar $1 \ \mathrm{MWh}$ de energía, considerando todos los costos y el total de energía producida en la vida útil del proyecto. Permite comparar diferentes tecnologías en igualdad de condiciones.
$$LCOE=\frac{\mathrm{CAPEX}+\sum^{lsp}_{i=1}\left( \frac{\mathrm{OPEX}}{(1+r)^i} \right)}{\sum^{lsp}_{i=1}\left( \frac{\mathrm{MWh}}{(1+r)^i} \right)}$$
- El numerador suma todos los costos: 
	- $\mathrm{CAPEX}$: inversión inicial
	- $\mathrm{OPEX}$: gastos operativos
- El denominador suma toda la energía producida durante la vida del proyecto.

# Potencia eólica
Cuánta energía puede obtenerse del viento al pasar por un área barrida por las palas del aerogenerador
$$P=\frac{1}{2}\cdot\rho \cdot A \cdot v^3$$
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
El parámetro de forma $k$ determina la forma de la distribución. Cuanto mayor es $k$ (centrada), menor sesgo hacia vientos bajos y mayor probabilidad de velocidades medias/altas y constantes.:
- $k<1$ (lugar con predominio de vientos muy débiles y pocas ráfagas fuertes):
	- La curva está muy sesgada hacia la **izquierda**.
	- Hay muchas probabilidades de vientos bajos.
	- La probabilidad cae rápidamente al aumentar la velocidad.
- $k>1$ (El viento es más estable y predomina una velocidad media-alta):
	- La curva se desplaza hacia la **derecha** y se vuelve más simétrica.
	- Aumenta la probabilidad de vientos moderados o altos.
	- Disminuye la probabilidad de vientos muy bajos.

# Factor de capacidad
Mide qué porcentaje de la potencia máxima instalada realmente se produce durante un período de tiempo, es decir, qué tan aprovechada está la capacidad instalada.
$$FC=\frac{E_{real}}{P_{nominal}\cdot T}=$$
Siendo $T=24\cdot 365=8 760$ para un año.
Si una planta solar tiene FC = 20% → durante un año produce el equivalente al 20% del tiempo a potencia máxima.

Ejemplo: 
