## 👨🏽‍🏫 Clase M3 AE4: Manejo de valores perdidos y outliers

### 📌 Introducción

En esta clase se estudian técnicas para detectar y manejar valores faltantes (nulos) y valores atípicos (outliers) en conjuntos de datos, pasos fundamentales para asegurar la calidad y confiabilidad del análisis.

---

### 🧱 Valores perdidos (Missing Data)

- Se identifican con funciones como `isnull()` o `isna()`.
- Métodos para tratarlos:
  - **Eliminación:** `dropna()` elimina filas o columnas con valores nulos.
  - **Imputación:** `fillna()` rellena valores faltantes con medias, medianas, modas u otros valores.

---

### ⚠️ Outliers (Valores atípicos)

- Son datos que se alejan significativamente del resto y pueden distorsionar análisis.
- Métodos comunes para detectarlos:
  - Estadísticas descriptivas (cuartiles, rango intercuartílico).
  - Visualización con boxplots.
- Técnicas para tratarlos:
  - Eliminación.
  - Transformaciones (logaritmos, normalización).
  - Reemplazo con valores más representativos.

---

### 🧪 Ejemplo básico

```python
import pandas as pd
import numpy as np

# Crear DataFrame con valores nulos y outliers
df = pd.DataFrame({
    'A': [1, 2, np.nan, 4, 5, 100],
    'B': [5, np.nan, 7, 8, 9, 10]
})

# Detectar valores nulos
print(df.isnull().sum())

# Rellenar valores nulos con la media de la columna A
df['A'] = df['A'].fillna(df['A'].mean())

# Detectar outliers (ejemplo simple con rango intercuartílico)
Q1 = df['A'].quantile(0.25)
Q3 = df['A'].quantile(0.75)
IQR = Q3 - Q1
outliers = df[(df['A'] < Q1 - 1.5 * IQR) | (df['A'] > Q3 + 1.5 * IQR)]
print("Outliers:\n", outliers)
