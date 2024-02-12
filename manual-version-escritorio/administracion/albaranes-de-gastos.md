# Albaranes de gastos

Mediante esta opción, podremos grabar, modificar o consultar todos los albaranes de gastos que hemos realizado. Al entrar en ella, nos aparece un menú con calendario, filtros de facturación y cliente en el que se nos presentan hasta 4 opciones y una rejilla que nos muestra todos los albaranes que hemos realizado en el día seleccionado en el calendario tras pulsación de F5 o el botón Actualizar.

**1.- NUEVO ALBARÁN**

Permite dar de alta a un nuevo albarán de gastos rellenando el siguiente formulario:

![](<../../.gitbook/assets/imagen (122).png>)

Un albarán está compuesto por la cabecera, donde se introducen los datos generales, como la serie, la fecha o cliente, y las líneas, donde se van grabando las referencias y la cantidad que se pide.

La imagen anterior nos muestra un formulario de albaranes de gastos, donde se graban todos los datos. La cabecera está compuesta por los siguientes campos:

* **Serie:** es un campo imprescindible de rellenar, y por defecto toma el valor definido en la ficha del usuario que graba el albarán. Si este no tuviera definida ninguna serie de albarán en su ficha, se tomará la de los parámetros del programa. En la serie del albarán se define, por ejemplo, el almacén que tomará por defecto las líneas del albarán. Todas las posibilidades de las series de documentos se detallan en la sección…explicación de series de documentos.
* **Número:** todos los documentos están clasificados por su serie y un número, que siempre será por defecto el siguiente al último grabado de la misma serie. Tanto el número como la serie de un documento se podrán modificar manualmente, aunque, a menos que sea imprescindible el cambio, no es aconsejable.
* **Fecha y fecha de recepción:** se indica aquí la fecha de grabación del documento y de la recepción del mismo. Esta fecha debe de estar dentro de los rangos definidos en parámetros.
* **Hora:** presenta la hora de grabación del albarán, no es manipulable por los usuarios.
* **Referencia**: campo libre para incluir datos. Un ejemplo puede ser añadir en él nombre y número del cliente en caso de ser el cliente contado (genérico sin NIF o CIF)
* **Centro:** este campo solo será visible por aquellas aplicaciones en las que se trabaje con más de un centro de trabajo y así se haya indicado en parámetros. Se utiliza para indicar el centro de trabajo para el que se hace el albarán. Este campo, se rellena automáticamente y solo será manipulable por aquellos usuarios autorizados.
* **Acreedor:** en los documentos de gastos, sólo se podrá indicar este tipo de entidad. El campo contiene botones incrustados para localizar, grabar o editar el acreedor seleccionado. Los campos situados justo debajo, presentarán la razón social, saldo, tipo de pago, régimen de IVA, vencimiento.
* **Documento acreditativo:** si el cliente es intracomunitario, y tiene documento acreditativo, se presentarán los campos relativos a este documento en esta pantalla. Si fuera intracomunitario y no tuviera documento acreditativo, saltará un mensaje indicándolo.
* **Régimen de IVA:** este campo tomará por defecto el tipo de IVA definido en la ficha del acreedor (único tipo de entidad seleccionable en este tipo de documento) seleccionado en el albarán. Se podrá modificar manualmente. Los diferentes tipos de IVA y de exentos, se explican en la sección [tipos de IVA](../configuracion-general/tipos-de-iva.md).

**Barra de pestañas**

* **LÍNEAS:** contiene una rejilla en la que se nos presentan las líneas de albaranes de gastos ordenadas por el campo contador de cada línea. Mediante está rejilla podremos consultar, grabar, modificar o eliminar cualquier línea de albarán.

Para grabar una nueva línea, podemos utilizar cualquiera de los métodos utilizados sobre cualquier otra rejilla. Se nos presentará el formulario de grabación de líneas con los siguientes campos:



![](<../../.gitbook/assets/imagen (99).png>)

\- **Artículo**: campo en el que introducimos la referencia del artículo. Se podrá meter la referencia manualmente, o utilizando la opción "Buscar Artículo" o "Buscar Servicio" de los botones incrustados de este campo. Si no localizamos la referencia en la base de datos de artículos o servicios, podemos utilizar la opción Referencia. Con esta opción, el programa buscará en primer lugar en el fichero de artículos, y si no la encontrara, buscará en el de tarifas. Una vez localizada, se nos presentará el siguiente formulario, desde el que podremos crear la referencia directamente. Los otros dos botones incrustados que contiene el campo de artículo, son para consultar/editar la referencia seleccionada, o para crear una nueva. La descripción del artículo tomará por defecto la definida en su ficha, y solo se podrá modificar si el artículo no está incluido en la tarifa.

**- Unidades**: indicamos aquí las unidades a asignar al albarán de gastos

\- **Precio**: importe de gasto del artículo.&#x20;

\- **Descuento y descuento 2**: porcentajes de descuento que se le realizará sobre el artículo o servicio. El descuento 2 se aplica sobre el resultando del primer descuento.

\- **Parcial**: valor total del artículo (sin sumar los impuestos) resultante de multiplicar las unidades pedidas por el precio menos los descuentos.

\- **Aceptar**: con este botón guardamos los cambios realizados.

\- **Cancelar**: abortamos el alta o modificación de la línea.Para eliminar una línea de albaranes de venta, tendremos que abrir la línea de artículo o servicio y pulsar en el botón "Eliminar".&#x20;

* **TOTALES:** presenta el desglose de importe totales del albarán de gastos:

![](<../../.gitbook/assets/imagen (105).png>)

* **OBSERVACIONES**: campo de texto que quedará ubicado únicamente en esta pestaña y que permite su impresión en el informe si así se diseña.
* **ARCHIVOS**: permite adjuntar archivos que quedarán almacenados en el servidor y asociados a la ficha del albarán de gastos. Es muy práctico para almacenar el documento original en PDF.
* **SEGUIMIENTOS**: se podrá grabar seguimientos relacionados con los albaranes de gastos, en esta pestaña se presentan los grabados.
* **ACCIONES**: log de control de todos los eventos registrados en esta ficha por acción, usuario y momento en el que ha ocurrido.

