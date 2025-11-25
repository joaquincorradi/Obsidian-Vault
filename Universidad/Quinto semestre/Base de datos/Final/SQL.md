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
### Subconsultas anidadas
Es una consulta que se coloca dentro de otra consulta principal, encerrada entre paréntesis. La subconsulta se ejecuta primero, y su resultado se utiliza en la consulta externa para filtrar, calcular o comparar datos.
### Vistas
Es una consulta almacenada en la base de datos que se presenta como una tabla virtual.
- Es un objeto almacenado en la base de datos: cuando creas una vista, la base de datos guarda su definición como un objeto con un nombre. Un alias, en cambio, sólo existe durante la ejecución de una consulta específica.
- Se comporta como una tabla: `podés` hacer `SELECT`, y en algunos casos `INSERT`, `UPDATE` o `DELETE`, directamente sobre la vista, como si fuera una tabla real, aunque los datos provienen de las tablas subyacentes ya que no almacenan datos físicamente. Por ejemplo, se crea una vista `CREATE VIEW empleados_info AS ...` y se realiza la consulta de la siguiente manera `SELECT * FROM empleados_info;`.
- Seguridad: permiten otorgar permisos específicos a usuarios o roles para que accedan solo a la vista, no a las tablas subyacentes. Esto se hace con el comando `GRANT`. Por ejemplo: `GRANT SELECT ON vista_publica_empleados TO cierto_usuario;`.
---
### Resumen (del libro)
- Los sistemas comerciales de bases de datos no utilizan la concisa y formal álgebra relacional. El ampliamente usado lenguaje SQL, que se ha estudiado en este capítulo, está basado en el álgebra relacional, pero incluye mucho “azúcar sintáctico” . 
- El lenguaje de definición de datos de SQL se utiliza para crear relaciones con esquemas especificados. El LDD de SQL soporta diferentes tipos de datos, como date y time. Se pueden ver más detalles sobre el LDD de SQL, en especial sobre el soporte de las restricciones de integridad. 
- SQL incluye varios constructores del lenguaje de consultas a la base de datos. Todas las operaciones del álgebra relacional, incluidas las operaciones del álgebra relacional extendida, se pueden expresar en SQL. SQL también permite la ordenación de los resultados de las consultas según los atributos especificados. 
- SQL trata las consultas sobre relaciones que contienen valores nulos añadiendo el valor lógico “desconocido” a los valores lógicos habituales de cierto y falso. 
- SQL permite subconsultas anidadas en las cláusulas where. La consulta más externa puede llevar a cabo gran variedad de operaciones sobre el resultado de la subconsulta, como la comprobación de relaciones vacías o de pertenencia de valores al resultado de una subconsulta. Las subconsultas de la cláusula from se denominan relaciones derivadas. 
- Las relaciones se definen como relaciones que contienen el resultado de consultas. Las vistas resultan útiles para ocultar información innecesaria y para recopilar información de más de una relación en una única vista. 
- Las vistas temporales definidas con la cláusula with también resultan útiles para descomponer consultas complejas en partes más pequeñas y más fáciles de comprender. 
- SQL proporciona constructores para actualizar, insertar y borrar información. Las actualizaciones mediante vistas sólo se permiten cuando se cumplen algunas condiciones bastante restrictivas. 
- Las transacciones son secuencias de consultas y de actualizaciones que, en su conjunto, desempeñan una tarea. Las transacciones se pueden comprometer o retroceder; cuando se hace retroceder una transacción, se deshacen los efectos de todas las actualizaciones llevadas a cabo por esa transacción. 
- SQL soporta varios tipos de reunión externa con diferentes tipos de condiciones de reunión.
