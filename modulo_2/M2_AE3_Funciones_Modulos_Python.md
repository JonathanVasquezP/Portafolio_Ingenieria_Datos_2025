## 👨🏽‍🏫 Clase M2 AE3: Funciones y módulos en Python

### Introducción

Las funciones son bloques de código reutilizables que realizan una tarea específica y pueden recibir entradas y devolver salidas. Permiten organizar el código, reducir la repetición, mejorar la legibilidad y facilitar el mantenimiento. En Python, las funciones se definen usando la palabra clave `def` seguida de un nombre y parámetros opcionales.

Los módulos son archivos que contienen definiciones y funciones, y se usan para organizar el código en unidades independientes y reutilizables. Importar módulos permite acceder a funciones y variables definidas en otros archivos o en la biblioteca estándar de Python, promoviendo la modularidad y la colaboración en proyectos.

---

### 1. Funciones en Python

- Definición: Una función es un bloque de código con un nombre que puede ser invocado para ejecutar su contenido.
- Parámetros y argumentos: Las funciones pueden recibir información mediante parámetros y devolver resultados.
- Retorno de valores: Se puede usar `return` para devolver un valor desde una función.
- Ventajas:
  - Reutilización de código.
  - Mejor organización y claridad.
  - Facilita la depuración y pruebas.

---

### 2. Ámbito de variables (Scope)

- Las variables definidas dentro de una función tienen un ámbito local y no son accesibles fuera de ella.
- Variables definidas fuera de funciones son globales, accesibles desde cualquier parte del código.
- Es importante manejar correctamente los ámbitos para evitar errores y comportamientos inesperados.

---

### 3. Módulos en Python

- Un módulo es un archivo `.py` que contiene funciones, clases o variables.
- Permite organizar el código en partes lógicas y separadas.
- Se pueden importar módulos estándar (como `math`, `random`) o propios creados por el usuario.
- El uso de módulos facilita el mantenimiento, la colaboración y la reutilización en proyectos grandes.

---

### 4. Importación de módulos

- Para usar funciones o clases de un módulo, se importa con la palabra clave `import`.
- Existen varias formas:
  - `import modulo`
  - `from modulo import funcion`
  - `import modulo as alias`
- La elección depende del contexto y la claridad del código.

---

### 5. Buenas prácticas

- Nombrar funciones y módulos con nombres descriptivos y en minúsculas, separando palabras con guiones bajos (`snake_case`).
- Documentar funciones con docstrings para explicar su propósito, parámetros y valores de retorno.
- Mantener funciones cortas y enfocadas en una tarea concreta.
- Organizar módulos por funcionalidad y evitar que sean demasiado extensos.
- Reutilizar módulos en lugar de duplicar código.

---

### 6. Ventajas de modularizar el código

- Facilita la lectura y el mantenimiento.
- Permite trabajar en equipo con mayor eficiencia.
- Reduce errores y facilita pruebas unitarias.
- Incrementa la escalabilidad y adaptabilidad del proyecto.

---

### 7. Resumen

El manejo adecuado de funciones y módulos es esencial para construir programas Python eficientes, claros y sostenibles. Las funciones encapsulan lógica específica que puede ser reutilizada y probada aisladamente, mientras que los módulos organizan estas funciones en unidades cohesivas, fomentando la modularidad y la colaboración en proyectos de cualquier tamaño.

Dominar estos conceptos te preparará para desarrollar aplicaciones más complejas y profesionales en ingeniería de datos y programación en general.

---
