# Predefinición de asientos analíticos en las plantillas de asientos

Hemos incorporado en Winmotor la posibilidad de predefinir en una plantilla los apuntes analíticos.  Ahora, al grabar una plantilla de un apunte veremos dos nuevas pestañas: “Costes“ y “Auxiliares”.&#x20;

En la pestaña “Costes” definiremos los datos relativos al apunte analítico y en auxiliares cómo debe comportarse la plantilla en el momento del cálculo.&#x20;

Supongamos el caso de la definición de una plantilla para la grabación de una factura de transportes para el centro de Alicante (es importante tener en cuenta que este ejemplo no tiene sentido práctico ya que en Winmotor los asientos relativos a cualquier factura se generan automáticamente):&#x20;

1 - Plantilla del asiento

* Línea del total con la cuenta del acreedor (dejamos abierto la cuenta auxiliar, el concepto y el número del documento):

<figure><img src="../.gitbook/assets/imagen (195).png" alt=""><figcaption></figcaption></figure>

* Línea del gasto (sólo tendrá que pedir el importe base de la factura, el resto de campos serán automáticos según los introducidos en el apunte del acreedor:

<figure><img src="../.gitbook/assets/imagen (196).png" alt=""><figcaption></figcaption></figure>

* Línea del IVA: no pedirá ningún dato puesto que podemos calcular incluso el importe por el saldo pendiente del asiento:

<figure><img src="../.gitbook/assets/imagen (197).png" alt=""><figcaption></figcaption></figure>

Las novedades que hemos añadido son:

* En la línea del gasto hemos creado la plantilla para el centro de costes. Dado que la plantilla ya la hemos definido como “Portes Alicante” el centro de costo lo hemos imputado directamente (hemos accedido a la creación de la plantilla de costes pulsando la pestaña “Costes” que aparece ahora en las plantillas de apuntes):

<figure><img src="../.gitbook/assets/imagen (193).png" alt=""><figcaption></figcaption></figure>

* <mark style="color:orange;">Definiciones:</mark>
  * Hemos predefinido que el centro es “Sevilla” y que lógicamente es un gasto.
  * Para el cálculo del importe podemos definir:
    * Manual - habrá que teclearlo en el momento de la grabación del apunte.
      * Importe - Se imputará el importe total del apunte en el que estemos.
      * Porcentaje - Se podrá definir que es un porcentaje del importe del apunte que estamos grabando.
  * Hemos añadido otra pestaña “Auxiliares” para definir datos que fuercen el comportamiento de la creación del asiento en general. En el apunte relativo al gasto hemos definido estos datos:

<figure><img src="../.gitbook/assets/imagen (194).png" alt=""><figcaption></figcaption></figure>

* <mark style="color:orange;">Configuración:</mark>
  * “Grabar costes”: hay que marcarlo siempre que queramos que la ejecución de la plantilla genere el apunte de costes.
  * “Generar los costes sin mostrar el formulario de grabación”: si como es el caso del ejemplo, en la plantilla de costes ya han quedado definidos&#x20;
  * “El apunte se grabará de forma repetida” - este parámetro de momento no es funcional.
  * “Generar el apunte sin mostrar el formulario de grabación” - Si hemos predefinido en el apunte todos los campos podremos marcar este check para indicar al programa que no tiene siquiera que mostrar este apunte. Lo hemos hecho así en el caso de la línea del IVA de manera que no aparece en el momento de la grabación, se genera automáticamente sin presentarse.

&#x20;2 - Grabación del asiento

* Una vez hemos definido en el asiento las fechas, hemos seleccionado en el campo de la plantilla la definida anteriormente “Transportes ejemplo centro de costes”.&#x20;
* Hemos mejorado este control de manera que muestra la lista de plantillas pulsando el botón de selección de la derecha

<figure><img src="../.gitbook/assets/imagen (199).png" alt=""><figcaption></figcaption></figure>

* También la hemos mejorado haciendo que se “Autocomplete” según el texto escrito, independientemente de que esté en mayúsculas o en minúsculas. En este caso escribiendo “portes a” ya nos ha aparecido en el selector “Portes Alicante”; pulsando la tecla de tabulación nos hemos situado sobre el botón “Generar”.
* Para la primera línea del total que hemos predefinido para el acreedor, hemos tecleado la cuenta auxiliar, el importe total de la factura en el haber, el concepto y el número de documento:

<figure><img src="../.gitbook/assets/imagen (200).png" alt=""><figcaption></figcaption></figure>

* Para la línea de la base sólo hemos tecleado el importe al debe, el resto de campos y la línea de costes se han grabado automáticamente:

<figure><img src="../.gitbook/assets/imagen (201).png" alt=""><figcaption></figcaption></figure>

* Y la línea del IVA también se ha grabado automáticamente y sin presentarse puesto que marcamos el check “Generar el apunte sin mostrar el formulario de grabación” en los datos auxiliares de la plantilla del apunte de IVA:

<figure><img src="../.gitbook/assets/imagen (202).png" alt=""><figcaption></figcaption></figure>

* Como resultado final tenemos este asiento:

<figure><img src="../.gitbook/assets/imagen (203).png" alt=""><figcaption></figcaption></figure>

* Y en la pestaña “Costes” esta imputación que no hemos tenido que grabar:

<figure><img src="../.gitbook/assets/imagen (204).png" alt=""><figcaption></figcaption></figure>

&#x20;
