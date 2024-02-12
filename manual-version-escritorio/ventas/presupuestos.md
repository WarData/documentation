# Presupuestos

PRESUPUESTOS DE VENTAS

Mediante esta opción, podremos grabar, modificar o consultar todos los presupuestos de ventas que hemos realizado. Al entrar en ella, nos aparece un menú con calendario en el que se nos presentan opciones para grabar, consultar y listar facturas, y una rejilla que nos muestra todas las que hemos realizado en el día seleccionado en el calendario.

**1 - F1 Nuevo Presupuesto**

Permite dar de alta a un nuevo presupuesto de venta de manera directa rellenando el siguiente formulario. Además de este modo de grabación, para dar de alta un presupuesto se pueden utilizar otros métodos como la opción "Servicios" en la pestaña "Facturación" para intervenciones valoradas o tras valorar una intervención en el botón "Crear Presupuesto".&#x20;

Un presupuesto está compuesto por su cabecera, donde se introducen los datos generales, como la serie, la fecha o cliente, y las líneas.

La cabecera está compuesta por los siguientes campos:

**-SERIE:** es un campo imprescindible de rellenar, y de él depende la presentación o contenido que tendrá el presupuesto. Entre otras cosas, en una serie de presupuesto de venta se define qué contenido tendrán las líneas que se incluyan. Todas las posibilidades de las series de documentos se detallan en la sección [SERIES](../configuracion-general/series.md).

**-NÚMERO:** todos los documentos están clasificados por su serie y un número, que siempre será por defecto el siguiente al último grabado de la misma serie. Tanto el número como la serie de un documento se podrán modificar manualmente, aunque, a menos que sea imprescindible el cambio, no es aconsejable.

**-FECHA:** se indica aquí la fecha de la factura. Esta fecha debe de estar dentro de los rangos definidos en parámetros.

**-CLIENTE / COMPAÑÍA / SUB-COMPAÑÍA / ASEGURADO:** en los documentos de ventas, se podrá indicar si se está vendiendo a un cliente o a una compañía / sub-compañía o seleccionar en el servicio a quién presupuestar tras completar los conceptos relativos a la intervención. Hay que recordar que son tablas de datos diferentes y solo se podrá indicar uno de ellos por presupuesto. Ambos campos contienen botones incrustados para localizar, grabar o editar el cliente seleccionado. Además de código del cliente, se presenta su razón social, su dirección de facturación y el CIF. Además de estos, bajo el CIF se presentará un campo con las notas de facturación del cliente si tuviera.

**-CENTRO:** este campo solo será visible por aquellas aplicaciones en las que se trabaje con más de un centro de trabajo y así se haya indicado en parámetros. Se utiliza para indicar el centro de trabajo para el que se hace el presupuesto. Este campo, se rellena automáticamente y solo será manipulable por aquellos usuarios autorizados.

**-TIPO DE PAGO, VENCIMIENTOS e IMPORTES:** un presupuesto de venta podrá tener distintos tipos de pago diferentes.&#x20;

**-TIPO DE IVA:** este campo tomará por defecto el tipo de IVA definido en la ficha del cliente seleccionado. Se podrá modificar manualmente. Los diferentes tipos de IVA y de exentos, se explican en la sección [TIPOS DE IVA](../configuracion-general/tipos-de-iva.md).

**PESTAÑERO**

**-CONTENIDO:** se presentará una rejilla diferente para cada tipo de presupuesto.

**Opciones desde un presupuesto de venta**

**Aceptar:** si pulsamos esta opción, quedarán guardados todos los cambios que hayamos realizado sobre la ficha del presupuesto.

**Cancelar:** con este botón, saldremos de la ficha del presupuesto sin guardar los posibles cambios que hayamos realizado. Se puede pulsar la tecla ESC para ejecutar esta opción.

**Borrar:** sirve para eliminar el presupuesto, y solo lo podrán hacer usuarios supervisores.

**Imprimir:** imprime el presupuesto de venta con el modelo indicado en la serie del presupuesto.

**Impresión selectiva:** imprime el presupuesto de venta con el modelo que se seleccione al pulsar el botón. Nos aparecerá un recuadro en el que tendremos que indicar el modelo informe.

2 – **Buscar Presupuesto**

Localizador de presupuestos de ventas a través de distintos criterios. Nos permite consultar, borrar o modificar la información de un presupuesto. Al acceder a esta opción encontraremos la siguiente pantalla:

Criterios de búsqueda:

**-NÚMERO, FECHA y CLIENTE:** el cursor se irá situando en el presupuesto cuyo número, fecha y código de cliente coincida con lo seleccionado.

**-PALABRAS NOMBRE CLIENTE:** el localizador presentará en pantalla aquellas presupuestos cuyo cliente contenga la palabra o palabras introducidas.

Para acceder a la ficha de la factura seleccionada, se puede hacer doble clic sobre él, pulsar el botón SELEC., o teclear el botón intro del teclado.

El formulario que se presenta es el mismo que el de grabación.

3 – Listado

Esta opción presenta listados por múltiples filtros sobre presupuestos de venta. Estos listados se pueden acotar a través de los filtros mencionados (fecha, entidad, tipo de pago, serie, etc...).

![](<../../.gitbook/assets/imagen (103).png>)

4 – Cambiar versión

Seleccionando un presupuesto mostrado en la rejilla del panel de presupuestos nos permitirá cambiar a otra de las posibles versiones existentes del mismo presupuesto (no genera una nueva, cambia entra las que ya existan dentro del documento). La identificación de la versión vendrá mediante añadir al número de documento una / y el número de versión.

