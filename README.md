# AnalisisdataTelecomXpt2

# Predicción de Evasión de Clientes - Telecom X

El objetivo central de este proyecto es el desarrollo de una infraestructura analítica capaz de identificar con precisión a los clientes en riesgo de abandonar la compañía Telecom X. Mediante el uso de técnicas avanzadas de ciencia de datos y aprendizaje automático, se busca transformar la estrategia de retención de la empresa de un modelo reactivo a uno proactivo. El análisis se centra en detectar patrones de comportamiento y características demográficas que preceden a la cancelación del servicio, permitiendo a la organización intervenir de manera estratégica antes de que la pérdida se concrete. La meta técnica es maximizar la métrica de sensibilidad para asegurar que la mayor proporción posible de evasores reales sea detectada por el sistema.

## 2. Estructura del proyecto y organización de los archivos

El proyecto está diseñado bajo una filosofía de desarrollo por capas, garantizando la modularidad y la escalabilidad del código. La organización se divide en cuatro bloques lógicos fundamentales. 
Primero, una capa de carga y limpieza donde se consolidan los siete mil doscientos sesenta y siete registros originales y se eliminan identificadores irrelevantes para evitar sesgos. 
Segundo, una capa de procesamiento técnico que incluye la codificación de variables categóricas, el balanceo de clases mediante la técnica sintética SMOTE y la estandarización de variables continuas para normalizar las magnitudes de gasto y permanencia. 
Tercero, una capa de modelado comparativo donde se entrenan y auditan arquitecturas de Regresión Logística y Random Forest. 
Finalmente, el repositorio se completa con el archivo de datos procesados en formato CSV y el cuaderno de Google Colab que integra todo el flujo de trabajo de forma secuencial.

## 3. Ejemplos de gráficos e insights obtenidos

Durante la fase de análisis dirigido y evaluación, se generaron visualizaciones críticas que revelaron la anatomía de la deserción en la empresa. Los diagramas de caja y los mapas de dispersión permitieron confirmar que la mayor densidad de fugas ocurre en los clientes con una permanencia inferior a doce meses, identificando un periodo de vulnerabilidad crítica al inicio de la relación contractual. Asimismo, el análisis de importancia de variables demostró que el tipo de contrato mensual y los cargos facturados son los motores principales de la evasión. 
Un hallazgo fundamental es que el modelo de Random Forest alcanzó un nivel de detección del ochenta y dos punto setenta y ocho por ciento, lo que valida la capacidad de la infraestructura para discernir entre clientes leales y aquellos con alta probabilidad de abandono basándose en sus hábitos de consumo y tiempo de servicio.

## 4. Instrucciones para ejecutar el notebook

Para reproducir este análisis en un entorno de Google Colab, es necesario acceder al entorno virtual y asegurar la disponibilidad del archivo de datos procesados mediante la interfaz de carga de archivos de la plataforma. Una vez que el archivo esté presente en el directorio local, se deben ejecutar las celdas de forma secuencial para importar las librerías necesarias, incluyendo herramientas de procesamiento de datos, aprendizaje automático y balanceo de clases. Es fundamental respetar el orden de ejecución para que las variables estandarizadas y los conjuntos de entrenamiento se generen correctamente antes de iniciar el proceso de modelado. El sistema procesará automáticamente las transformaciones y presentará los reportes de rendimiento y matrices de confusión al final del recorrido del código.
