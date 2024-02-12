# Lectura automática de correos de entrada y generación de fichas de servicios

<mark style="color:orange;">**Configuración de modelos en las fichas de las compañías**</mark>



Cuando una entidad es compañía o cliente aparece ahora a la derecha de la pestaña “Históricos” una nueva pestaña “OCR”; haciendo doble clic en una posición vacía damos de alta un nuevo “Modelo de importación”:

<figure><img src="../../.gitbook/assets/imagen (2).png" alt=""><figcaption></figcaption></figure>

●        **Entidad:** será siempre la de la ficha desde la que estamos creando el modelo, no se puede modificar.

●       **Identificador:** es el nombre que le asignamos al modelo.

●        **Tipo de lectura:**

* Alta manual: el contenido del servicio hay que leerlo desde un archivo PDF descargado previamente. En este caso, el origen directo no es un correo electrónico al no realizarse el sistema automático de lectura. El archivo se incorpora dando de alta un servicio y añadiendo un cliente o compañía de seguros que tenga un modelo OCR con alta manual:

<figure><img src="../../.gitbook/assets/imagen (3).png" alt=""><figcaption></figcaption></figure>

* Tiene adjunto: indica al sistema automático de lectura que los datos del servicio vienen dados desde un archivo PDF adjunto al correo. En caso de no marcarlo, los datos tendrán su origen en el cuerpo del correo.
* Lectura por coordenadas: al desmarcar el check "Modelo para la importación de servicios" disponemos de un tercer modelo que leerá los datos mediante las coordenadas (X,Y) de posición de los campos:

<figure><img src="../../.gitbook/assets/imagen (5).png" alt=""><figcaption></figcaption></figure>

_Ejemplo de alta de servicio con modelo OCR de alta manual:_

<figure><img src="../../.gitbook/assets/imagen (6).png" alt=""><figcaption></figcaption></figure>

●        **Cuentas receptoras:** hasta tres posibles cuentas en las que pueden entrar correos de esta entidad solicitando un servicio.

●       **Cuentas origen:**

* Tres posibles cuentas desde las que pueden enviar correos solicitando un servicio.
* El programa leerá cualquier combinación de estas cuentas, es decir, no tiene relación la cuenta receptora dos con el origen dos. Si el programa detecta que en alguna de las cuentas receptoras entra un correo de alguna de las cuentas origen lo considerará una solicitud de servicio y lo procesará según los datos del modelo.

●        **Series destino**

* En caso de que la distribución sea multicentro el programa calculará la serie por la provincia relativa al servicio solicitado.
* Hay que definir por lo tanto una serie por cada provincia en la que actúe el cliente.
* Para el caso de que el programa no pueda localizar la provincia relativa al servicio hay que definir siempre al final una serie sin provincia. Lo idóneo será crear una serie específica para estos casos de manera que el usuario que vaya luego a procesar los servicios detecte rápido el problema y le asigne la serie que le corresponda.

●        **Notificación:** es el código de la notificación de entidad donde habremos definido el mensaje y los destinatarios a los que queremos que se avise cuando entre un servicio de esta entidad.

&#x20;\-----------------------------------------------------------------------------------------------------

Después de pulsar “Aceptar” en el formulario de alta se creará automáticamente una ficha por cada campo de servicios.

Al entrar después en el modelo creado aparecerá así:

&#x20;

<figure><img src="../../.gitbook/assets/imagen (7).png" alt=""><figcaption></figcaption></figure>

<mark style="color:orange;">**Definición de campos**</mark>



Se trata ahora de indicar al programa los criterios para localizar cada campo del servicio en el contenido del correo o en el .PDF adjunto.&#x20;

En caso de haber ya definido un modelo parecido a este en esta entidad u otra entidad podremos utilizar el botón “Importar campos” para seleccionar el modelo origen y automáticamente se rellenarán los valores de los campos igual que el ese modelo seleccionado.

Al hacer doble clic en cada uno de los campos nos aparece este formulario:

&#x20;![](<../../.gitbook/assets/imagen (8).png>)

●        **Campo:** no es editable, lo ha asignado el programa automáticamente y no se puede modificar.

●        **Fórmula de conversión:**

* Necesitarás la ayuda de un programador para utilizar este campo. Se utiliza rara vez y sirve para ajustar el contenido obtenido del documento origen al campo en la ficha del servicio.
* Tienes que partir de la variable $OCR\_CAM\_CUR que contiene en tiempo de ejecución el valor obtenido para este campo.

●        **Localizar el campo en:** sólo en el caso de la utilización de la lectura “Directa” el programa nos pregunta si el contenido de este campo aparece en el asunto o en el cuerpo del correo.

●        **Etiqueta de identificación:**

* Es el texto que nos dará la ubicación del campo. Para el contenido del campo “Póliza” lo normal es que en el contenido del correo origen aparezca el texto “Nº Póliza” o algo por el estilo.
* Este es por lo tanto el texto que tenemos que indicar en la etiqueta de identificación para que el programa sepa dónde está este campo.
* Es muy aconsejable utilizar siempre el “cortar y pegar” para este contenido puesto que muchas veces hay caracteres que no vemos como espacios o intros.
* Los caracteres especiales como “ ª” o “ º “ no son interpretados correctamente por el sistema. Por lo tanto dado este caso indicaremos en la etiqueta de identificación solamente “Póliza” y con esto es suficiente.

●        **Aparición número:** para el caso de la póliza es raro que sea necesario, pero por ejemplo sí ocurre con los teléfonos. Si la etiqueta de identificación es “Teléfono” y ésta aparece en el contenido del correo varias veces tenemos que indicar al programa cuál de ellas es la que tiene que leer.

●        **Posición:**&#x20;

* A la derecha > “Teléfono: “ 959 954 455
* Debajo > “Teléfono: “

959 954 455

* Contenido

&#x20;       \* Indica que es la propia etiqueta en sí la que nos va a dar un valor de si o no (0 / 1).

&#x20;       \* Para el caso por ejemplo de “Urgente” si marcamos que su posición es “Contenido” estamos indicando al programa que, sí existe esa palabra, marque el urgente como 1 (Si).

●       **Leer hasta:**

* Para el caso de posición a la derecha o debajo necesitaremos muchas veces decir al programa hasta dónde tiene que leer.
* En el caso de “Código postal:  03560 Población: CAMPELLO” tendremos que indicar para el campo “Código postal” leer hasta “Población”; con esto se quedará con 03560 que es el texto contenido entre la etiqueta de identificación y “leer hasta”.&#x20;

&#x20;

<mark style="color:orange;">**Formulario de pruebas**</mark>



Dentro de cada ficha de modelo aparece una segunda pestaña “Pruebas” que podemos utilizar además para probar y para completar la configuración de los campos:

<figure><img src="../../.gitbook/assets/imagen (9).png" alt=""><figcaption></figcaption></figure>

●        **Archivo a subir:**

* Este campo aparece sólo en el caso de que el tipo de lectura del servicio sea “Combinada”.
* Nos permite seleccionar un archivo .PDF para hacer la lectura del mismo y probar la configuración de los campos.

●        **Botón “Subir”:**

* Aparece también en la lectura combinada y sólo se activará si está relleno el archivo a subir.
* Ejecutará la lectura del archivo y rellenará el contenido en la zona del “Cuerpo”. Al mismo tiempo ejecutará la conversión de este contenido en un servicio en caso de haber campos ya definidos.

●        **El botón “Generar servicio”** entre el cuerpo y el modelo calculará según los parámetros definidos y el contenido del campo “Cuerpo” un servicio que se visualizará en el modelo.

&#x20;\* Para permitir afinar y mejorar las pruebas el campo “Cuerpo” es editable, se pueden modificar los contenidos para comprobar el efecto al crear el documento.

●        **Botón “Campos”:** nos presenta la lista de campos para poder ver sus parámetros y modificarlos directamente en la lista sin tener que cambiar de pestaña

<figure><img src="../../.gitbook/assets/imagen (10).png" alt=""><figcaption></figcaption></figure>

&#x20;

&#x20;

&#x20;
