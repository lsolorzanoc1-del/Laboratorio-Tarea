Laboratorio-Tarea
<br>
Ejercicio en Clase 3 – Modularización en Java

Curso: Programación 1
<br>
Parte 1 – Análisis del Programa Original

En el programa original se observó que todo el código estaba concentrado dentro del método main.

Dentro de este método se realizaban todas las tareas del sistema:

<br>

• Agregar estudiante
• Mostrar estudiantes
• Calcular promedio
• Buscar la calificación más alta
• Mostrar el menú

<br>

Cada una de estas tareas cumple una función específica, por lo tanto pueden convertirse en métodos independientes.

<br>
 Validaciones repetitivas detectadas

• Verificar si las listas están vacías.
• Conversión de texto a números sin control de errores.

<br>
 ¿Por qué dividir estas tareas mejora el programa?

• Hace el código más organizado.
• Permite reutilizar métodos.
• Facilita el mantenimiento.
• Reduce la posibilidad de errores.
• Mejora la legibilidad del programa.

<br> <br>
 Variables Locales vs Globales
<br>
 Variables Globales (static)
static List<String> estudiantes;
static List<Double> calificaciones;

Se dejaron como globales porque:

• Representan los datos principales del sistema.
• Son utilizadas en varios métodos.
• Deben mantenerse disponibles durante toda la ejecución.

<br>
 Variables Locales

Ejemplos:

• Scanner scanner
• int opcion
• double suma
• double promedio
• double calificacion

<br>

Se declararon dentro de los métodos porque:

• Solo se usan en una parte específica del programa.
• Reducen el riesgo de modificar datos accidentalmente.
• Mejoran la seguridad y claridad del código.

<br> <br>
Parte 2 – Modularización del Programa

Para mejorar la estructura del programa se dividió el código en métodos específicos, cada uno con una sola responsabilidad.

<br>
Métodos creados:

• mostrarMenu()
• agregarEstudiante()
• mostrarEstudiantes()
• calcularPromedio()
• mostrarMejorEstudiante()
• leerEntero()
• leerDouble()

<br>

Ahora el método main únicamente:

• Muestra el menú.
• Lee la opción del usuario.
• Llama al método correspondiente.

<br>
Beneficios de esta organización

• Separación clara de responsabilidades.
• Código más limpio y ordenado.
• Mayor facilidad para hacer mejoras.
• Programa más profesional.

<br> <br>
Parte 3 – Validaciones y Manejo de Excepciones

En el programa original podían ocurrir errores como:

• Ingresar texto cuando se esperaba un número.
• Ingresar una calificación fuera del rango permitido.
• Calcular promedio sin estudiantes registrados.
• Buscar la calificación más alta sin datos.

<br>
Mejoras implementadas

• Uso de try-catch para evitar fallos por entradas incorrectas.
• Métodos leerEntero() y leerDouble() para validar datos.
• Validación del rango de calificaciones (0 a 100).
• Verificación de listas vacías antes de operar.

<br>
Importancia de las validaciones

• Evitan que el programa se cierre inesperadamente.
• Mejoran la experiencia del usuario.
• Hacen el sistema más seguro y confiable.

<br> <br>
Parte 4 – Preguntas de Reflexión
<br>
¿Qué ventajas tiene dividir el código en métodos?

• Mejor organización.
• Mayor claridad.
• Reutilización del código.
• Facilidad para encontrar errores.
• Mejor mantenimiento.

<br>
¿Por qué no es recomendable usar muchas variables globales?

• Pueden modificarse desde cualquier parte del programa.
• Generan dependencia entre métodos.
• Dificultan la detección de errores.
• Aumentan el riesgo de fallos inesperados.

<br>
¿Cómo mejora la modularización la legibilidad?

• Divide el programa en partes pequeñas y claras.
• Cada método tiene un nombre descriptivo.
• Permite entender rápidamente qué hace cada sección.
• Hace el código más fácil de leer.

<br> <br>
Conclusión

La modularización permitió reorganizar el programa en métodos específicos, mejorar la estructura del código y agregar validaciones que hacen el sistema más seguro y estable.

El programa final es más claro, más ordenado y más fácil de mantener que la versión original.

<br>
