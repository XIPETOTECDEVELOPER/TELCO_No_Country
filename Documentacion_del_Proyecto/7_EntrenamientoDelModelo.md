# 🧠 Paso 7 — Entrenamiento de Modelos (Baseline + Selección)

## Objetivo del paso

Entrenar modelos de **clasificación supervisada**, evaluar su desempeño y **elegir un modelo** para el MVP de *churn*.

⚠️ En este paso:
- NO hay API  
- NO hay serialización  
- NO hay despliegue  

Solo **modelado y evaluación**.

---

## 7.1 Definir el modelo baseline (referencia mínima)

### ¿Qué es un baseline?

Un modelo **simple, rápido y explicable** que sirve como:

- Punto de comparación  
- Referencia mínima aceptable  

👉 Se utiliza **Logistic Regression**, estándar en problemas de *churn*.

### Código 7.1 — Modelo baseline

```python
from sklearn.linear_model import LogisticRegression

baseline_model = LogisticRegression(
    max_iter=1000,
    random_state=42
)

baseline_model.fit(X_train, y_train)
