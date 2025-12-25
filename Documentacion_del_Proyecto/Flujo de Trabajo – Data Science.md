# 📊 Flujo de Trabajo – Data Science

## Objetivo

Definir de forma clara y ordenada el **flujo completo de trabajo del equipo de Data Science**, dejando el resultado listo para su consumo por el equipo de Back-end.

---

## 🔹 Etapas del Proceso de Data Science

### 1️⃣ Definición del problema

* Identificación del problema a resolver.
* Planteamiento del objetivo del modelo.

### 2️⃣ Comprensión del negocio

* Análisis del contexto de negocio.
* Entendimiento del impacto del modelo en la toma de decisiones.

### 3️⃣ Definición del dataset

* Identificación de las fuentes de datos.
* Definición de variables disponibles y variable objetivo.

### 4️⃣ Carga de datos

* Importación de datos desde archivos o bases de datos.
* Validación inicial de estructura y tipos de datos.

### 5️⃣ Exploración de datos (EDA)

* Análisis estadístico descriptivo.
* Visualización de distribuciones y relaciones.
* Detección de valores nulos y outliers.

### 6️⃣ Limpieza y preparación de datos

* Tratamiento de valores faltantes.
* Corrección de inconsistencias.
* Normalización y/o estandarización.

### 7️⃣ Ingeniería de características (Feature Engineering)

* Creación de nuevas variables.
* Transformación de variables existentes.

### 8️⃣ Selección de variables (X / y)

* Definición de variables independientes (X).
* Definición de la variable objetivo (y).

### 9️⃣ División de datos (Train / Test)

* Separación del conjunto de entrenamiento y prueba.
* Validación de proporciones y balance de clases.

### 🔟 Selección del modelo

* Definición de algoritmos candidatos.
* Selección inicial basada en el problema.

### 1️⃣1️⃣ Entrenamiento del modelo

* Entrenamiento del modelo seleccionado.
* Ajuste inicial de parámetros.

### 1️⃣2️⃣ Evaluación del modelo

* Uso de métricas adecuadas (Accuracy, Precision, Recall, F1, AUC).
* Análisis de resultados.

### 1️⃣3️⃣ Ajuste del umbral de decisión

* Optimización del umbral según métricas de negocio.
* Evaluación de trade-offs.

### 1️⃣4️⃣ Prueba de predicción individual

* Validación del modelo con registros individuales.
* Verificación de salidas esperadas.

### 1️⃣5️⃣ Validación del contrato de entrada

* Definición del formato de entrada.
* Validación de tipos, orden y valores esperados.

### 1️⃣6️⃣ Serialización del modelo

* Guardado del modelo entrenado (`.pkl` / `.joblib`).
* Serialización del pipeline de preprocesamiento.

### 1️⃣7️⃣ Documentación para Back-end

* Descripción del flujo del modelo.
* Definición de inputs y outputs.
* Métricas finales y consideraciones de uso.

---

## 🚧 Fin del Alcance de Data Science

El equipo de Back-end continúa con la integración, despliegue y consumo del modelo.

---

## 👤 Autor

Oscar Rubio
Data Science | Ingeniería en Gestión de Tecnologías de la Información
