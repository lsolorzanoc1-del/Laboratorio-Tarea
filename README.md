# Laboratorio-Tarea
<br>

##  Ejercicio en Clase 3 – Modularización en Java

Curso: Programación 1
<br>
### Parte 1 – Análisis del Programa Original

En el programa original se observó que todo el código estaba concentrado dentro del método main.

#### Dentro de este método se realizaban todas las tareas del sistema:
<br>

• Agregar estudiante <br>
• Mostrar estudiantes <br>
• Calcular promedio <br>
• Buscar la calificación más alta <br>
• Mostrar el menú 

<br>

Cada una de estas tareas cumple una función específica, por lo tanto pueden convertirse en métodos independientes.

<br>
 Validaciones repetitivas detectadas

• Verificar si las listas están vacías. <br>
• Conversión de texto a números sin control de errores.

<br>
 ¿Por qué dividir estas tareas mejora el programa?

• Hace el código más organizado. <br>
• Permite reutilizar métodos. <br>
• Facilita el mantenimiento. <br>
• Reduce la posibilidad de errores. <br>
• Mejora la legibilidad del programa.

<br> <br>
 #### Variables Locales vs Globales
<br>
 Variables Globales (static) <br>
static List<String> estudiantes; <br>
static List<Double> calificaciones; <br>

<br>
Se dejaron como globales porque:

• Representan los datos principales del sistema. <br>
• Son utilizadas en varios métodos. <br>
• Deben mantenerse disponibles durante toda la ejecución.

<br>
 Variables Locales

Ejemplos:

• Scanner scanner <br>
• int opcion <br>
• double suma <br>
• double promedio <br>
• double calificacion

<br>

Se declararon dentro de los métodos porque:

• Solo se usan en una parte específica del programa. <br>
• Reducen el riesgo de modificar datos accidentalmente. <br>
• Mejoran la seguridad y claridad del código. <br>

<br> <br>
### Parte 2 – Modularización del Programa

Para mejorar la estructura del programa se dividió el código en métodos específicos, cada uno con una sola responsabilidad.

<br>
Métodos creados:

• mostrarMenu() <br>
• agregarEstudiante() <br>
• mostrarEstudiantes() <br>
• calcularPromedio() <br>
• mostrarMejorEstudiante() <br>
• leerEntero() <br>
• leerDouble()

<br>

Ahora el método main únicamente:

• Muestra el menú. <br>
• Lee la opción del usuario. <br>
• Llama al método correspondiente.

<br>
Beneficios de esta organización

• Separación clara de responsabilidades. <br>
• Código más limpio y ordenado. <br>
• Mayor facilidad para hacer mejoras. <br>
• Programa más profesional.

<br> <br>
### Parte 3 – Validaciones y Manejo de Excepciones

En el programa original podían ocurrir errores como:

• Ingresar texto cuando se esperaba un número. <br>
• Ingresar una calificación fuera del rango permitido. <br>
• Calcular promedio sin estudiantes registrados. <br>
• Buscar la calificación más alta sin datos.

<br>
Mejoras implementadas

• Uso de try-catch para evitar fallos por entradas incorrectas. <br>
• Métodos leerEntero() y leerDouble() para validar datos. <br>
• Validación del rango de calificaciones (0 a 100). <br>
• Verificación de listas vacías antes de operar. 

<br>
Importancia de las validaciones

• Evitan que el programa se cierre inesperadamente. <br>
• Mejoran la experiencia del usuario. <br>
• Hacen el sistema más seguro y confiable. 

<br> <br>
### Parte 4 – Preguntas de Reflexión
<br>
¿Qué ventajas tiene dividir el código en métodos?

• Mejor organización. <br>
• Mayor claridad. <br>
• Reutilización del código. <br>
• Facilidad para encontrar errores. <br>
• Mejor mantenimiento.

<br>
¿Por qué no es recomendable usar muchas variables globales?

• Pueden modificarse desde cualquier parte del programa. <br>
• Generan dependencia entre métodos. <br>
• Dificultan la detección de errores. <br>
• Aumentan el riesgo de fallos inesperados.

<br>
¿Cómo mejora la modularización la legibilidad?

• Divide el programa en partes pequeñas y claras. <br>
• Cada método tiene un nombre descriptivo. <br>
• Permite entender rápidamente qué hace cada sección. <br>
• Hace el código más fácil de leer.

<br> <br>
## Conclusión

La modularización permitió reorganizar el programa en métodos específicos, mejorar la estructura del código y agregar validaciones que hacen el sistema más seguro y estable.

El programa final es más claro, más ordenado y más fácil de mantener que la versión original.

<br>
