# 🔍 Data Quality & Exploratory Analysis Prompt  
**Dataset:** Libros Dataset.xlsx  

## 🎯 Objetivo
Realizar un análisis exploratorio exhaustivo del dataset (Libros Dataset.xlsx) para:
- Detectar problemas de calidad de datos.
- Identificar inconsistencias estructurales.
- Anticipar riesgos que puedan sesgar análisis posteriores o modelos.

---

## 1. 📥 Carga y visión inicial
- Cargar el fichero Excel especificando hoja.
- Mostrar:
  - Dimensiones (`rows`, `columns`)
  - Primeras filas (`head`)
  - Tipos de datos (`info`)

---

## 2. 🧱 Validación estructural
- Validar:
  - Tipos de datos por columna
  - Número de valores nulos (`isnull().sum()`)
  - Porcentaje de nulos por columna
  - Registros duplicados (`duplicated()`)

✅ Output esperado:
- Lista clara de columnas con problemas
- Indicador de criticidad (alto/medio/bajo)

---

## 3. 📊 Análisis de calidad de datos

### 3.1 Variables numéricas
- Calcular:
  - Estadísticas descriptivas (`mean`, `std`, `min`, `max`, `quartiles`)
- Detectar outliers usando:
  - IQR:  
    - Lower bound = Q1 − 1.5 × IQR  
    - Upper bound = Q3 + 1.5 × IQR
  - Z-score (>3 desviaciones)

✅ Identificar:
- Columnas con valores extremos
- Impacto potencial en análisis (ej. sesgo en medias)

---

### 3.2 Variables categóricas
- Analizar:
  - Valores únicos (`nunique`)
  - Listado de categorías (`unique`)
- Detectar:
  - Inconsistencias de formato (mayúsculas, espacios, typos)
  - Categorías duplicadas semánticamente

✅ Ejemplo de riesgo:
- "Yes", "yes", "YES" → fragmentación de métricas

---

### 3.3 Validación de tipos internos
- Revisar coherencia dentro de cada columna:
  - Identificar mezcla de tipos (`str`, `int`, `float`)
  
✅ Ejemplo crítico:
- Campo texto con valores numéricos → error de tipado

---

### 3.4 Reglas de negocio / coherencia lógica
- Validar relaciones entre variables:
  - Rangos razonables (edad, precios, tiempos)
  - Coherencia entre métricas (ej. tiempo vs actividad)

✅ Detectar:
- Valores fuera de lógica operativa
- Posibles errores de captura

---

## 4. 🚨 Resumen de problemas de calidad

Generar un output estructurado con:

### 🔴 Críticos
- Tipos incorrectos
- Outliers extremos
- Datos corruptos

### 🟠 Medios
- Inconsistencias de categorías
- Valores fuera de rango esperado

### 🟡 Leves
- Formato no estandarizado
- Potenciales mejoras de limpieza

---

## 5. 📌 Recomendaciones accionables
Para cada problema identificado:
- Acción propuesta (ej. imputación, conversión, eliminación)
- Riesgo si no se corrige
- Prioridad

---

## 6. 📊 Output esperado
- Resumen ejecutivo (1–2 párrafos)
- Lista estructurada de issues
- Insights clave del dataset
- Preparación recomendada antes de análisis avanzado / ML

---

## ⚠️ Consideraciones clave
- No asumir calidad de datos → validar siempre
- Priorizar consistencia sobre volumen
- Documentar todas las transformaciones

