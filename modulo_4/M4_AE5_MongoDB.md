# 🍃 MongoDB

## 📌 ¿Qué es MongoDB?

MongoDB es una base de datos NoSQL orientada a documentos que almacena la información en formato BSON (una representación binaria de JSON). Es ampliamente utilizada por su flexibilidad, escalabilidad y facilidad de uso en entornos de desarrollo modernos.

---

## 🧠 Características Principales

- **Modelo de documentos:** Almacena los datos como documentos similares a JSON, permitiendo estructuras anidadas y dinámicas.
- **Esquema flexible:** No requiere una estructura fija de columnas, lo que facilita la evolución del modelo de datos.
- **Escalabilidad horizontal:** Soporta particionado automático (sharding) para distribuir datos en múltiples servidores.
- **Alta disponibilidad:** Permite replicación de datos entre nodos para tolerancia a fallos.
- **Consultas poderosas:** A través de una sintaxis intuitiva basada en documentos.

---

## 🧩 Componentes Clave

- **Documentos:** Unidades básicas de datos, representadas en formato BSON.
- **Colecciones:** Conjuntos de documentos relacionados (equivalente a una tabla en bases relacionales).
- **Bases de datos:** Conjunto de colecciones.
- **Replica Sets:** Conjunto de instancias que aseguran redundancia y alta disponibilidad.
- **Sharding:** Método de particionamiento horizontal para manejar grandes volúmenes de datos.

---

## 🎯 ¿Cuándo usar MongoDB?

- Cuando se necesita una **estructura de datos flexible** y en constante evolución.
- En aplicaciones con **altos volúmenes de lectura/escritura**.
- Para soluciones web, móviles, analítica en tiempo real, IoT o sistemas de contenido.
- Cuando la **escalabilidad horizontal** y la tolerancia a fallos son clave.

---

## 💼 Casos de uso comunes

- **Plataformas de comercio electrónico:** Almacenan productos, carritos y órdenes con esquemas variados según el tipo de ítem o usuario.
- **Aplicaciones móviles:** Manejan datos de usuario, configuraciones y notificaciones sin estructura fija.
- **Sistemas de gestión de contenido (CMS):** Donde los tipos de contenido cambian y evolucionan frecuentemente.
- **Sistemas de geolocalización:** Almacenan datos espaciales que requieren flexibilidad y alta velocidad de consulta.
- **Aplicaciones en tiempo real:** Como chats, redes sociales o dashboards con actualizaciones constantes.
- **Internet de las cosas (IoT):** Captura y almacena datos de sensores y dispositivos con estructuras cambiantes.

---

## ⚖️ Ventajas

- Alta velocidad de desarrollo por su modelo sin esquemas fijos.
- Fácil integración con aplicaciones modernas y APIs REST.
- Replicación automática y balanceo de carga.
- Amplio ecosistema y soporte para múltiples lenguajes de programación.

---

## ⚠️ Desventajas

- No es ideal para operaciones complejas con relaciones entre entidades.
- Las consultas pueden ser menos eficientes si no se diseñan índices adecuados.
- Puede requerir más memoria RAM para optimizar el rendimiento.

---

## 🛠️ Recomendaciones

- Diseña los documentos pensando en las consultas más frecuentes.
- Indexa los campos usados en búsquedas para mejorar el rendimiento.
- Utiliza replica sets para asegurar la disponibilidad del sistema.
- Planifica el uso de sharding si esperas crecimiento masivo de datos.
