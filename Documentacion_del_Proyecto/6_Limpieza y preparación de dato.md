# 6. Limpieza y preparación de datos

## Objetivo del paso

Preparar el dataset para que pueda ser consumido por un modelo de *Machine Learning*, asegurando:

- Tipos de datos correctos  
- Valores consistentes  
- Variables listas para transformación posterior  

⚠️ En este paso **NO** se hace modelado, **NO** se seleccionan *features* finales y **NO** se codifican aún las variables categóricas.  
Solo se deja el dataset **limpio y coherente**.

---

## 6.1 Eliminación de variables no predictivas

### Variable: `customerID`

- Es un identificador único  
- No aporta información al comportamiento del cliente  
- Debe eliminarse  

**Regla:** ningún ID debe entrar al modelo.

---

## 6.2 Corrección de tipos de datos

### Variable: `TotalCharges`

**Estado actual:**
- Tipo: `object`  
- Representa un valor numérico (cargos totales)  
- Contiene valores que impiden conversión directa  

**Acción:**
- Convertir a tipo numérico  
- Forzar errores a `NaN`  

**Resultado esperado:**
- `TotalCharges` pasa a tipo numérico  
- Algunos valores se convierten en nulos (comportamiento esperado)

---

## 6.3 Tratamiento de valores nulos

Tras la conversión de `TotalCharges` aparecen valores nulos asociados a:

- Clientes con `tenure = 0`  
- Clientes muy nuevos  

### Decisión recomendada (simple y válida)

- Eliminar esos registros  
- Impacto mínimo en un dataset de ~7,000 filas  

**Alternativa válida (no obligatoria):**
- Imputar con 0  

➡️ Para este proyecto:  
✔ Se eliminan filas con `NaN` en `TotalCharges`

---

## 6.4 Normalización de valores categóricos

Se verifica que las variables categóricas:

- No tengan espacios inconsistentes  
- No tengan errores tipográficos  
- Usen valores consistentes (`Yes` / `No`, categorías claras)  

**Ejemplo:**
- `"No internet service"` se mantiene como categoría  
- No se transforma ni agrupa todavía  

⚠️ Solo se valida consistencia, no se codifica.

---

## 6.5 Conversión de la variable objetivo

### Variable: `Churn`

**Estado actual:**
- Valores: `"Yes"` / `"No"`

**Acción obligatoria:**
- Conversión a binaria:
  - `Yes` → `1`
  - `No` → `0`

Esto es necesario para cualquier modelo supervisado de clasificación.

---

## 6.6 Revisión final post-limpieza

Al finalizar este paso se valida que:

- No existan valores nulos  
- Los tipos de datos sean coherentes  
- El dataset esté listo para *Feature Engineering*  

**Validaciones típicas:**

- `df.info()`  
- `df.isnull().sum()`

---

## Resultado del paso 6

✔ Dataset sin IDs innecesarios  
✔ Tipos de datos corregidos  
✔ Variable objetivo binaria  
✔ Sin valores nulos  
✔ Dataset preparado para modelado  

🔒 **Paso 6: Limpieza y preparación de datos — CERRADO**
