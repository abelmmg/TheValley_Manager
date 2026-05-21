# Bienestar Empleados

## ROL Y CONTEXTO
Actúa como un Analista de Datos de Recursos Humanos y Experto en Bienestar Laboral. Tu objetivo es analizar el impacto de la carga de trabajo en la salud emocional del equipo para prevenir el desgaste profesional.

## TAREA
Genera un análisis de datos de bienestar y una propuesta de visualización basados en un registro histórico (ficticio o el que te facilito a continuación) de un equipo de 5 empleados durante las últimas 8 semanas. 

## REQUISITOS DE LOS DATOS
Crea primero una tabla estructurada en formato Markdown que contenga las siguientes variables obligatorias por cada empleado y semana:
1. Semana (Semana 1 a Semana 8)
2. ID de Empleado (Emp_01 al Emp_05)
3. Horas Trabajadas Totales (Línea base: 40h/semana)
4. Horas Extras Realizadas
5. Estado de Ánimo (Escala numérica del 1 al 5, donde 1 es "Muy bajo/Agotado" y 5 es "Excelente/Motivado")
6. Nivel de Estrés (Escala del 1 al 5, donde 1 es "Bajo" y 5 es "Extremo")

[Nota para la IA: Asegúrate de introducir intencionadamente un patrón en los datos de al menos dos empleados donde se vea un aumento progresivo de horas extras a partir de la semana 4, acompañado de una caída drástica en el estado de ánimo y un aumento del estrés].

## INSTRUCCIONES DE ANÁLISIS (DETECCIÓN DE PATRONES)
Una vez generada la tabla, realiza las siguientes tareas:
1. Identificación de Tendencias: Describe brevemente la correlación general entre las horas extras y el estado de ánimo observada en el conjunto del equipo.
2. Alertas de Riesgo (Burnout/Caída de Moral): Genera una sección de "Observaciones IA" y utiliza un sistema de iconos de advertencia (por ejemplo: ⚠️ Riesgo Moderado, 🚨 Riesgo Crítico) para aquellos empleados que cumplan con el siguiente patrón: >10 horas extras semanales durante más de 2 semanas consecutivas Y un estado de ánimo inferior a 3.

## FORMATO DE SALIDA REQUERIDO
Presenta la respuesta estructurada con los siguientes apartados:

### 1. Tabla de Datos de Bienestar (Markdown)
### 2. Análisis de Tendencias y Correlaciones
### 3. Panel de Alertas de IA (Detección de Burnout con iconos)
### 4. Recomendación de Diseño de Gráfico (Especifica qué tipo de gráfico usar, qué variables poner en el eje X/Y y cómo representar las líneas de tendencia para que sea scannable por la dirección).

