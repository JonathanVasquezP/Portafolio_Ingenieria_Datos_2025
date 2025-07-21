## 👨🏽‍🏫 Clase M3 AE6: Agrupamiento y pivoteo de datos

### 📌 Introducción

Esta clase aborda técnicas para agrupar datos y transformar su estructura utilizando funciones como `groupby()`, `pivot()` y `pivot_table()` en Pandas, facilitando análisis resumidos y visualizaciones.

---

### 🧱 Conceptos clave

- **Agrupamiento (`groupby`)**: Permite segmentar datos según una o más columnas y aplicar funciones de agregación (suma, media, conteo).
- **Pivoteo (`pivot`)**: Reestructura datos de formato largo a ancho, reorganizando filas y columnas.
- **Tabla dinámica (`pivot_table`)**: Similar a `pivot`, pero permite agregar valores cuando hay duplicados, usando funciones como suma o promedio.

---

### ⚙️ Funciones principales

- `df.groupby('columna').agg({'otra_col': 'función'})`
- `df.pivot(index='fila', columns='columna', values='valor')`
- `df.pivot_table(index='fila', columns='columna', values='valor', aggfunc='función')`

---

### 🧪 Ejemplo básico

```python
import pandas as pd

# Crear DataFrame de ejemplo
data = {
    'Ciudad': ['A', 'A', 'B', 'B', 'C', 'C'],
    'Mes': ['Enero', 'Febrero', 'Enero', 'Febrero', 'Enero', 'Febrero'],
    'Ventas': [100, 150, 200, 250, 300, 350]
}

df = pd.DataFrame(data)

# Agrupar por Ciudad y calcular suma de ventas
grouped = df.groupby('Ciudad').agg({'Ventas': 'sum'})

# Crear tabla pivote
pivot = df.pivot(index='Ciudad', columns='Mes', values='Ventas')

print("Agrupamiento:\n", grouped)
print("\nTabla pivote:\n", pivot)
