Devolución de IA:

Aquí tienes la lista numerada de todas las ambigüedades detectadas en la especificación, categorizadas para facilitar su revisión con el equipo de desarrollo o el Analista Funcional:



1\.  \*\*Origen de la navegación:\*\* El texto dice "Ingresa al buscador, ingresa a la web". No queda claro si se refiere a un buscador externo (como Google), a un buscador interno del sistema, o si el "buscador" es el campo donde se coloca el número de cuenta.

2\.  \*\*Ubicación del botón "Alta":\*\* Se indica que el botón se debe mostrar o no según el estado de la cuenta, pero no se especifica su ubicación física en la interfaz (¿está dentro de la ficha de la cuenta, en una tabla de resultados o en un menú global?).

3\.  \*\*El control de "Sexo":\*\* Se define como un \*Checkbox\*. Un checkbox suele representar una opción binaria de sí/no. No se especifica qué valor se guarda si está marcado y cuál si está desmarcado, ni cómo se contemplan opciones de género no binarias si el sistema lo requiere.

4\.  \*\*Lógica de generación del CUIT:\*\* Se menciona que se genera según el "Sexo". Al ser el sexo un checkbox, no hay una regla clara para asignar los prefijos de CUIT (20 para hombres, 27 para mujeres, 23 para ambos).

5\.  \*\*Edición del CUIT para no-DNI:\*\* Para documentos distintos al DNI, el CUIT deja de ser obligatorio. La ambigüedad reside en si el campo debe ocultarse, quedar vacío para carga manual o si el sistema debe intentar generarlo de otra forma.

6\.  \*\*Límite superior de Fecha de Nacimiento:\*\* Se establece que debe ser "de 1940 en adelante", pero no se define el límite superior. ¿Se permiten fechas futuras o solo hasta la fecha actual del sistema?

7\.  \*\*Tipo de controles para Domicilio:\*\* No se aclara si los campos "Localidad", "Provincia" y "País" son campos de texto libre o listas desplegables (dropdowns) dependientes entre sí.

8\.  \*\*La obligatoriedad de "Piso":\*\* En la lista de campos de domicilio figura "Piso", pero en el párrafo de campos obligatorios se omite. No queda claro si un beneficiario que vive en una casa (sin piso) puede dejar el campo vacío.

9\.  \*\*Imposibilidad de actualizar datos:\*\* Si la persona ya existe, los campos se bloquean. Esto genera una ambigüedad operativa: ¿qué sucede si el domicilio o el estado civil de esa persona cambió? El sistema no parece permitir la actualización desde esta pantalla.

10\. \*\*Lógica de distribución del 100%:\*\* Se indica que si ya existen beneficiarios, se debe habilitar la edición de los anteriores para que la suma dé 100%. Las dudas son:

&#x20;   \* ¿El sistema valida el 100% antes de guardar o mientras el usuario escribe?

&#x20;   \* ¿Se pueden guardar cambios parciales si la suma aún no llega a 100%?

&#x20;   \* ¿Qué pasa si el usuario borra un beneficiario? ¿El sistema reparte el porcentaje sobrante automáticamente?

11\. \*\*Soporte de decimales:\*\* No se especifica si el "Porcentaje de beneficio" acepta decimales (ej. 33.33%) o si deben ser estrictamente números enteros.

12\. \*\*Ubicación y detalle de Mensajes de Error:\*\* Dice que se debe "mostrar un mensaje de error". No se especifica si es un mensaje general (pop-up) o mensajes específicos al lado de cada campo invalidado.

13\. \*\*Acciones en la Pantalla de Éxito:\*\* Al finalizar, se muestra la pantalla con todos los beneficiarios. La ambigüedad es si esta pantalla es solo de lectura o si desde allí se pueden realizar nuevas acciones (editar, eliminar, volver atrás).

14\. \*\*Estados de cuenta no previstos:\*\* Solo se mencionan los estados "activo, suspendido, dado de baja". No se especifica el comportamiento si la cuenta está en un estado intermedio o nulo (ej. "Pendiente de aprobación" o "Bloqueada").

15\. \*\*Formato de Documentos Extranjeros:\*\* Para tipos de documento como PAS (Pasaporte) o CE (Cédula de Extranjería), no se definen máscaras de entrada ni longitudes máximas, que suelen ser distintas al DNI.

