Una transacción es una unidad lógica de trabajo que agrupa una o más operaciones sobre la base de datos y que debe cumplir íntegramente las propiedades **ACID** o no tener ningún efecto permanente.
### ACID
Para asegurar la integridad de los datos se necesita que el sistema de base de datos mantenga las siguientes propiedades de las transacciones:
- Atomicidad: o se ejecutan todas las operaciones o ninguna. Si la transacción falla, se deshacen todos los cambios.
- Consistencia: la base de datos pasa de un estado consistente a otro estado consistente, nunca queda en estado inválido. Se garantiza con restricciones (PK, FK, CHECK), triggers y reglas de integridad.
- Aislamiento: 