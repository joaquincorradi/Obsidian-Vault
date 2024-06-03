# Temas
- [[#Unidad 2]]
	- [[#Información]]
		- [[#Concepto de información]]
		- [[#Tipos]]
		- [[#Funciones de la información]]
		- [[#Atributos de la información]]
	- [[#Sistemas de información]]
		- [[#Concepto de sistemas de información]]
		- [[#Componentes]]
		- [[#Funciones]]
		- [[#Propósito]]
		- [[#Modalidades de procesamiento]]
		- [[#Niveles de organización]]
	- [[#Clasificación de los sistemas de información]]
		- [[#TPS (Transaction Processing Systems)]]
		- [[#MIS (Management Information Systems)]]
		- [[#DSS (Decision Support Systems)]]
		- [[#ESS/EIS (Executive Support/Information Systems)]]
- [[#Unidad 3]]
	- [[#ERP (Enterprise Resourse Planning)]]
		- [[#Concepto de ERP]]
		- [[#Objetivo]]
		- [[#Atributos]]
		- [[#Características]]
		- [[#Clasificación]]
		- [[#Capacidades]]
		- [[#Criterios de selección e implantación]]
		- [[#Pasos para la implantación]]
	- [[#Fabricantes y productos ERP]]
- [[#Unidad 4]]
	- Sistemas funcionales de información
- [[#Unidad 9]]
	- [[#SIPOC]]
		- [[#Concepto de SIPOC]]
		- [[#¿Cuándo es útil?]]
		- [[#¿Cuándo se debe utilizar?]]

---
# Unidad 2
## Información
### Concepto de información
Datos procesados en forma significativa para el receptor, con valor real y perceptible para decisiones presentes y futuras.
### Tipos
- **Datos maestros** 
	- No volatiles. Se espera que estos datos permanezcan inalterados durante mucho tiempo y se usen varias veces.
	- Representan
		- Objetos: artículos, productos.
		- Sujetos: clientes, empleados.
		- Conceptos: formas de pago.
- **Datos transaccionales**
	- Son generados por diversos tipos de transacciones.
	- Sólo son válidos para una transacción concreta.
	- Se crean utilizando los datos maestros.
	- Ejemplos: notas de pedido, facturas (tipo, razón social, fecha de vencimientos, CAE), recibos.
### Funciones de la información
- Agrega conocimiento.
- Evalúa y notifica.
- Sorprende y estimula.
- Reduce la incertidumbre.
- Influye sobre otros individuos.
- Estimula a la acción.
- Ayuda a la resolución de problemas y TD.
- Revela y filtra alternativas posibles.
### Atributos de la información
- Completitud (cantidad).
- Exactitud (precisión, detalle, error).
- Relevancia.
- Confianza (calidad, presentación).
- Oportunida.
- Verificabilidad.
- Economicidad.
### Jerarquía

| Nivel jerárquico | Características                                                                                                                                                                                                                                                                     | Fuentes  | Decisiones |
| ---------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------- | ---------- |
| Estratégico ↑    | <table><tr><th>Alcance</th><td>Amplio</td></tr><tr><th>Periodo</th><td>Predictivo</td></tr><tr><th>Precisión</th><td>Baja</td></tr><tr><th>Frecuencia</th><td>Baja</td></tr><tr><th>Expectativa</th><td>Inesperada</td></tr><tr><th>Agregación</th><td>Condensada</td></tr></table> | Externas |            |
| Operativo ↓      | <table><tr><th>Alcance</th><td>Definido</td></tr><tr><th>Periodo</th><td>Histórico</td></tr><tr><th>Precisión</th><td>Alta</td></tr><tr><th>Frecuencia</th><td>Alta</td></tr><tr><th>Expectativa</th><td>Anticipada</td></tr><tr><th>Agregación</th><td>Detallada</td></tr></table> | Internas |            |

## Sistemas de información
### Concepto de sistemas de información
Un sistema de información se define como un conjunto de partes interrelacionadas que permite *capturar*, *procesar*, *almacenar* y *distribuir* información para apoyar las decisiones y el control de una organización.
### Componentes
Los componentes de un sistema de información son:
- A nivel de empresa
	- Humanos (usuarios y de sistemas).
	- Procesos de negocio (procedimientos).
- A nivel de sistemas de información
	- Hardware.
	- Software.
	- Base de datos.
	- Redes o telecomunicaciones.
### Funciones
Las funciones de un sistema de información son
- Entrada de los recursos de datos.
- Almacenamiento de los recursos de datos.
- Procesamiento de D en I ????
- Producir salidas de informes y reportes.
- Control de desempeño (retroalimentación).
### Propósito
El propósito de un sistema de información es el de optimizar la gestión y utilización de la información para mejorar la eficiencia, la eficacia y la competitividad de una organización.
### Modalidades de procesamiento
Las modalidades de procesamiento indican cómo y cuándo se actualizan los datos en un sistema de información, así como la arquitectura utilizada para manejar y distribuir estos datos. Son los siguientes
- Interactivo (online, real time)
	- Actualización inmediata: los datos se actualizan en el mismo momento en que se produce la transacción. Esto significa que la información está siempre actualizada y reflejando el estado más reciente.
	- Ejemplos: cajero automático, sistema de reserva de pasajes aereos.
- No interactivo (batch o lotes)
	- Actualización diferida: las transacciones se recopilan y se procesan juntas (por lotes) en un momento posterior. Los datos no se actualizan inmediatamente, sino en un momento específico, que puede ser una vez al día, una vez a la semana, etc.
	- Ejemplos: facturación de servicios.
- Procesamiento centralizado / distribuido.
### Niveles de organización

![[niveles_de_organizacion.png]]
## Clasificación de los sistemas de información

![[tipos_niveles.png]]
### ESS/EIS (Executive Support/Information Systems)
- Objetivo: Combinar DSS + SE para el proceso de toma de decisiones no programada, abordando problemas no estructurados.
- Nivel: estratégico ↑
### MIS (Management Information Systems)
Sistema de información gerencial.
- Objetivo: manejar datos para la toma de decisiones programada y resolución de problemas estructurados.
- Nivel: táctico ─
### DSS (Decision Support Systems)
Sistema de soporte a decisiones
- Objetivo: manejar información para la toma de decisiones semiestructuradas.
- Nivel: táctico ─
### TPS (Transaction Processing Systems)
Sistema de procesamiento de transacciones.
- Objetivo: mejorar eficacia y eficiencia en el desarrollo de las actividades rutinarias de la organización.
- Nivel: operativo ↓

---
# Unidad 3
## ERP (Enterprise Resourse Planning)
### Concepto de ERP
Sistema integrado de software de gestión empresarial, compuesto de módulos funcionales (Logística, Finanzas, RRHH, Producción, Ventas, Compras, etc.) susceptibles de ser adaptados a las necesidades de cada cliente.
### Objetivo
Facilitar la gestión de los recursos de la empresa integrando y coordinando la información de los distintas áreas funcionales.
### Atributos
- **Única DB:** integridad y consistencia de datos.
- **Entorno internacional:** idiomas, monedas, impuestos, localización de documentos legales.
- **Soluciones verticales/sectoriales:** aplicaciones a medida.
### Características
- **Es el sistema de mayor nivel de complejidad.**
- **Orientado al cliente y resultados finales.**
- **Integración vertical con**
	- Provedores (módulo SCM, supply chain management, gestión de la cadena de suministros).
	- Clientes (módulo CRM,  customer relationship management, gestión de las relaciones con los clientes).
- **Integración horizontal.**
- **Alineado con la visión por procesos.**
### Clasificación
- **Por tipo de instalación**
	- Local
	- En la nube
- **Por código empleado**
	- Open source
	- Código privativo
- **Por especializacion**
	- Vertical (sector específico)
	- Horizontal (soluciones genéricas)
### Capacidades
- **Capacidad de parametrización:** permiten personalizar los menús y funciones según las necesidades específicas de la empresa.
- **Adaptación a estructura organizacional:** puede configurarse para gestionar múltiples sucursales y depósitos, y asignar funciones específicas a cada usuario según su rol en la organización.
- **Interfaz de usuario (UI) y de sistema (U/S) flexible y avanzada:** ofrecen interfaces que son intuitivas y fáciles de usar.
- **Integración con otras aplicaciones:** pueden integrarse con otros sistemas y aplicaciones a través de EDI (Intercambio Electrónico de Datos), XML para comunicación en internet, herramientas ofimáticas (como Microsoft Office), y soluciones de Business Intelligence (BI) como Data Warehousing (DW) y Data Mining (DM).
- **Capacidad de acceso a información:** cuentan con generadores de reportes avanzados que permiten el análisis y la visualización de datos. OLAP (Procesamiento Analítico en Línea) facilita el análisis multidimensional de datos.
- **Otras herramientas:** incluyen funcionalidades de seguridad para proteger los datos y las operaciones del sistema. Ofrecen ayuda en línea para asistencia inmediata y cuentan con auditorias de bases de datos.
### Criterios de selección e implantación
- Funcionalidad (módulos, carencias)
- Criterios técnicos (plataforma, DB, XML, EDI, lenguajes y herramientas)
- Criterios económicos (licencia, implantación, consultoría, análisis ROI)
- Criterios organizativos (cambio áreas)
- Facilidad de uso
- Proveedores (fabricante + representantes)
- Referencias de implantación (del mismo sector)
### Pasos para la implantación
1. **Estudio técnico-funcional del proyecto.**
	- Restricciones económicas.
	- Restricciones temporales del proyecto.
	- Apoyo de consultores.
2. **Elección ERP.**
	- Alcance funcional (módulos a implantar).
	- Alcance organizativo (departamentos, procesos).
	- Viabilidad del proyecto
	- Desarrollos específicos para necesidades no cubiertas.
3. **Desarrollo progresivo.**
	- Por módulos / unidades organizativas.
4. **Tunning o parametrización.**
	- Ajuste técnico del sistema.
	- Formación de usuarios.
	- Documentación del proyecto.
5. **Mantenimiento.**
	- Disponer de medios para mantener el ERP.
## Fabricantes y productos ERP
- Tango Gestión
- Microsoft Dynamics 365
- SAP ERP
- Odoo
- ERPNext

---
# Unidad 4
---
# Unidad 9
## SIPOC
### Concepto de SIPOC
Herramienta en formato de tabla que utilizan los equipos de mejora para identificar todos los elementos relevantes de un proceso organizacional antes de que el trabajo comience. 
Ayuda a definir un proyecto complejo que puede no estar bien enfocado.
El nombre de la herramienta incita a un equipo a considerar los proveedores del proceso (*SUPPLIERS*), las entradas (*lNPUTS*), la secuencia de operaciones del proceso (*PROCESS*), las salidas (*OUTPUTS*) y los clientes que reciben las salidas del proceso (*CUSTOMERS*).
### ¿Cuándo es útil?
Cuando no está claro:
- ¿Quién provee entradas al proceso?
- ¿Qué especificaciones se piden en las entradas?
- ¿Quiénes son los clientes verdaderos del proceso?
- ¿Cuáles son los requerimientos de los clientes?
### ¿Cuándo se debe utilizar?
- Como punto de partida para investigar un proceso y cuando el equipo tiene que entender los conceptos básicos que conforman el proceso.
- Cuando un equipo necesita una manera de registrar el conocimiento colectivo sobre un proceso en un formato fácil de ver.
- Cuando un equipo tiene que presentar una comunicación concisa a los demás acerca de un proceso y los parámetros que lo componen.