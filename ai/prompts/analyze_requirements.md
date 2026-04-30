IA utilizada: Gemini PRO


Promt:

Tengo la siguiente especificacion de requerimientos y necesito que detectes todas las ambiguedades que encuentres, para luego poder generar los casos de prueba:



Ahora te paso todo el enunciado:



Ejercicios Prácticos

Debemos generar la funcionalidad de alta de beneficiarios en un seguro de vida, teniendo en cuenta los siguientes criterios:

Pasos previos: Ingresa al buscador, ingresa a la web, carga el número de cuenta (uno activo, otro suspendido, dado de baja), y se deberá mostrar el botón o no según las condiciones.

El seguro de vida debe estar activo, en caso de estar suspendido o dado de baja, no mostrar el botón de alta de beneficiario.

Se deben completar los siguientes campos:


Datos personales:

\- Tipo documento (Desplegable)

\- Número documento

\- Fecha de nacimiento (de 1940 en adelante)

\- Nombre

\- Apellido

\- Sexo (Checkbox)

\- Cuit

\- Nacionalidad (Desplegable)

\- Condición de iva (Desplegable)

\- Estado civil (Desplegable)

\- Discapacidad (Checkbox)

\- Porcentaje de beneficio


Domicilio:

\- Calle

\- Número

\- Piso

\- Código postal

\- Localidad

\- Provincia

\- País



Se deben tener en cuenta las siguientes condiciones:

\- Al ingresar un tipo y número de documento, si esa persona ya existe dada de alta en el sistema (no necesariamente como beneficiario), los campos se deben autocompletar (exceptuando el porcentaje de beneficio) y se deben bloquear los campos para no permitir la edición de los mismos. El campo porcentaje de beneficio debería quedar editable para poder cargar el dato. (En este caso, se da por sentado que la persona existente está viva y activa).

\- Si la persona no existe en el sistema, todos los campos del apartado datos personales a completar son OBLIGATORIOS.

\- El campo cuit se debe autogenerar contemplando los campos: tipo documento, número documento y sexo. Este campo se autogenera solo en caso de que el tipo documento sea DNI, caso contrario el campo deja de ser obligatorio.

\- Los campos calles, número, código postal, localidad, provincia y país son OBLIGATORIOS.

\- El porcentaje de beneficio no debe ser 0

\- El porcentaje de beneficio siempre debe ser 100%, en caso de ya existir uno o más beneficiarios cargados, se debe habilitar la edición del porcentaje de esos beneficiarios, para que la suma de todos de 100%

\- Al hacer click en guardar, se deben validar todos los campos, en caso de que alguno sea incorrecto se debe mostrar un mensaje de error y no permitir el alta.

\- En caso de que todos los datos sean correctos, mostrar un mensaje de alta exitosa y mostrar la pantalla de beneficiario con todos los beneficiarios cargados.


Valores posibles:

Tipo documento: ET, PAS, CE, DNI, CL

Condición de iva: consumidor final, exento, inscripto, monotributista, no categorizado,

sin condición

Estado civil: casado, convivencia, divorciado, otros, separado de hecho, separado

legal, soltero, unión de hecho, viudo 


Haceme una lista numeradas de las ambigüedades



