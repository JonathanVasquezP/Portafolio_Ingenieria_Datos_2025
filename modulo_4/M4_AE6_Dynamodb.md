# ⚡ Amazon DynamoDB

## 📌 ¿Qué es DynamoDB?

Amazon DynamoDB es un servicio de base de datos NoSQL totalmente administrado por AWS. Está diseñado para ofrecer alto rendimiento, baja latencia y escalabilidad automática sin necesidad de gestionar servidores o infraestructura.

---

## 🧠 Características Principales

- **Modelo clave-valor y de documentos:** DynamoDB combina ambos modelos, permitiendo almacenar datos estructurados y semi-estructurados.
- **Totalmente administrado:** AWS se encarga del aprovisionamiento, configuración, escalabilidad, replicación y respaldo.
- **Escalabilidad automática:** Se ajusta de manera automática al volumen de datos y tráfico de consultas.
- **Latencia baja en milisegundos:** Ideal para aplicaciones en tiempo real.
- **Soporte de transacciones:** Permite operaciones ACID entre múltiples elementos.

---

## 🧩 Componentes Clave

- **Tablas:** Contenedores principales de datos en DynamoDB.
- **Ítems:** Equivalentes a filas, son las unidades de datos individuales.
- **Atributos:** Equivalentes a columnas, pueden ser tipos simples o complejos.
- **Clave primaria:** Obligatoria; puede ser una sola clave (clave de partición) o compuesta (clave de partición + clave de ordenamiento).
- **Índices secundarios:** Para permitir consultas adicionales fuera de la clave primaria.
- **Throughput:** Capacidad de lectura/escritura provisionada o bajo demanda.

---

## 🎯 ¿Cuándo usar DynamoDB?

- Cuando se requiere **alta disponibilidad y tolerancia a fallos**.
- Para aplicaciones que manejan **grandes volúmenes de datos** con accesos frecuentes.
- Si necesitas **latencias constantes** y rápidas.
- Cuando prefieres un enfoque **serverless** sin administrar la infraestructura de base de datos.
- Si trabajas dentro del ecosistema de **AWS**.

---

## 💼 Casos de uso comunes

- **Aplicaciones móviles y web:** Almacenamiento de perfiles de usuario, configuración de sesiones y preferencias.
- **Sistemas de gestión de catálogos:** Ideal para e-commerce con millones de productos y filtros dinámicos.
- **Juegos en línea:** Registro de jugadores, puntuaciones y estados de juego en tiempo real.
- **Sistemas de recomendación:** Donde se necesita velocidad de lectura para personalización.
- **IoT y sensores:** Captura continua de datos con almacenamiento flexible y sin interrupciones.
- **Plataformas de mensajería y notificaciones:** Manejo de colas de mensajes y estados de entrega.

---

## ⚖️ Ventajas

- Escalabilidad automática sin intervención manual.
- Latencia consistente y baja, incluso con millones de transacciones por segundo.
- Alta disponibilidad con replicación en múltiples zonas de disponibilidad.
- Integración nativa con otros servicios AWS como Lambda, API Gateway, CloudWatch, etc.

---

## ⚠️ Desventajas

- El modelo de datos debe estar bien diseñado desde el inicio para evitar cuellos de botella.
- Costos pueden crecer si no se controla el throughput o los accesos frecuentes.
- Limitaciones en la cantidad de operaciones complejas o uniones de datos.
- La curva de aprendizaje puede ser empinada al trabajar con índices secundarios o particiones.

---

## 🛠️ Recomendaciones

- Define cuidadosamente la clave primaria y los patrones de acceso.
- Usa índices secundarios cuando se requieran consultas adicionales.
- Habilita el modo de capacidad bajo demanda si el tráfico es variable.
- Monitorea el rendimiento y utiliza alertas para optimizar el costo y rendimiento.
