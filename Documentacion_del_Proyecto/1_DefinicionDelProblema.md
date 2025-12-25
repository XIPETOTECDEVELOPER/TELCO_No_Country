# 📊 Proyecto de Data Science – Predicción de Churn

## 1️⃣ Definición del problema

### Problema a resolver

Las empresas con modelos de suscripción o servicios recurrentes pierden ingresos cuando los clientes cancelan el servicio (*churn*).

El principal problema es que la cancelación normalmente se detecta **cuando ya ocurrió**, lo que deja poco margen de acción para retener al cliente.

---

### Enunciado del problema

Dado el **historial de comportamiento y uso de un cliente**, predecir si es probable que cancele el servicio en el corto plazo.

---

### Tipo de problema de Data Science

**Clasificación binaria**

* **1** → Va a cancelar
* **0** → Va a continuar

**Salida adicional:**

* Probabilidad de cancelación (valor entre **0 y 1**)

---

### Unidad de análisis

**Cliente individual**

Cada predicción corresponde a un solo cliente, no a grupos ni a periodos agregados.

---

### Restricciones del problema

* Dataset pequeño y controlado.
* Variables simples y explicables.
* Predicción pensada para tiempo real (enfoq
