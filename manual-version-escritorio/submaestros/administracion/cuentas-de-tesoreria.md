# Cuentas de Tesorería

Es el área de una empresa en la cual se organizan y gestionan todas las acciones relacionadas con operaciones de flujo monetario o flujo de caja. ... Esto incluye los cobros por actividades de la empresa, los pagos a proveedores, las gestiones bancarias y cualquier otro movimiento de la caja de una empresa.

**\* LAS CUENTAS DE TESORERÍA SE APLICAN A LOS PERFILES DE LOS USUARIOS (para que un usuario o grupo de usuarios de un perfil puedan asignar una cuenta de tesorería, ésta tiene que haberse añadido anteriormente desde Configuración > Permisos / Perfiles > Perfiles > seleccionar perfil y en la pestaña "Cuentas" añadir las cuentas de tesorería que podrá usar ese perfil)**

La opción muestra un listado de cuentas de tesorería donde podemos dar de alta nuevas usando botón derecho "Alta de Ficha" o doble clic en una zona sin datos.

Las básicas serían "Caja" y "Banco" determinando cada una el tipo de cuenta. La configuración de "Caja" sería del siguiente modo, pudiendo añadir o cambiar cualquier configuración final en la empresa del cliente.

**Asiento de apertura de caja automático**

Dentro del cierre de una cuenta existe la opción de que se cree el asiento de apertura de la caja automáticamente en el día siguiente al cierre.1.- ¿Cuándo funciona? Se debe tener relleno el parámetro "concepto apertura caja" dentro del formulario de Parámetros, en la pestaña Administración / Generales. En cada cuenta, se podrá definir si se crea este asiento de apertura o no : para ello, hay un nuevo campo en el formulario de cuentas: "crear asiento apertura al cerrar cuenta"

2.- ¿Cómo funciona? En la opción F6 - Cerrar cuenta, del panel de tesorería, cuando seleccionemos una cuenta que tenga marcado el check mencionado anteriomente, nos aparecerán campos para definir la fecha del asiento (por defecto un día después a la fecha de cierre seleccionada), y el saldo de apertura (por defecto el saldo de la cuenta hasta el día de cierre. Solo tiene en cuenta movimientos con canal efectivo, es decir, que el canal del asiento sea igual al canal definido como canal de efectivo en la cuenta). Después de rellenar estos datos, el programa automáticamente creará en el día indicado una asiento de la caja correspodiente, con el concepto definido en el parámetro "concepto apertura caja", y el importe o saldo indicado.

![](https://files.gitbook.com/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FbPc6iB3pb9wJfn0AiPvy%2Fuploads%2Fgit-blob-55bef08feb3afb7ec7036b2512c6089178a32797%2Fimage.png?alt=media)

o Código: es un campo auto-numérico que nos servirá para identificar cada cuenta, en este caso el orden en el listado

o Identificador: es un campo auto-numérico que nos servirá para identificar cada cuenta, en este caso por tipo

o Check "Activa": marca la situación de la cuenta (activa / inactiva)o Cuenta contable: añade la cuenta de tesorería a la contabilidad

o Tipo de cuenta: indica si la cuenta es tipo "Caja" o tipo "Banco"

o Opciones "Movimientos especiales" / "Movimientos oficiales" / "Indistinto":

o Canales "Efectivo" / "Tarjeta 1-2-3": indican el procedimiento por el cual se realiza el pago. Mediante efectivo, tarjetas, TPV de determinada entidad bancaria, etc.

o Cuentas contables (de cada canal): por cada uno de los 4 posibles canales de una cuenta de tesorería es posible indicar una cuenta contable hacia la contabilidad

o Pestañas:

o Cierres: muestra los cierres de caja a su fecha (opción cierrar cuenta F6 del panel de tesorería), es decir, si el anterior cierre que se muestra es de hace una semana, el último acumulará el cierre de la cuenta de tesorería por intervalo de una semana.

o Perfiles: muestra los perfiles que tienen acceso a la cuenta de tesorería, además de permitir añadir o eliminar el acceso perfiles.

o Pagarés: permite configurar la impresión de pagarés

o Auditoría: datos sobre fecha de creación, usuario y fecha de modificación y usuario.

La configuración "Banco" sería:

![](https://files.gitbook.com/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FbPc6iB3pb9wJfn0AiPvy%2Fuploads%2Fgit-blob-be01ec7b30c9e0e1acd5e4239e85ce42851eac13%2Fimage.png?alt=media)

Se pueden añadir cuentas de tesorería tipo "Caja" con hasta 4 canales de entrada o añadir cuentas de forma independiente para cada canal, incluso cajas por departamento.

o Código: es un campo auto-numérico que nos servirá para identificar cada cuenta, en este caso el orden en el listado

o Identificador: es un campo auto-numérico que nos servirá para identificar cada cuenta, en este caso por tipoo Check "Activa": marca la situación de la cuenta (activa / inactiva)o Cuenta contable: añade la cuenta de tesorería a la contabilidad

o Tipo de cuenta: indica si la cuenta es tipo "Caja" o tipo "Banco"

o Cuenta bancaria: añade la cuenta bancaria a la que se asocia dicha cuenta de tesorería

o Opciones "Movimientos especiales" / "Movimientos oficiales" / "Indistinto": queda restri**n**gido a "movimientos oficiales"

o Pestañas:

o Cierres: muestra los cierres de caja a su fecha (opción cerrar cuenta F6 del panel de tesorería), es decir, si el anterior cierre que se muestra es de hace una semana, el último acumulará el cierre de la cuenta de tesorería por intervalo de una semana.

o Perfiles: muestra los perfiles que tienen acceso a la cuenta de tesorería, además de permitir añadir o eliminar el acceso perfiles.

o Pagarés: permite configurar la impresión de pagarés

o Auditoría: datos sobre fecha de creación, usuario y fecha de modificación y usuario.
