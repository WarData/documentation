---
description: >-
  Cuando no cuadra el cálculo de Resultado del ejercicio con el informe de
  Pérdidas y Ganancias
---

# Revisión del Balance de Situación

Excepto el balance de sumas y saldos el resto de informes de Winmotor son parametrizados, es decir para cada partida que presentan se calcula el saldo de una serie de cuentas definidas por nosotros. Todas las cuentas que se entregan en el plan contable de Winmotor están incluidas en sus correspondiente informe.

Por otro lado en el informe relativo al Balance de Situación hace un cálculo especial para la partida del resultado del Ejercicio (129) que no es el saldo de esta cuenta puesto que el programa tiene que poder calcularlo aunque no se haya cerrado el ejercicio sino que es el cálculo de la diferencia entre todas las cuentas que afectan al balance de situación (grupos 1 al 5) y las que afectan al informe de pérdidas y ganancias (grupos 6 y 7)

Vamos a explicar qué pasos hay que seguir en caso de que esta partida no coincida con el resultado total del informe de la cuenta de Pérdidas y Ganancias:

<mark style="color:yellow;">**Revisión general:**</mark>

* El balance de sumas y saldos debe estar cuadrado
* En el panel de asientos no debe aparecer el botón “Hay asientos descuadrados”.
* La suma de todos los apuntes coincide con los valores acumulados ”Suma” del balance de sumas y saldos.
* Revisión de informes (esta opción comprueba que no has utilizado cuentas de mayor (1 a 4 dígitos) que no estén incluidas en los cálculos del balance de Situación o de la cuenta de Pérdidas y Ganancias que estás utilizando)
  *   Revisión del Balance de Situación

      * Calcula un balance de sumas y saldos de los grupos 1 a 5, nivel de presentación “Auxiliar” y sin marcar “Presentar sólo cuentas con saldo”.
      * Pulsa el botón para opciones especiales que hay abajo a la izquierda:



      <figure><img src="../.gitbook/assets/image (45).png" alt=""><figcaption></figcaption></figure>

      * Selecciona la opción “Revisar informes”
      * El programa presenta la lista de todos los informes que existen en la base de datos y tienes que seleccionar haciendo doble click el modelo de balance de situación que estás utilizando (general, abreviado o Pyme).
      * Se revisará que todas las cuentas que están en pantalla en el balance de sumas están definidas en alguna de las partidas del informe seleccionado. En caso de que alguna no lo esté se prestará en una lista al final del proceso. Más adelante explicaremos cómo solucionar esto.
      * Revisión de la cuenta de Pérdidas y Ganancias
        * A diferencia de la revisión anterior en este caso hay que filtrar en el balance de sumas y saldos las cuentas de los grupos 6 al 7
        * En el botón de opciones especiales selecciona el informe que has utilizado para calcular la cuenta de Pérdidas y Ganancias
*   Solución a las incidencias encontradas en la revisión de informes:

    * Las cuentas que han aparecido en la revisión indican que no están incluidas en el informe que estás utilizando, alguien las has creado y se ha saltado el paso de la aplicación del informe para esa cuenta.
    * Ve al menú de contabilidad / maestros / PGC
    * Edita la cuenta que te esté apareciendo en la revisión y pincha en la pestaña “Informes”
      * Te aparecerán una lista de los informes en los que esa cuenta está incluida y abajo un botón “Editar” que es para incluirla en uno nuevo



    * Aquí se trata de seleccionar en la izquierda la partida relativa al informe en la que debe estar incluida la cuenta y pinchar el botón “Añadir seleccionado”.
    * Aparecerá en la derecha el informe y la sección donde se va a incluir el saldo de la cuenta en curso.

    <figure><img src="https://winmotor.gitbook.io/~gitbook/image?url=https:%2F%2Flh7-us.googleusercontent.com%2FPUXrv7UJAmKgQ-zoyshZIbR4xEdoCgday530m3inANsKeKwM0MPHCPdI7gQF-HH0VqIK70PaEpOAtoq95SNm0kfGN67iNsPQBZqPDZzNuiBlVD0BCSxz8KDzx1F5cjKObbm54DRzmPUQ4gwNIVK6f9U&#x26;width=768&#x26;dpr=4&#x26;quality=100&#x26;sign=679a82b0fbe204d3f0c01188f773526db6eece4b59c6b6ba2d913e54bee58ce4" alt=""><figcaption></figcaption></figure>

<mark style="color:yellow;">**Revisión para bases de datos que utilizan cuentas analíticas (grupos 0, 8 y 9)**</mark>

Para este caso hay dos pequeñas diferencias al proceso general que hay que tener en cuenta:

* Si al calcular el balance de sumas y saldos has filtrado los grupos 1 al 7, la suma de todos los apuntes no coincidirá con la del balance puesto que tienes apuntes de otros grupos.
* Debes comprobar por otro lado que no existe ningún asiento que contenga apuntes normales y analíticos mezclados y sus debe / haber no estén cuadrados. Es decir, la integridad contable debe cumplirse de manera que en estos asientos la suma de todos los apuntes del grupo 1 al 7 esté cuadrada a nivel debe / haber y lo mismo con los apuntes del resto de grupos.
* Para hacer esta comprobación tienes una opción en el panel de asientos. Pulsando el botón de opciones especiales del panel de asientos abajo a la izquierda selecciona la opción “Localizar en un asiento descuadres en cuentas del grupo 0”. Al pulsarla el programa buscará entre todos los asientos que están filtrados en pantalla si alguno presenta un descuadre al nivel que hemos explicado y habrá por lo tanto que solucionarlo.

<figure><img src="https://winmotor.gitbook.io/~gitbook/image?url=https:%2F%2Flh7-us.googleusercontent.com%2FPe7oNdxyfqGk_d6Y0e2_INiLgUqPD5SHD-losoLR0ert2yeX6T7kjPKd6bh2MyJ7YgpvySUlkwOdcIcV5p-2E7J9qhxbYIZ3EQVJYYBvRrt2py_miYx1B74lYfxxC49mEDzrX268GHMvtOM4ITpq1Zc&#x26;width=768&#x26;dpr=4&#x26;quality=100&#x26;sign=1d3220d1ca2c37fe9209e3fb800c5d07371a5b714a5aa2f480a945bb61ced8b3" alt=""><figcaption></figcaption></figure>

Última actualización hace 1 minuto
