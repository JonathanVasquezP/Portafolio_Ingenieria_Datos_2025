## 👨🏽‍🏫 Clase M3 AE3: Obtención de datos desde archivos

### 📌 Introducción

En esta clase se aborda cómo cargar datos desde diferentes tipos de archivos usando Pandas, una habilidad esencial para la preparación y análisis de datos. Se aprende a importar datos desde CSV, Excel y otras fuentes para integrarlos en DataFrames de Pandas.

---

### 🧱 Formatos de archivo comunes

- **CSV:** Archivos de texto separados por comas, fáciles de manejar y muy utilizados.
- **Excel:** Archivos con múltiples hojas que permiten organizar datos complejos.
- **JSON, HTML, SQL:** Otros formatos que Pandas puede manejar para obtener datos.

---

### ⚙️ Funciones clave para cargar datos

- `pd.read_csv('archivo.csv')`: Carga datos desde un archivo CSV.
- `pd.read_excel('archivo.xlsx')`: Carga datos desde un archivo Excel.
- `pd.read_html('url_o_archivo')`: Extrae tablas de páginas web.
- `pd.read_json()`, `pd.read_sql()` para otros formatos.

---

### 🧪 Ejemplo básico

```python
import pandas as pd

# Cargar archivo CSV
df_csv = pd.read_csv('datos.csv')

# Cargar archivo Excel
df_excel = pd.read_excel('datos.xlsx')

# Cargar tabla desde página web
tablas = pd.read_html('https://es.wikipedia.org/wiki/Anexo:Países_por_población')
df_web = tablas[0]  # Primera tabla encontrada

# Mostrar primeras filas
print(df_csv.head())
print(df_excel.head())
print(df_web.head())
