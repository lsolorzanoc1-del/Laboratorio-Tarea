# Laboratorio-Tarea
<br>

## Ejercicio en Clase 3 – Modularización en Java
Curso: Programación 1
<br>

### Parte 1 – Análisis del Programa Original
En el programa original se observó que todo el código estaba dentro del método main, incluyendo:

1)Agregar estudiante

2)Mostrar estudiantes

3)Calcular promedio

4)Buscar la calificación más alta

5)Mostrar el menú



Estas tareas pueden convertirse en métodos independientes porque cada una cumple una función específica. 
<br>
<br>
<br>

##### También se repiten validaciones como:

1)Verificar si las listas están vacías.

2)Conversión de texto a números sin control de errores.
<br>
<br>

##### Dividir estas tareas mejora el programa porque:

1)Hace el código más organizado.

2)Permite reutilizar métodos.

3)Facilita el mantenimiento.

4)Reduce la posibilidad de errores.
<br>
<br>
<br>

### Variables Locales vs Globales

Variables Globales (static) <br>
static List<String> estudiantes;<br>
static List<Double> calificaciones;



##### Se dejaron como globales porque:

1)Representan los datos principales del sistema.

2)Son utilizadas en varios métodos.

3)Deben mantenerse disponibles durante toda la ejecución.
<br>
<br>



#### Variables Locales

##### Ejemplos:

1)Scanner scanner

2)int opcion

3)double suma

4)double promedio

5)double calificacion

6)Estas se declararon dentro de los métodos porque:

7)Solo se usan en una parte específica del programa.

8)Reducen el riesgo de modificar datos accidentalmente.

9)Mejoran la seguridad y claridad del código.
