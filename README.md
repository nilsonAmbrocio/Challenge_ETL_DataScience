# 📊 Análisis de Deserción de Clientes

Este proyecto tiene como objetivo identificar patrones de deserción (*churn*) en clientes de una empresa de servicios, utilizando análisis exploratorio de datos y visualización.

---

## 🧰 Librerías utilizadas

- **`pandas`**: para el manejo de la base de datos.
- **`seaborn`**: para la generación de gráficos categóricos y estadísticos.
- **`matplotlib`**: para el control visual de los gráficos.
- **`numpy`**: se utilizó únicamente para convertir la columna `Charges.Total` de tipo `object` a `float`.

---

## ⚙️ Tratamiento de la base de datos

- Se identificaron y reemplazaron valores vacíos representados como `''` y `' '` usando el método `.loc` de `pandas`.
- Se renombraron algunas columnas para facilitar su interpretación.
- Se realizó conversión de tipos de datos cuando fue necesario para análisis numérico.

---

## 📈 Visualización y análisis

Se realizaron diferentes visualizaciones para entender el comportamiento de los clientes en relación a la deserción:

- **`countplot`** (`seaborn`): para analizar la distribución de clientes desertores según variables categóricas (como género, método de pago, servicios contratados, etc.).
- **`boxplot`** (`seaborn`): para observar diferencias en variables numéricas como antigüedad (`tenure`), pago mensual (`Charges.Monthly`) y pago total (`Charges.Total`) entre los clientes que desertaron y los que no.

---

## 🧠 Conclusiones

- Los clientes que **desertaron** tienden a ser **jóvenes** e **independientes** (tanto hombres como mujeres).
- Contrataban **más servicios**, lo que se refleja en **mayores cantidades de Cuentas mensual y total**.
- Pagaban usando **cheques electrónicos** y recibían **facturas electrónicas**.
- Muchos **no recibían soporte técnico**, ni contaban con **seguridad en línea**, **copias de respaldo** ni **protección de dispositivos**, lo que posiblemente generó desconfianza o falta de fidelización.
- La mayoría tenía **contratos mensuales**, lo que facilita la decisión de abandonar el servicio.

---

## 📂 Archivos incluidos

- `TelecomX_Data.json`: dataset utilizado.
- `Challenge_ETL_Oracle.ipynb`: notebook con procesamiento, limpieza y visualización.
- `README.md`: este documento.

---

## 🚀 Requisitos

Este proyecto fue desarrollado con:

```bash
Python
pandas
numpy
seaborn
matplotlib
