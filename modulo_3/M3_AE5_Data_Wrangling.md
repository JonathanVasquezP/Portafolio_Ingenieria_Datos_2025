## 👨🏽‍🏫 Clase M3 AE5: Data Wrangling

### 📌 Introducción

Data Wrangling es el proceso de limpiar, transformar y preparar datos crudos para análisis. Esta clase se enfoca en técnicas para organizar y optimizar datasets, asegurando su calidad y utilidad.

---

### 🧱 Técnicas principales

- Detección y manejo de valores nulos y duplicados.
- Transformación de datos categóricos a numéricos.
- Uso de funciones como `groupby()`, `agg()` y mapeo para resumir datos.
- Filtrado, ordenamiento y reorganización de DataFrames para facilitar el análisis.

---

### ⚙️ Funciones útiles

- `dropna()`, `fillna()` para valores faltantes.
- `drop_duplicates()` para eliminar registros repetidos.
- `map()` y `apply()` para transformar datos.
- `groupby()` y `agg()` para agregaciones.
- `sort_values()` para ordenar.

---

### 🧪 Ejemplo básico

```python
import pandas as pd

# Crear DataFrame de ejemplo
data = {'Categoria': ['A', 'B', 'A', 'C', 'B', 'A'],
        'Valor': [10, 20, None, 30, 20, 10],
        'Cantidad': [1, 2, 1, 3, 2, 1]}

df = pd.DataFrame(data)

# Imputar valores nulos con la media
df['Valor'] = df['Valor'].fillna(df['Valor'].mean())

# Eliminar duplicados
df = df.drop_duplicates()

# Agrupar y sumar valores por categoría
df_grouped = df.groupby('Categoria').agg({'Valor': 'mean', 'Cantidad': 'sum'})

print(df_grouped)
