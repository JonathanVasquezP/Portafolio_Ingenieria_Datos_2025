## 👨🏽‍🏫 Clase M2 AE2: Sentencias básicas del lenguaje Python

### Introducción

Las sentencias condicionales constituyen el fundamento para el control del flujo en la programación. Gracias a ellas, un programa puede tomar decisiones basadas en condiciones específicas, permitiendo que diferentes bloques de código se ejecuten según los datos o eventos que se presenten durante la ejecución. Esto dota a los programas de flexibilidad y capacidad para adaptarse a distintos escenarios.

En Python, estas estructuras se manejan principalmente con las sentencias `if`, `elif` y `else`, que evalúan expresiones lógicas para determinar el camino a seguir. Además, combinan operadores relacionales y lógicos que permiten construir condiciones precisas y complejas.

---

### 1. Estructuras condicionales en Python

- **Sentencia `if`**: Evalúa una condición booleana (que puede ser el resultado de una comparación o expresión lógica). Si el resultado es `True`, el bloque indentado que le sigue se ejecuta.
- **Sentencia `elif`**: Se utiliza para evaluar condiciones adicionales cuando la condición del `if` es `False`. Puede haber múltiples `elif` encadenados para verificar distintas alternativas.
- **Sentencia `else`**: Captura todos los casos que no hayan cumplido ninguna condición anterior, funcionando como una especie de “última alternativa” o “caso por defecto”.

---

### 2. Operadores relacionales

Estos operadores comparan valores y devuelven un resultado booleano (`True` o `False`), esencial para la evaluación en condicionales:

| Operador | Descripción         |
| -------- | ------------------- |
| `==`     | Igualdad            |
| `!=`     | Diferente           |
| `<`      | Menor que           |
| `>`      | Mayor que           |
| `<=`     | Menor o igual que   |
| `>=`     | Mayor o igual que   |

---

### 3. Operadores lógicos

Para combinar múltiples condiciones, Python dispone de operadores lógicos:

- **`and`**: Retorna `True` solo si ambas condiciones son `True`.  
- **`or`**: Retorna `True` si al menos una de las condiciones es `True`.  
- **`not`**: Invierte el valor lógico de una condición (`True` a `False` y viceversa).  

---

### 4. Precedencia y uso de paréntesis

Los operadores tienen reglas de precedencia (orden de evaluación). Para evitar confusión o errores lógicos, es recomendable usar paréntesis para agrupar condiciones, facilitando la lectura y garantizando que las expresiones se evalúen en el orden esperado.

---

### 5. Entrada y normalización de datos

- La función `input()` recibe datos del usuario como texto (`str`).
- Para comparar cadenas con condiciones, es importante normalizar el texto (eliminar espacios en blanco, unificar mayúsculas/minúsculas).
- Métodos útiles:
  - `strip()`: elimina espacios al inicio y final.
  - `lower()`, `upper()`, `capitalize()`: convierten el texto a minúsculas, mayúsculas o capitalizado para uniformidad.

---

### 6. Buenas prácticas y recomendaciones

- **Validar entrada:** Siempre verificar que la entrada del usuario sea del tipo esperado para evitar errores (ejemplo: que la edad sea un número entero).
- **Control de errores:** Implementar manejo de excepciones para casos donde la conversión de tipos falle (por ejemplo, si el usuario ingresa texto en lugar de un número).
- **Claridad y legibilidad:** Escribir condiciones claras y separarlas en variables auxiliares si son muy complejas.
- **Comentarios:** Documentar el código para explicar la lógica detrás de cada decisión.
- **Normalización:** Estandarizar datos antes de evaluarlos para evitar errores por diferencias en mayúsculas/minúsculas o espacios.
- **Modularidad:** Usar funciones para organizar el código y facilitar la reutilización y pruebas.

---

### 7. Conceptos complementarios

- **Booleanos:** El tipo `bool` en Python sólo puede ser `True` o `False`. Se usan para controlar la lógica en las sentencias condicionales.
- **Expresiones booleanas:** Son combinaciones de operadores relacionales y lógicos que retornan un valor booleano.
- **Cortocircuito:** En expresiones con `and` y `or`, Python detiene la evaluación tan pronto se pueda determinar el resultado final, lo que puede optimizar el rendimiento y evitar errores.

---

### 8. Resumen

Las sentencias condicionales son una piedra angular en la construcción de programas dinámicos y adaptativos. Dominar las sentencias `if`, `elif` y `else`, junto con los operadores relacionales y lógicos, permite construir lógica compleja de manera clara y eficiente. Además, el manejo adecuado de la entrada del usuario y la normalización de datos asegura que los programas sean robustos y fáciles de mantener.

Esta clase sienta las bases para que puedas avanzar en el desarrollo de programas que requieran toma de decisiones, condición y control de flujo, fundamentales en todo proyecto de programación e ingeniería de datos.

---
