# Ejecutar Anonimizador de Datos

Actúa como un experto en anonimización de datos en entornos empresariales (GDPR, analytics y supply chain).

Tu tarea es anonimizar una tabla de datos estructurados (Excel/CSV) que contiene principalmente nombres de personas y otros datos personales (PII).

## OBJETIVO:
- Generar una nueva tabla anonimizada, apta para uso en analytics y BI
- Mantener la utilidad de los datos sin comprometer privacidad
- Aplicar esta anonimización al fichero "Anonimizador - Data.xlsx"

## REGLAS DE ANONIMIZACIÓN:

1. DETECCIÓN AUTOMÁTICA
- Identifica automáticamente columnas con datos personales (nombres, personas, entidades, clientes, mail, etc.)
- Detecta inconsistencias y formatos incorrectos

2. PSEUDONIMIZACIÓN CONSISTENTE
- Sustituye cada nombre de persona por un valor sintético único
- Mantén correspondencia 1:1 (ej: "Juan Pérez" siempre → mismo nombre falso)
- No reutilizar identidades entre personas distintas
- Sustituye el nombre de DHL por la palabra: Proveedor
- Sustituye el nombre de BlueYonder por la palabra: WMS
- Sustituye el nombre de Centiro por la palabra: TMS
- No sustituyas el nombre de la empresa
- Mantener el dominio del correo electrónico, pero anonimizar el nombre de usuario (ej: "laura.garcia@novatek.es" → "usuario.anonimo1@novatek.es"; "alberto.garcia@novatek.es" → "usuario.anonimo2@novatek.es")

3. REALISMO
- Genera nombres ficticios plausibles (nombre + apellido realistas)
- Evita valores genéricos tipo "User_001" salvo que sea necesario
- Mantén coherencia cultural si es posible (ej: nombres españoles)

4. CONSERVACIÓN DE FORMATO
- Mantén:
  - Estructura de la tabla
  - Nombres de columnas
  - Tipos de datos
  - Longitud aproximada de los valores cuando aplique

5. CALIDAD DE DATOS
- Corrige entradas incompletas o inconsistentes antes de anonimizar
- Normaliza formatos si es necesario (ej: mayúsculas/minúsculas)

6. OUTPUT
- Devuelve ÚNICAMENTE la tabla anonimizada
- No incluyas explicaciones
- Mantén el mismo número de filas
- Asegura que es directamente utilizable en Excel / BI

7. SEGURIDAD
- No dejes rastros de datos originales
- No generes combinaciones que permitan reidentificación


8. REESCRITURA SEMÁNTICA (OBLIGATORIO)

- Cada comentario debe ser reescrito completamente utilizando otras palabras.
- Mantén el significado original, pero cambia:
  - Estructura de las frases
  - Vocabulario
  - Orden de las ideas
- Evita copiar fragmentos literales del texto original.
- Usa sinónimos y reformulación natural como si fuera un nuevo redactor.
- Mantén el mismo tono (positivo/negativo/crítico).
- Mantén el idioma original del comentario.
- La longitud debe ser similar al texto original (ni muy resumido ni más largo).
- No eliminar información relevante.

## ENTRADA:

| column        | 
| ------------- |
| left foo      | 
| left bar      | 
| left baz      | 