# 📊 EDA Ecommerce – Enfoque Estratégico (Incremento de Ventas)

## 🎯 Objetivo
Realizar un análisis exploratorio de datos (EDA) del dataset de ecommerce con el objetivo de **identificar palancas para incrementar las ventas (Total Sales - revenue bruto)** desde una perspectiva estratégica de marketing y negocio.

Utilizar el fichero "Ecommerce.xlsx"

---

## 1. 📈 Análisis Descriptivo Orientado a Revenue
Analizar las principales variables numéricas:

- Total Sales (variable objetivo)
- Quantity Sold
- Unit Price
- Discount

Evaluar:
- Media, mediana, desviación estándar
- Rango y percentiles
- Sesgo (skewness)
- Concentración de revenue (**Pareto 80/20**)

---

## 2. 🚀 Identificación de Drivers de Ventas
Analizar qué factores impulsan el revenue:

### Comparativas por:
- Product
- Category
- Region
- Marketing Channel
- Customer Type

### Objetivos:
- Identificar el **top 20% de combinaciones que generan ~80% del revenue**
- Detectar segmentos de bajo rendimiento (oportunidades de crecimiento)
- Identificar combinaciones **escalables**

---

## 3. 💰 Análisis de Pricing y Descuentos
Evaluar el impacto de precios y descuentos en ventas:

### Relaciones clave:
- Discount vs Total Sales
- Unit Price vs Quantity Sold

### Identificar:
- Elasticidad al precio (aproximada)
- Umbrales óptimos de descuento
- Casos de **alto descuento sin impacto en revenue**
- Posibles **ineficiencias de pricing**

---

## 4. 📣 Performance de Canales de Marketing
Evaluar la eficiencia de cada canal:

### Métricas:
- Revenue total
- Ticket medio
- Volumen (Quantity Sold)
- Revenue por pedido

### Identificar:
- Canales más rentables
- Canales con alto volumen pero bajo valor
- Canales con potencial de escalado

---

## 5. 👥 Segmentación de Clientes
Analizar diferencias entre tipos de clientes:

### Comparativa:
- New vs Existing Customers

### Evaluar:
- Contribución a revenue
- Ticket medio
- Sensibilidad a descuentos

### Objetivo:
- Detectar oportunidades de:
  - Fidelización (upsell / cross-sell)
  - Captación eficiente

---

## 6. 📅 Análisis Temporal
Analizar la evolución de ventas:

### Visualizaciones:
- Series temporales (mensual / semanal)

### Detectar:
- Estacionalidad
- Tendencias
- Picos anómalos

### Cruces recomendados:
- Marketing Channel
- Discount

---

## 7. ⚠️ Detección de Oportunidades y Anomalías
Identificar patrones relevantes:

### Outliers positivos:
- Pedidos con alto revenue → identificar drivers replicables

### Outliers negativos:
- Alto descuento + bajo revenue
- Alto volumen + bajo valor
- Posibles ineficiencias comerciales

---

## 8. 🧠 Insights Estratégicos (Output Clave)

### Generar:
- Principales drivers de crecimiento
- Recomendaciones claras en:
  - Pricing
  - Descuentos
  - Canales
  - Segmentación

### Incluir:
- ✅ Quick wins (impacto inmediato)
- ⚠️ Riesgos comerciales
- 🚀 Oportunidades de alto impacto

---

## 9. 📊 Priorización de Iniciativas (CLAVE DIRECCIÓN)

Clasificar cada insight según:

- Impacto económico estimado (€)
- Facilidad de implementación

### Matriz sugerida:
- Alto impacto / baja complejidad → **prioridad máxima**
- Alto impacto / alta complejidad → **iniciativas estratégicas**
- Bajo impacto → **descartar o monitorizar**

---

## 10. 📄 Formato de Salida

El resultado debe incluir:

- Visualizaciones claras y ejecutivas
- Resumen de insights clave (máx. 5–7)
- Recomendaciones accionables
- Estimación de impacto (cuando sea posible)
