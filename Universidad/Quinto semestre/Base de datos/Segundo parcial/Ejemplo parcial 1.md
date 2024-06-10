## Enunciado
**Contexto:** Una empresa de entrega de paquetería, *"EntregaUCC"*, ha decidido modernizar su sistema de gestión de envíos y entregas. Para ello, necesita diseñar una base de datos que permita almacenar toda la información relevante sobre sus operaciones diarias.

**Requerimientos:** La empresa necesita registrar información sobre los ==clientes== que utilizan sus servicios. Cada cliente tiene nombre completo formado por primer nombre, segundo nombre y apellido, dirección (que puede desglosarse en calle, número, barrio, ciudad y código postal), varios teléfonos de contacto y correos electrónicos. No es necesario guardar el prefijo del país en los teléfonos. Es necesario registrar su DNI, fecha en la que se dio de alta y la antigüedad que tiene en el sistema calculado con la fecha antes mencionada. Es necesario guardar la fecha de nacimiento y un código de identificación interno formado por la union del primer nombre, el DNI y la fecha de alta. El sistema, por el momento, no soporta clientes que no tengan DNI.
Cada ==paquete== enviado a través de *"EntregaUCC"* debe tener registrado su peso, dimensiones formadas por (largo, ancho y alto), descripción del contenido y el valor declarado. los paquetes tienen registrado un seguro. Cada paquete es enviado en un solo envío y estos pueden soportar varios paquetes. Actualmente la empresa no soporta paquetes cuyo peso supere los 200 kilos. La empresa cuenta con empleados que realizan distintas funciones. Cada empleado tiene nombres, apellido, número de seguro social, puesto de trabajo que puede ser (Responsable, personal de planta o gerente), salario, fecha de contratación y antiguedad. Además, algunos empleados tienen certificaciones especiales otros no. Estas certificaciones tiene un nombre, una descripción y un puntaje. no todas las certificaciones fueron realizadas por un empleado. Los envíos son gestionados por varios empleados.

  

Es importante para la empresa almacenar un % de comisión en cada uno de los envíos realizados por cada uno de los empleados. esta comisión puede ser del 15%, 20% ο 30%.

  

Las entregas se realizan a través de rutas predeterminadas. Cada ruta tiene un identificador único cuyo valor se genera concatenando los km a recorrer, 2 letras del abecedario y 3 números. Este atributo lo ingresa el usuario manualmente, nombre de la

  

ruta, descripción y ciudades por las que pasa la ruta. También se almacena la cantidad de kilómetros estimados recorridos y la duración estimada de todo el trayecto. Estas rutas están pre cargadas en el sistema y pueden no haberse usado nunca o haberse usado muchas veces. La empresa necesita almacenar tanto los kilómetros totales utilizados en el envío, la duración total de todo el

  

envío y la duración y los kilómetros reales consumidos en cada una de las rutas utilizadas en cada envío. Un envío representa la acción de transportar un paquete desde el cliente hasta su destino. Cada envío tiene fecha de envío, fecha estimada de entrega, estado del envío (en tránsito, entregado, retrasado, etc.) y puede involucrar a uno o más empleados durante el proceso. Además, cada envío debe registrar las rutas utilizadas y el cliente que envía el paquete. El sistema debe permitir que un cliente envíe múltiples paquetes. Los clientes se dan de alta en el sistema al momento de hacer un envío. Cada envío permite varios paquetes y lo realiza solo un cliente. En la base de datos del sistema, no todos los empleados realizaron envíos. Es importante que el sistema permita que cada empleado pueda realizar multiples envios. Cada uno de los envíos tiene como mínimo una ruta asignada y el recorrido total puede estar formado por varias rutas.

  

Cada paquete tiene un costo base asignado al momento de darlo de alta. Es importante almacenar en el sistema el costo total del envío que se calcula sumando cada uno de los costos de envío base de cada paquete involucrado multiplicado por la cantidad de kilometros totales.