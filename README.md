# 📊 Segmentación de Clientes con Análisis RFM

## 📌 Resumen Ejecutivo
Este proyecto aplica la metodología **RFM (Recencia, Frecuencia y Valor Monetario)** para segmentar clientes según su comportamiento de compra.

A partir de un dataset de transacciones comerciales, se identificaron cinco segmentos clave que permiten optimizar estrategias de marketing, mejorar la retención y maximizar el valor del cliente (LTV).

---

## 🎯 Objetivos
- Analizar el comportamiento de compra de los clientes  
- Identificar segmentos estratégicos  
- Detectar clientes en riesgo  
- Optimizar decisiones comerciales basadas en datos  

---

## 🧾 Dataset

- Registros originales: **541,909**
- Registros después de limpieza: **397,884**
- Variables clave:
  - `CustomerID`
  - `InvoiceDate`
  - `Quantity`
  - `UnitPrice`
  - `Country`

---

## ⚙️ Preparación de Datos

- Eliminación de valores nulos críticos  
- Filtrado de transacciones inválidas  
- Conversión de tipos de datos  
- Creación de variable:

`TotalPrice = Quantity * UnitPrice`

---

## 🧠 Análisis RFM

### 🔹 Métricas
- **Recencia:** días desde la última compra  
- **Frecuencia:** número de compras  
- **Monetario:** gasto total  

📌 Fecha de referencia: **2011-12-10**

---

## 📊 Segmentación de Clientes

| Segmento             | Clientes |
|----------------------|----------|
| 🔴 Clientes Perdidos | 2438     |
| 🟢 Campeones         | 573      |
| 🟠 En Riesgo         | 519      |
| 🔵 Clientes Leales   | 445      |
| 🟡 Leales Potenciales| 363      |

---

## 📈 Resultados Visuales

<p align="center">
  <img src="imagenes/rfm_distribution.png" width="600">
</p>

<p align="center">
  <img src="imagenes/rfm_pie.png" width="600">
</p>

<p align="center">
  <img src="imagenes/rfm_means.png" width="600">
</p>

<p align="center">
  <img src="imagenes/heatmap.png" width="600">
</p>

<p align="center">
  <img src="imagenes/monetary_hist.png" width="600">
</p>

<p align="center">
  <img src="imagenes/monetary_box.png" width="600">
</p>

<p align="center">
  <img src="imagenes/champions_scatter.png" width="600">
</p>

<p align="center">
  <img src="imagenes/champions_freq_monetary.png" width="600">
</p>

<p align="center">
  <img src="imagenes/comparacion_gasto_prom.png" width="600">
</p>

---

## 🔍 Insights Clave

- Los **Clientes Perdidos** representan el mayor volumen  
- Los **Campeones** generan el mayor ingreso promedio (~8658)  
- Existe una fuerte relación entre frecuencia y gasto  
- Segmento “En Riesgo” es clave para estrategias de reactivación  

---

## 🤖 Modelo Predictivo

- MAE: 2033.84  
- R²: 0.07  

📌 Bajo poder predictivo → mejorar modelo

---

## 💡 Recomendaciones

- Campeones → Programas VIP  
- Leales → Fidelización  
- En riesgo → Reactivación  
- Perdidos → Recuperación  

---

## 📁 Estructura del Proyecto

```
.
├── G5-AnalisisDatos-EDA.ipynb
├── Analytical Customer Segmentation Analysis.csv
├── rfm_segmentation_report.csv
├── imagenes/
└── README.md
```

---

## ▶️ Ejecución

```
pip install pandas numpy matplotlib seaborn scikit-learn
jupyter notebook
```

---

## 🧩 Conclusión

El análisis RFM permite transformar datos en decisiones estratégicas para mejorar la rentabilidad del negocio.

## 👥 Autores

**Grupo 5 - Tratamiento de Datos**

| Nombre |
|--------|
| Sixto Encalada |
| Jimmy Anzules |
| Yordhan Guerron |