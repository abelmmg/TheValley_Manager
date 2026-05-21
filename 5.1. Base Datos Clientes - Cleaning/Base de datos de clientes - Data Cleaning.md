## Pipeline de Limpieza, Validación y Estandarización de Datos de Ventas

## Rol
Actúa como un Ingeniero de Datos Senior y Analista de Operaciones de Business Intelligence.

## Contexto
Disponemos de un dataset preliminar de ventas ("Base Datos de Ventas por Clientes.xlsx") que presenta anomalías típicas de extracción de sistemas transaccionales (ERPs/WMS): registros nulos, inconsistencias de strings, duplicados potenciales y discrepancias de formato.

## Objetivo
Ejecutar un proceso sistemático de Data Cleaning y transformación para dejar el dataset listo para producción y análisis ejecutivo.

## Instrucciones de Procesamiento (Paso a Paso):

1. Gestión de Registros Nulos e Identidad:
   - Identificar IDs de cliente ausentes. [Insertar aquí la regla de negocio elegida, ej: "Asignar ID genérico '9999' / Eliminar fila"].
   - Validar duplicados de transacciones basándose en la combinación de Customer ID + Purchase Date + Product Category. Si son transacciones legítimas, mantenerlas pero añadir una columna de ID de Transacción único.

2. Estandarización de Datos Categóricos (Texto):
   - Homogeneizar la columna 'Product Category' aplicando Title Case. Corregir errores de pluralización (ej. "Electronic" y "Electronics" deben consolidarse en "Electronics"; "books" en "Books").
   - Homogeneizar 'Payment Method'. Corregir variaciones de formato (ej. "pay-pal" a "PayPal"). Manejar los valores nulos categorizándolos como "Not Specified".

3. Normalización de Estados Operativos (Shipping Status):
   - Unificar el criterio de caja (Case Styling) a formato Capitalizado (ej. "shipped" y "Shipped" -> "Shipped").
   - Identificar y aislar los estados "RETURNED" para asegurar que la lógica de negocio posterior pueda excluir estas transacciones de las métricas de ingresos netos si fuera necesario.

4. Formateo y Tipos de Datos:
   - Asegurar que 'Purchase Date' se parsee estrictamente como formato YYYY-MM-DD.
   - Forzar 'Quantity' como Entero (Integer) y 'Price' como Flotante (Float).
   - Crear una columna calculada: [Total Revenue = Quantity * Price].

## Entregables Requeridos:
1. Una tabla con el dataset completamente limpio y estandarizado.
2. Un reporte ejecutivo breve de anomalías detectadas (Data Quality Audit Log) detallando cuántas filas se modificaron y por qué.