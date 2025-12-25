# 🔍 Exploración de datos (EDA)

## Objetivo del EDA

Entender cómo son los datos, cómo se distribuyen y qué patrones básicos existen, **sin limpiar ni transformar aún**.

En este paso se busca **contexto**, no conclusiones definitivas.

---

## 5.1 Vista general del dataset

Con el dataset ya cargado, se confirma:

* **Filas:** 7,043 clientes
* **Columnas:** 21 variables
* **Unidad de análisis:** Cliente individual

Esto confirma que el dataset es:

* Suficiente para el proyecto
* Manejable para análisis y modelado

---

## 5.2 Variable objetivo: Churn

* **Tipo:** Categórica (Yes / No)

### Observaciones iniciales

* El churn no es un evento raro ni extremo.
* Existen clientes que cancelan y clientes que continúan.
* El dataset es apto para un problema de **clasificación binaria**.

En esta etapa solo interesa:

* Confirmar que existe churn.
* Ver que hay suficientes ejemplos de ambas clases.

> ⚠️ No se balancea ni se corrige la variable objetivo en este punto.

---

## 5.3 Variables numéricas principales

### Variables detectadas

* **tenure** → Antigüedad del cliente (meses)
* **MonthlyCharges** → Costo mensual
* **SeniorCitizen** → Indicador binario (0 / 1)

### Observaciones generales

* *tenure* presenta un rango amplio (clientes nuevos y antiguos).
* *MonthlyCharges* es una variable continua.
* *SeniorCitizen* es binaria, aunque esté codificada como numérica.

Estas variables:

* Tienen sentido de negocio
* Son candidatas claras para el modelo

---

## 5.4 Variables categóricas

### Ejemplos relevantes

* Contract
* PaymentMethod
* InternetService
* TechSupport
* StreamingTV
* PaperlessBilling

### Observaciones

* Muchas variables son del tipo **Yes / No**.
* Otras presentan múltiples categorías.
* Todas son explicables desde la perspectiva del negocio.

Esto confirma que el dataset:

* Es realista
* Es interpretable
* Es adecuado para modelos clásicos (ej. *Logistic Regression*)

---

## 5.5 Calidad visual inicial (sin limpieza)

Durante el EDA se detecta:

* **TotalCharges** está almacenada como texto → posible conversión futura.
* **customerID** funciona solo como identificador → no aporta al modelo.
* No se observan columnas obviamente corruptas.

> ⚠️ En este punto **no se corrige nada**; solo se documentan hallazgos.

---

## 5.6 Primeras preguntas que surgen (EDA)

Estas preguntas **no se responden aún**, pero guían los siguientes pasos:

* ¿Los clientes con menor *tenure* cancelan más?
* ¿El tipo de contrato influye en el churn?
* ¿El método de pago está relacionado con cancelaciones?
* ¿Los servicios adicionales reducen el churn?

Estas preguntas justifican el análisis profundo y el modelado posterior.

---

## Resultado del Paso 5

✔ Se entiende la estructura general del dataset
✔ Se identifica claramente la variable objetivo
✔ Se reconocen variables numéricas y categóricas
✔ Se detectan posibles ajustes futuros
✔ No se ha modificado ningún dato

---

🔒 **Paso 5 cerrado: Exploración de datos (EDA)**
