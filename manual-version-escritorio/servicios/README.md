# Servicios

Un servicio es la comunicación por parte de una compañía, administrador, asegurado o cliente de un siniestro que requiere de una o varias intervenciones que serán realizadas por uno o más operarios con su vehículo.

**¿Qué es una intervención en un servicio?** Las intervenciones son aquellas operaciones que se realizan para solucionar el servicio. Puede contar con una o varias intervenciones que serán cotizadas de forma independiente y que podrán presupuestarse o facturarse de forma independiente o conjunta a la compañía o al asegurado, así mismo cada una de las intervenciones podrá realizarse por distintos operarios y vehículos en función de las necesidades del servicio. [Véase Tipos de intervenciones](../submaestros/tipos-de-intervenciones.md)

**1.- PANEL DE SERVICIOS**

![](<../../.gitbook/assets/imagen (26).png>)

A) Filtros sobre la búsqueda de servicios mediante fecha de apertura por intervalo, por palabras (campo "Filtro"), pudiendo añadir además tipo de intervención, estado, tipo de vehículo, perito y administrador mediante el uso del botón ![](<../../.gitbook/assets/imagen (11).png>):

![](<../../.gitbook/assets/imagen (71).png>)

Estos filtros se pueden fijar a fin de no tener que aplicarlos cada vez que se cierra la pestaña o la aplicación mediante el desplegable mostrado a continuación y aplicando **"Establecer filtro por defecto"** pudiendo modificarlo en cualquier momento y posteriormente pulsando en el botón inferior "Cerrar" para una visualización óptima de la rejilla de servicios:

<figure><img src="../../.gitbook/assets/imagen (78).png" alt=""><figcaption></figcaption></figure>

B) Botones de Servicios desde el menú desplegable:

<figure><img src="../../.gitbook/assets/imagen (61).png" alt=""><figcaption></figcaption></figure>

Nuevo servicio      ![](<../../.gitbook/assets/imagen (82).png>)

Localizar servicio  ![](<../../.gitbook/assets/imagen (137).png>)

Actualizar (fuera del menú desplegable)  ![](<../../.gitbook/assets/imagen (165).png>)

Imprimir servicios  ![](<../../.gitbook/assets/imagen (69).png>)

Establecer filtro por defecto ![](<../../.gitbook/assets/imagen (181).png>)

[Vista por Operarios - Enlace](vista-por-operarios.md) ![](<../../.gitbook/assets/imagen (172).png>) - _Opcional_

Cambiar vista (activa rejilla avanzada) ![](<../../.gitbook/assets/imagen (30).png>)

[Producción por usuario - Enlace](produccion-por-usuario.md) ![](<../../.gitbook/assets/imagen (182).png>) - _Opcional_

C) Códigos de color de los servicios

![](<../../.gitbook/assets/imagen (36).png>)

![](<../../.gitbook/assets/imagen (96).png>)

Mediante el uso de colores en las líneas de los servicios podemos identificar servicios pasados, para hoy, para mañana o posteriores y los dados de alta mediante programación de mantenimientos. Según la primera imagen, tenemos 5 eventos pasados del día actual y 2 servicios programados

Disponemos además de 2 modos de panel "Grabación" y "Consulta" para simplificar el contenido de botones y visualizar fácilmente servicios, eliminando filtros en el modo grabación.

**2.- ALTA DE SERVICIO**

![](<../../.gitbook/assets/imagen (94).png>)

En el documento de alta de un servicio encontramos los siguientes campos:

A) Serie > Permite asignar diferentes series por posibles altas en centros distintos, control independiente de servicios o cualquier necesidad asociada a la serie por parte del cliente. [Véase Series](../configuracion-general/series.md)

B) Centro > Se puede asociar la serie del servicio al centro y/o modificarlo posteriormente en este campo que ofrece las opciones en forma de desplegable (para distribuciones con multi-centro activo).

C) Fecha de apertura > Se rellena automáticamente en la fecha y hora de apertura siendo modificable

D) Estado > [véase Estados](../submaestros/estados.md)

E) Cliente > Permite añadir entidades existentes mediante código al mismo tiempo que se presentan unas opciones distintas en función de si la entidad es cliente o compañía de seguros.

&#x20;**Una entidad tipo "Cliente" mostrará el campo "Pedido"** para identificar el código de pedido del servicio si es necesario y cuando sea **una entidad tipo "Compañía" mostrará que es compañía de seguros, campos Sub-compañía / Siniestro / Póilza y Cobertura (con campo porcentaje y check si está cubierto al 100%).**

**El Cliente es quien solicita el servicio, teniendo en cuenta que si es una compañía de seguros, se activarán los campos requeridos indicados anteriormente.**

**La Compañía de seguros es la** entidad que realiza el encargo de servicio en nombre del asegurado y a la que es posible facturar o presupuestar además de al asegurado.

F) Sub-Compañía > entidad que encarga el servicio a la compañía

G) Siniestro > código alfanumérico asignado por la compañía o empresa al siniestro o en su defecto breve descripción de lo ocurrido

H) Póliza > código alfanumérico de la póliza del asegurado

I) Afectado > entidad que recibirá el servicio pudiendo ser a la vez cliente y afectado o sólo afectado (ejemplo: un vecino de una Comunidad de Vecinos con seguro, el cliente es la Comunidad y el afectado es el vecino).

J) Dirección / Población / Teléfono > datos del asegurado donde la escritura es libre. Sobre el teléfono se disponen de hasta 8 campos libres

K) Descripción > información detallada del siniestro

L) Observaciones > campo libre que completa la información de la descripción

Sobre los **datos de contacto:**

M) Fecha / Hora > muestra el momento en el que se ha contactado con el asegurado o compañía, es modificable y, en la apertura del servicio, coincide con la fecha y hora de apertura

N) Usuario > aquel que da de alta el servicio

O) Contactado > Opción **SI** - muestra las opciones "Aplazamiento acordado con el cliente" y "Cita acordada". El primero sólo permite añadir un comentario sobre el motivo del aplazamiento y el segundo la fecha y hora de la cita así como un comentario // Opción **NO** - muestra las opciones Motivo > "Teléfono apagado", "No contesta", "Comunica" y "Teléfono erróneo" y comentario.

**\*\*\* Para que el estado del servicio cambie de "PENDIENTE DE CITA" a "CITADO" es imprescindible modificar la hora de la cita**, en caso contrario la situación del servicio se mantendrá en pendiente.

**\*\*\*** Una vez dada la cita para una intervención y cambia su estado, **al dar de alta una nueva intervención cambiará de nuevo para informar del último.**

Sobre la **intervención:**

![](<../../.gitbook/assets/imagen (68).png>)

P) Fecha / Hora intervención > momento acordado para el inicio de la intervención. Cuando el operario llegue a la localización y active en la aplicación móvil "Hora de llegada", este campo cambiará a dicho momento para informar a los supervisores.

Q) Rejilla de **Tipos de intervención** > muestra todos los tipos disponibles a fin de seleccionar uno o varios tipos

R) Rejilla **Vehículos** > muestra un campo desplegable a fin de seleccionar uno o varios vehículos para la intervención. Es posible asignar vehículos a operarios a fin de que salga por defecto uno en función del operario, pudiendo cambiarlo si es necesario

S) Rejilla **Operarios** > muestra un campo desplegable a fin de seleccionar uno o varios trabajadores sobre la intervención

