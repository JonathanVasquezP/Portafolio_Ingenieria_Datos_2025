# 🗄️ Apache Cassandra

## 📌 ¿Qué es Cassandra?

Apache Cassandra es una base de datos NoSQL distribuida, diseñada para manejar grandes volúmenes de datos en múltiples servidores sin un punto único de falla. Fue creada por Facebook y luego liberada como proyecto de código abierto bajo la Apache Software Foundation.

---

## 🧠 Características Principales

- **Modelo de datos basado en columnas:** A diferencia de las bases relacionales, Cassandra almacena los datos por columnas, no por filas.
- **Alta disponibilidad:** Ofrece replicación de datos entre nodos, permitiendo tolerancia a fallos sin detener el sistema.
- **Escalabilidad horizontal:** Permite añadir nodos fácilmente sin afectar el rendimiento.
- **Sin maestro (Masterless):** Todos los nodos tienen el mismo rol, lo que mejora la resiliencia y la distribución de carga.
- **Lenguaje CQL (Cassandra Query Language):** Inspirado en SQL, pero adaptado a su modelo NoSQL.

---

## 🧩 Arquitectura de Cassandra

- **Nodos:** Cada máquina en el clúster es un nodo, donde se almacenan los datos.
- **Clúster:** Conjunto de nodos trabajando juntos.
- **Keyspace:** Equivalente a una base de datos; define la replicación.
- **Tabla:** Define el esquema de los datos por columnas.
- **Particiones:** Los datos se distribuyen en el clúster por clave de partición.

---

## 🎯 ¿Cuándo usar Cassandra?

- Cuando se necesita **escritura rápida a gran escala**.
- En aplicaciones que requieren **alta disponibilidad 24/7**.
- Para manejar **grandes volúmenes de datos distribuidos geográficamente**.
- En escenarios de **IoT, análisis de logs, redes sociales y telecomunicaciones**.

---

## ⚖️ Ventajas

- Alta tolerancia a fallos sin pérdida de disponibilidad.
- Escritura eficiente en grandes cantidades.
- Escalabilidad horizontal sin interrupciones.
- Diseño ideal para entornos distribuidos.

---

## ⚠️ Desventajas

- No es óptima para consultas complejas o agregaciones como JOINs.
- Requiere un buen diseño de clave de partición para evitar cuellos de botella.
- Mayor complejidad operativa que otras bases de datos tradicionales.

---

## 🛠️ Recomendaciones

- Planifica cuidadosamente el **modelo de datos** desde el inicio.
- Usa claves de partición bien distribuidas para evitar hotspots.
- Aprovecha la **replicación configurable** según las necesidades de consistencia y disponibilidad.

