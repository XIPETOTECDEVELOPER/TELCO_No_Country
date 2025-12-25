# 📊 Alcance del Proyecto – Data Science

## Objetivo
Definir **exclusivamente las responsabilidades y entregables del equipo de Data Science**, dejando el desarrollo posterior en manos del equipo de Backend.

Este documento delimita claramente hasta dónde llega el trabajo de Data Science y a partir de qué punto continúa Backend.

---

## 🔹 Alcance del Equipo de Data Science

### 1️⃣ Comprensión del problema
- Definición del objetivo del modelo (ej. predicción de churn).
- Identificación de la variable objetivo (*target*).
- Entendimiento del contexto del negocio y sus necesidades.

---

### 2️⃣ Recolección y carga de datos
- Identificación de fuentes de datos.
- Carga de datasets en formato estructurado (CSV, SQL, etc.).
- Validación inicial de integridad y consistencia de los datos.

---

### 3️⃣ Análisis Exploratorio de Datos (EDA)
- Análisis estadístico descriptivo.
- Identificación de valores nulos.
- Detección de outliers.
- Análisis de correlaciones.
- Visualización de distribuciones y relaciones entre variables.

---

### 4️⃣ Limpieza y preprocesamiento
- Tratamiento de valores faltantes.
- Codificación de variables categóricas.
- Normalización y/o estandarización de variables numéricas.
- Balanceo de clases (si aplica).

---

### 5️⃣ Ingeniería de características (Feature Engineering)
- Creación de nuevas variables relevantes.
- Selección de variables con mayor impacto.
- Eliminación de características redundantes o irrelevantes.

---

### 6️⃣ Selección y entrenamiento de modelos
- Definición de modelos candidatos.
- Entrenamiento inicial de cada modelo.
- Comparación de desempeño entre modelos.

---

### 7️⃣ Evaluación del modelo
- Definición de métricas de evaluación (Accuracy, Precision, Recall, F1-score, AUC).
- Evaluación sobre conjunto de prueba.
- Interpretación de resultados.

---

### 8️⃣ Optimización del modelo
- Ajuste de hiperparámetros.
- Mejora del desempeño del modelo.
- Selección del modelo final.

---

### 9️⃣ Entregables para el equipo de Backend
- Modelo entrenado serializado (`.pkl` o `.joblib`).
- Pipeline de preprocesamiento.
- Diccionario de variables (features).
- Recomendaciones de uso del modelo.
- Métricas finales documentadas.

---

### 🔟 Documentación técnica
- Descripción del flujo de datos.
- Supuestos del modelo.
- Limitaciones conocidas.
- Requisitos de entrada y salida del modelo.

---

## 🚧 Fin del Alcance de Data Science
A partir de este punto:

- ❌ No se implementa API
- ❌ No se realiza despliegue
- ❌ N
