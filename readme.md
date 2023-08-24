# Note Know

> Programa para almacenar contactos y notas


## Desarrollado con

- Java

# Requerimientos
- Debe existir una pestaña para gestionar (i.e. agregar, editar, modificar o buscar) la agenda de anotaciones, y otra para gestionar los contactos. Las agenda de anotaciones debe guardar internamente la fecha de creación de la anotación, junto con su contenido explícito escrito por el usuario, mientras que los contactos poseerán: Nombre, número de teléfono, correo electrónico y descripción corta. 
- Debe existir un menú superior que permita limpiar por completo los datos serializados. Su programa deberá recordar el estado del sistema guardando todos sus elementos mediante serialización, donde el archivo final deberá llamarse DATA donde la extensión serán sus 4 siglas de nombres y apellidos. 
- Debe existir un menú superior que permita el "Acerca de" para visualizar la información del autor del sistema, con información de nombre, correo institucional, asignatura, fecha, docente y número de cuenta. Redacte en esta ventana adicional una descripción de la funcionalidad del sistema (2~3 párrafos) y de su análisis principal como el que desarrolló mediante la - Documentación del Entrega Avance 1. 

# Analisis
- La interfaz base sera en la que se creeran las notas
- En esta se veran las pestañas notas(actualmente activa) y la de contactos
- En todo momento se podran ver los botones de ayuda y archivos
- En la pestaña de notas tendremos varios componentes para crear las notas
  - Se agregara un campo de texto para ingresar el contenido de la nota
  - Se agregara un boton para crear un nuevo texto el cual limpiara el contenido de la caja de texto
  - Se agregara un boton para guardar la nota escrita
  - Se agregara una lista con las notas existentes
  - Se agregara un boton para eliminar la nota seleccionada en la lista
- Habrá que crear el objeto de tipo NoteBuilder para crear las notas desde el programa
  - Note builder ejecutara contendra las funciones que seran posteriomente ejecutadas por medio de las interacciones de la interfaz
  - Tendra un arreglo de tipo Note[] con el objetivo de mostrar las notas
  - tendra un metodo addNote el cual creara un nuevo objeto de tipo Nota para posteriormente serializarlo
  - tendra un metodo deleteNote para borrar las notas seleccionadas enviando como parametro el la fecha como un string
- Se creara un objeto de tipo Nota cuyo constructor recibira la cadena de caracteres con la informacion y tendre la fecha la cual sera obtenida creando un objeto Date de tipo LocalDate
  - Se agregara un metodo dateToString que devolvera la fecha convertida a un tipo de dato string
- Se creara un objeto Serializer cuyos metodos seran estaticos
 - Tendrá un metodo serialize para guardar los datos pasados
 - Se creara un metodo por cada tipo de dato (en este caso Note y Contact)


## Autores

👤 **Walter Velasquez**

- GitHub: [@Sirvelasque](https://github.com/Sirvelasque)

