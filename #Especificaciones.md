#Especificaciones
Especificación No Funcional

    Debe funcionar correctamente en los siguientes navegadores: Firefox, Chrome
    Debe permitir almacenar al menos 15 contactos

Especificación Funcional
Listado

El usuario ingresa al sistema
	

El sistema muestra la pantalla:

    Títulos: Contactos
    Grilla
        Columnas
            Nombre: Nombre del contacto
            Mail: Dirección de correo electrónico del contacto
            Opciones (Sólo disponibles cuando hay contactos guardados)
                Editar
                Borrar
        Por defecto la grilla está vacía. Se debe visualizar el mensaje: "No hay contactos guardados"
        Opciones para ordenar los datos por nombre o por mail
        Por defecto, la lista se ordena alfabéticamente por nombre de contacto.

    Opción para agregar nuevo contacto: "Nuevo Contacto"

	
Alta

El usuario selecciona la opción para agregar un nuevo contacto
	

El sistema despliega un formulario con la siguiente información

    Nombre (texto, obligatorio, 35 caracteres). Valor por defecto: vacío. Nombre del contacto.
    Mail (dirección de correo electrónico, obligatorio, 35 caracteres). Valor por defecto: vacío.
    Opciones: Guardar y cancelar

	

Si se estaba agregando un nuevo contacto o editando uno existente el sistema emite un mensaje informando que se perderán los cambios

El usuario completa los campos obligatorios.
	

El sistema almacena los datos, los cuales se visualizan en la parte superior de la pantalla, en una grilla junto a las opciones editar y eliminar.
	

    Si no se completa algún campo obligatorio el sistema muestra un mensaje informando que dicho campo debe completarse.
    Si la dirección de correo no cumple con el formato especificado en el Anexo A, el sistema emite el mensaje: "El valor ingresado no es un email"
    Si ya se encuentra almacenada una dirección de correo electrónico igual a la que se está ingresando, el sistema emite un mensaje informando que no es posible almacenar direcciones de mail duplicadas

Edición

El usuario selecciona la opción para modificar un contacto
	

El sistema despliega un formulario con la siguiente información

    Nombre(texto, obligatorio, 35 caracteres). Valor por defecto: El nombre asociado al contacto seleccionado
    Mail (dirección de correo electrónico, obligatorio, 35 caracteres). Valor por defecto: El mail asociado al contacto seleccionado
    Opciones: Guardar y cancelar

	

Si se estaba agregando un nuevo contacto o editando uno existente el sistema emite un mensaje informando que se perderán los cambios

El usuario los campos
	

El sistema almacena los datos
	

Mismas validaciones que en el alta
Baja

El usuario selecciona la opción para eliminar un contacto
	

El sistema emite un mensaje solicitando la confirmación del usuario sobre estar seguro de querer borrar el contacto: "Está seguro que quiere borrar el contacto <Nombre del contacto>"
	

El usuario confirma el mensaje
	

Si el usuario cancela el mensaje, los datos no se eliminan

Los datos son eliminados
	

Anexo A: Formato de direcciones de email

Siguiendo las especificaciones de http://tools.ietf.org/html/rfc5322#section-3.4.1, el mail está formado por:

    Una cadena no nula compuesta por letras, números, "+", ".", "_" y/o "-"
    El signo @
    Una cadena no nula, compuesta por letras, números,  ".", "_" y/o "-"
    Un punto
    Una cadena de entre 2 y 4 caracteres (inclusive) compuesta por letras
