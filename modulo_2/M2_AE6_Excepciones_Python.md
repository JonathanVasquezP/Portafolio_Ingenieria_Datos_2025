## 👨🏽‍🏫 Clase M2 AE6: Excepciones en Python

### Introducción

Las excepciones son mecanismos que permiten manejar errores y situaciones inesperadas que pueden ocurrir durante la ejecución de un programa. Python proporciona estructuras para detectar, capturar y responder a estos errores, mejorando la robustez y la experiencia del usuario.

---

### 1. Concepto de excepciones

- Una excepción es un evento que interrumpe el flujo normal del programa debido a un error o situación excepcional.  
- Cuando ocurre una excepción y no se maneja, el programa termina abruptamente con un mensaje de error.

---

### 2. Manejo de excepciones

- El manejo se realiza mediante bloques `try-except` que permiten capturar excepciones específicas y ejecutar código alternativo.  
- La estructura básica es:

  ```python
  try:
      # código que puede generar una excepción
  except TipoDeError:
      # código para manejar la excepción

Es posible capturar múltiples excepciones usando varios bloques `except`.

### 3. Bloques adicionales

- `else`: Se ejecuta si no ocurre ninguna excepción en el bloque `try`.
- `finally`: Se ejecuta siempre, ocurra o no una excepción, ideal para liberar recursos o limpieza.

### 4. Creación de excepciones personalizadas

- Se pueden definir clases de excepciones propias heredando de la clase base `Exception`.
- Esto permite crear errores específicos del dominio de la aplicación y manejarlos adecuadamente.

### 5. Buenas prácticas en el manejo de excepciones

- Capturar solo las excepciones que se esperan y se pueden manejar.
- No usar excepciones para controlar el flujo normal del programa.
- Proporcionar mensajes claros y útiles para el usuario o para el registro de errores.
- Utilizar el bloque `finally` para asegurar la liberación de recursos.
- Documentar las excepciones que una función puede lanzar.

### 6. Ventajas del manejo de excepciones

- Incrementa la robustez y estabilidad de los programas.
- Facilita la detección y corrección de errores.
- Mejora la experiencia del usuario al evitar cierres inesperados.
- Permite separar la lógica de manejo de errores del código principal.

### 7. Resumen

El manejo adecuado de excepciones es crucial para desarrollar aplicaciones confiables y profesionales en Python. Permite anticipar y gestionar errores, asegurando que el programa pueda continuar o finalizar de manera controlada, mejorando la calidad y mantenibilidad del software.
