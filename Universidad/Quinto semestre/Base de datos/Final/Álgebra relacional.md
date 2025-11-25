### Estructura básica
- Relaciones: una relación es una tabla que consta de filas y columnas, que representan datos en un formato estructurado. Cada relación tiene un nombre único y está formada por tuplas.
- Tuplas:  es una sola fila en una relación, que contiene un conjunto de valores para cada atributo. Representa una única entrada o registro de datos en una tabla relacional.
- Valores: componentes de una tupla.
- Atributos: son las columnas de una relación, cada una de las cuales representa una característica o propiedad específica de los datos.
- Dominio: conjunto de valores que puede tomar un atributo.

|        | A1  | A2  |
| ------ | --- | --- |
| **T1** | V1  | V2  |
| **T2** | V1  | V2  |

### Operaciones fundamentales
#### Selección ($\sigma$)
Permite filtrar un subconjunto de tuplas que cumplan una condición $P$ de una relación $R$.
$$\sigma_{P}(R)$$
Por ejemplo $\sigma_{apellido=xy}(alumnos)$ selecciona todas las tuplas que contengan "xy" como apellido en la relación "alumnos".
Una condición puede ser una combinación booleana, donde se pueden usar operadores como $\land$, $\lor$, combinándolos con operadores $<$, $>$, $\leqslant$, $\geqslant$, $=$, $\neq$.
#### Proyección ($\Pi$)
Permite extraer atributos $A_n$ de una relación $R$, dando como resultado un subconjunto vertical de atributos de la relación pero eliminando valores duplicados.
$$\Pi_{A_{n}}(R)$$
Por ejemplo $\Pi_{nombre, apellido}(alumno)$ muestra las columnas nombre y apellido completas sin los duplicados.
#### Unión ($\cup$)
Se utiliza para combinar los resultados de dos consultas en un único resultado. La única condición es que ambas consultas deben devolver el mismo número de columnas con el mismo tipos de datos.
Por ejemplo $R\cup S$ retorna el conjunto de tuplas que están en $R$, o en $S$, o en ambas.
#### Diferencia ($-$)



