# Master Universitario avanzado en Inteligencia Artificial de la UAX

Actúa como un Director de Operaciones Académicas y Consultor EdTech senior. Tu objetivo es diseñar una tabla de cronograma quirúrgica y detallada para el lanzamiento y la ejecución del "Máster Universitario Online Avanzado en Inteligencia Artificial de la UAX", un programa de 12 meses de duración (Formato Executive) dirigido a profesionales STEM de nivel avanzado.

El diseño debe estructurarse bajo los siguientes parámetros operativos y restricciones estrictas:

# 1. ARQUITECTURA E INFRAESTRUCTURA DE COMPUTACIÓN (GOOGLE CLOUD)
- La infraestructura central se basará al 100% en Google Cloud Platform (GCP), utilizando Vertex AI, Google Kubernetes Engine (GKE) para la orquestación de MLOps, e instancias de Compute Engine con GPUs dedicadas.
- Restricción crítica: Todo el entorno de Sandbox y los límites/cuotas de coste por alumno en GCP deben estar auditados, validados y operativos 4 semanas antes del inicio de las clases.

# 2. LOGÍSTICA ACADÉMICA Y CARGA HORARIA RESTRINGIDA
- Duración total del programa: 12 meses improrrogables para profesionales en activo.
- Dedicación del alumno: 15-20 horas semanales distribuidas estrictamente en:
  * 4 horas síncronas los fines de semana (Viernes tarde o Sábado mañana) para Code Reviews, resolución de cuellos de botella arquitectónicos y sesiones con expertos.
  * 12-16 horas de trabajo asíncrono en laboratorios GCP y desarrollo del proyecto.

# 3. EMBARQUE TÉCNICO Y PROCESO FILTRADO DE ADMISIONES (MESES 1-2)
- Fase 0 y 1 (Meses 1-2): Cierre de plan de estudios, validación de la infraestructura Cloud de IA y campaña de Admisiones técnicas.
- El filtro técnico inicial obligatorio se realizará mediante una evaluación de código automatizada en HackerRank enfocada en algoritmos, optimización matemática y Python avanzado.
- Hito de Nivelación: Los alumnos admitidos con áreas de mejora identificadas deberán cursar obligatoriamente un Bootcamp previo de nivelación (repaso intensivo de cálculo multivariable, álgebra lineal numérica y fundamentos de scripting en entornos Linux) que concluirá antes de iniciar el Mes 2 del calendario.

# 4. ITINERARIOS DE ESPECIALIZACIÓN (Fase 4 - Desdoblada en Meses 10-11)
- En la fase de especialización avanzada (Meses 10-11), el cronograma debe dividirse obligatoriamente en dos tracks paralelos para que el alumno elija uno:
  * Track A: Advanced GenAI & LLMOps (Especializado en arquitecturas de atención, fine-tuning y despliegue de grandes modelos de lenguaje).
  * Track B: Edge AI & Computer Vision de Alto Rendimiento (Especializado en optimización de modelos para dispositivos embebidos, TensorRT y sistemas autónomos).

# 5. PROYECTO DE FIN DE MÁSTER (TFM) E HITO PRESENCIAL DE CIERRE (MES 12)
- Estrategia del TFM: El proyecto se desarrolla en paralelo a lo largo del año. Los pipelines de MLOps construidos en los bloques core iniciales servirán como la infraestructura base sobre la que se desplegará el modelo avanzado del TFM.
- Requisito de Cierre (Mes 12): La defensa del TFM ante el tribunal académico de la UAX se realizará de manera presencial obligatoria en el campus de Madrid al finalizar el programa.

# FORMATO DE SALIDA REQUERIDO:
- Organiza la información en una tabla Markdown con las siguientes columnas estrictas: [Mes / Fase del Proyecto], [Hito u Objetivo Operativo], [Entregable Técnico Académico], [Restricciones, Dependencias Críticas y Stack GCP].
- Asegura que el orden sea estrictamente cronológico a lo largo de los 12 meses, mostrando de manera clara el desdoblamiento de los dos tracks en la fase de especialización y el solapamiento del pipeline del TFM. Evita explicaciones introductorias genéricas; ve directo a la tabla de planificación de operaciones.