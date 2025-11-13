Es un lenguaje estructurado de consultas utilizado para administrar y manipular bases de datos relacionales.
### Componentes
#### LDD: lenguaje de definición de datos
Es un subconjunto que proporciona comandos para la **definición**, **borrado**, **modificación** de relaciones. Su propósito es establecer cómo se organizan los datos, sin manipular el contenido en sí.
#### LMD: lenguaje de manipulación de datos
Es un subconjunto del lenguaje utilizado para **manipular** los datos almacenados en una base de datos relacional. Se centra en la gestión del contenido, es decir, los registros o filas dentro de las tablas. Sus comando principales son:
- SELECT: sirve para **consultar** y **recuperar** datos de una o más tablas en una base de datos. Permite especificar qué columnas deseas obtener, filtrar resultados, ordenarlos y combinar datos de múltiples tablas. (debe tener el `FROM` o `WHERE` para no ser DQL). Ejemplo: `SELECT nombre, edad FROM usuarios WHERE edad > 18;`
- INSERT: **añade** nuevos registros a una tabla. Ejemplo: `INSERT INTO usuarios (nombre, edad) VALUES ('Ana', 30);`
- UPDATE: **modifica** registros existentes en una tabla. Ejemplo: `UPDATE usuarios SET edad = 31 WHERE nombre = 'Ana';`
- DELETE: **elimina** registros de una tabla según una condición. No afecta la estructura de la tabla, solo los datos. Ejemplo: `DELETE FROM usuarios WHERE edad < 18;`
### Funciones de agregación
Son funciones que **procesan** un conjunto de valores en una columna y **devuelven un único valor** resumido. Las funciones de agregación son `COUNT`, `SUM`, `AVG`, `MAX`, `MIN`.
### Valores nulos
Los valores nulos indican la **ausencia** de un valor en una columna de una tabla. Un valor `NULL` no es lo mismo que un valor vacío (como una cadena vacía ''), cero ($0$), o un espacio en blanco; representa que el dato es desconocido, no aplicable o simplemente no está definido.
### 
