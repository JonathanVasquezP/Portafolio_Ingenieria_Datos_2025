## 👨🏽‍🏫 Clase M3 AE2: La librería Pandas

### 📌 Introducción

Pandas es una biblioteca de Python especializada en la manipulación y análisis de datos. Proporciona estructuras de datos flexibles y eficientes como `Series` y `DataFrame`, ideales para trabajar con datos tabulares.

---

### 🧱 Estructuras principales

- **Series:** Estructura unidimensional similar a un arreglo con etiquetas.
- **DataFrame:** Tabla bidimensional con filas y columnas etiquetadas, similar a una hoja de cálculo.

---

### ⚙️ Funcionalidades básicas

- Carga de datos desde archivos CSV, Excel y bases de datos.
- Selección y filtrado de datos.
- Manejo de valores nulos con funciones como `isnull()`, `fillna()` y `dropna()`.
- Agrupamiento y agregación de datos con `groupby()`.
- Transformación y reestructuración de datos con `pivot()`, `melt()` y `pivot_table()`.

---

### 🧪 Ejemplo básico

```python
import pandas as pd

# Crear una Serie
serie = pd.Series([10, 20, 30], index=['a', 'b', 'c'])

# Crear un DataFrame
datos = {'Nombre': ['Ana', 'Luis', 'Carlos'], 'Edad': [25, 30, 22]}
df = pd.DataFrame(datos)

# Mostrar DataFrame
print(df)
