# 📥 Carga de datos

## Objetivo de este paso

Leer el dataset desde el archivo CSV y verificar que:

* El archivo se carga correctamente.
* Las columnas existen y tienen los nombres correctos.
* Los tipos de datos son coherentes.
* El número de registros coincide con lo esperado (≈ 7,000).

> ⚠️ En este punto **NO se limpia ni se transforma ningún dato**; únicamente se valida la carga.

---

## Fuente de datos

* **Formato:** CSV
* **Origen:** Dataset histórico de clientes
* **Archivo esperado:** `churn_data.csv`

---

## Acción principal

Cargar el dataset en un **DataFrame de Pandas**.

```python
import pandas as pd

df = pd.read_csv("churn_data.csv")
```

---

## Verificaciones mínimas

### Vista inicial del dataset

```python
df.head()
```

Permite confirmar:

* Orden de columnas.
* Valores de ejemplo.
* Formato general del dataset.

---

### Dimensiones del dataset

```python
df.shape
```

Permite confirmar:

* Número de filas (≈ 7,000).
* Número de columnas.

---

### Nombres de columnas

```python
df.columns
```

Permite confirmar:

* Nombres correctos.
* Ausencia de espacios o errores tipográficos.

---

### Tipos de datos

```python
df.dtypes
```

Permite confirmar:

* Variables numéricas vs categóricas.
* Posibles errores de tipo.

---

## Resultado esperado

Al finalizar este paso:

* El dataset está correctamente cargado en memoria.
* La estructura coincide con lo definido en el **Punto 3: Definición del dataset**.
* No se ha modificado ningún dato.

---

✔ **Con esto queda cerrado el Punto 4: Carga de datos.**
