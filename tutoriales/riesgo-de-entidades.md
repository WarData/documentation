# Riesgo de entidades

Winmotor incorpora controles automáticos para la gestión del riesgo en entidades, tanto de clientes como de proveedores y acreedores.

Estos controles consisten, por un lado, en calcular a tiempo real y por cada entidad los distintos datos que afectan al riesgo (anticipos, albaranes no facturados, facturas de contado no saldadas, cartera vencida, etc), y por otro lado, en bloquear las entidades en las que se ha excedido el riesgo (siempre que tengan un valor mayor a 0 de importe concedido).

Dentro de las entidades se puede acceder a los datos de riesgo en la pestaña administración. Si la base de datos es multicentro, aparecerán los valores por cada uno de ellos.

<figure><img src="https://lh7-us.googleusercontent.com/RM5ms6p-2lAsnn67R4eZ6mW0hjScYze42CjgP9k5EP1rhsFEgY97ulMEIgpRQQsASk8H-eVn9j8Q7TGT9MCl6TjgjlvRNkqPGgrAPA6VseadNT4OULQJbloe9gXd9n0tsc8aB-i89gmo" alt=""><figcaption></figcaption></figure>

Los datos de riesgo que se pueden establecer son:

* Ventas
  * Externo: importe máximo concedido por una empresa externa
  * Interno: importe máximo que nuestra empresa le concede al cliente
    * <mark style="color:blue;">Total concedido</mark> (suma del importe externo e interno)
  * Dispuesto: se calcula automáticamente por la suma de albaranes/ORs pendientes de facturar, facturas de contado no cobradas y cartera pendiente o devuelta. Menos anticipos.
    * <mark style="color:blue;">Disponible</mark> (importe total concedido menos importe dispuesto).
* Compras y gastos
  * Concedido: límite máximo que nos ofrece el proveedor/acreedor
  * Dispuesto: se calcula automáticamente por la suma de albaranes pendientes de facturar, facturas de contado no pagadas y cartera pendiente o devuelta. Menos anticipos.
    * <mark style="color:blue;">Disponible</mark> (importe total concedido menos importe dispuesto).
  * Acumulación del riesgo ventas / compras: sirve para definir si el riesgo disponible como cliente lo calculamos “quitando” el riesgo dispuesto como proveedor.
* Total
  * <mark style="color:blue;">Dispuesto</mark>: si tenemos el parámetro anterior marcado, se calcula el total dispuesto restando al dispuesto en ventas el dispuesto en compras. Si NO está el parámetro marcado, el total dispuesto será igual al dispuesto en ventas.
  * <mark style="color:blue;">Disponible</mark>: riesgo concedido al cliente menos el total dispuesto.

Los valores calculados automáticamente son:

* Ventas
  * Anticipos: acumulación de los anticipos del cliente no compensados
  * Albaranes u ORs no facturados
  * Contado pendiente de cobro: facturas cuyo tipo de pago son de tipo contado y no están cobradas
  * Pte. recibir en plazo, pte. recibir fuera de plazo, en cartera no vencidos, en cartera vencidos, devueltos: son todos los estados que hacen referencia a cartera pendiente.
* Compras
  * Anticipos: acumulación de los anticipos que he realizado el proveedor y no se han compensado
  * Albaranes no facturados
  * Contado pendiente de pago
  * En cartera no vencidos: estado de la cartera de pago pendiente.\


En documentos, se podrá ver el saldo disponible del cliente así como el cuadro de riesgo de la entidad desde el botón €.&#x20;

<figure><img src="https://lh7-us.googleusercontent.com/mBpZADAd1NBcp5aZxeDsAKqSQEVp9-ls_j0xB-3zrJSvRuKAbBPvcM-WDx3R3Jx5SYEFYnEByFIPVo524iH4vCWAaoMMcAXiR69yvL-0JvzCG8VOJ389FL4RVhcp20u-1M6pFlvRUjT8" alt=""><figcaption></figcaption></figure>

El cuadro del riesgo que aparece al pulsar el botón es el siguiente

<figure><img src="https://lh7-us.googleusercontent.com/Ag3Mx1Cc2W5pXFefn0vRdMyIM15RdpC4A0KknGPOEWTaJhKl_xYmrSz6dpx7R72iUhhfgEimnZvgI_D-8DLOfwzDW92JctuXqFGbR0yqcrXZpe2AtGhZVejgzdSUOXtab7_EKZbAe7FA" alt=""><figcaption></figcaption></figure>

Si el cliente está bloqueado o tiene el riesgo excedido no permitirá grabarlo. Si empezamos a grabar un documento de venta y el cliente tiene riesgo disponible, a medida que vamos insertando líneas se va controlando que el total del documento no supere su riesgo.

También se controla que, cuando se entrega un pedido no se supere el riesgo. Lo mismo ocurre en la generación de albarán o factura directa desde un presupuesto.

\
