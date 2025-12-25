# 📁 Definición del dataset

## Objetivo del dataset

El dataset debe representar el **comportamiento histórico de los clientes** antes de que ocurra (o no) la cancelación, de modo que el modelo pueda aprender patrones asociados al *churn*.

Cada fila del dataset representa **un cliente en un momento determinado**.

---

## Tamaño del dataset

* **7,000 registros**.
* Considerado un dataset **pequeño y controlado**.

Adecuado para:

* Entrenamiento rápido.
* Validación clara de resultados.
* Uso en contextos de hackathon o proyectos académicos.

---

## Variable objetivo (*target*)

| Columna | Tipo    | Significado                        |
| ------- | ------- | ---------------------------------- |
| churn   | Binaria | 1 = cliente canceló / 0 = continuó |

> ⚠️ Esta variable **NO se usa como entrada** del modelo; solo funciona como **etiqueta** durante el entrenamiento.

---

## Variables predictoras (*features*)

Las variables deben cumplir con los siguientes criterios:

* Ser conocidas **antes** de la cancelación.
* Tener sentido desde la perspectiva del negocio.
* Ser utilizables posteriormente vía API.

### Variables mínimas recomendadas

| Variable              | Tipo       | Descripción               |
| --------------------- | ---------- | ------------------------- |
| tiempo_contrato_meses | Numérica   | Antigüedad del cliente    |
| retrasos_pago         | Numérica   | Número de pagos tardíos   |
| uso_mensual           | Numérica   | Uso promedio del servicio |
| plan                  | Categórica | Tipo de plan contratado   |

---

## Estructura esperada del CSV

```csv
tiempo_contrato_meses,retrasos_pago,uso_mensual,plan,churn
12,2,14.5,Premium,1
24,0,32.1,Basico,0
6,3,5.2,Estandar,1
```

---

## Restricciones del dataset

* No incluir datos personales sensibles.
* No incluir columnas que revelen directamente la cancelación futura.
* No permitir valores imposibles (negativos, textos erróneos, formatos inconsistentes).
* Columnas alineadas al contrato de entrada en formato JSON.

---

## Relación con el Back-end

Las columnas del dataset definen **directamente** los campos que el Back-end enviará a la API.

> Si una columna existe en el dataset, **debe existir en el JSON de entrada**.

---

✔ **Con esto queda cerrado el Punto 3: Definición del dataset.**
El dataset queda conceptualmente definido, aunque todavía **no ha sido cargado ni analizado**.
