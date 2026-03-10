# Telecom X – Predicción de Cancelación de Clientes (Churn)

## Descripción del Proyecto

Este proyecto forma parte del desafío **Telecom X – Parte 2**, enfocado en el desarrollo de modelos de **Machine Learning** para predecir la cancelación de clientes (Churn).

Después de realizar el proceso de limpieza, transformación y análisis exploratorio de datos en la primera etapa del proyecto, en esta segunda fase se construye un **pipeline de modelado predictivo** que permite identificar clientes con mayor probabilidad de cancelar sus servicios.

El objetivo principal es demostrar cómo las técnicas de **ciencia de datos y aprendizaje automático** pueden ayudar a las empresas a anticipar el abandono de clientes y diseñar estrategias efectivas de retención.

Este análisis permite transformar datos históricos en información útil para la toma de decisiones estratégicas dentro de una organización.

---

# Objetivos del Proyecto

Los principales objetivos de este proyecto son:

- Preparar los datos para el modelado predictivo.
- Analizar la relación entre distintas variables y la cancelación de clientes.
- Construir modelos de clasificación para predecir el churn.
- Evaluar el rendimiento de los modelos utilizando métricas de Machine Learning.
- Identificar los factores que influyen en la cancelación de clientes.
- Generar insights que puedan apoyar estrategias de retención.

---

# Dataset

El dataset utilizado en este proyecto corresponde a información de clientes de **Telecom X** e incluye variables relacionadas con:

- Información demográfica de los clientes
- Servicios contratados
- Tipo de contrato
- Métodos de pago
- Tiempo de permanencia en la empresa
- Gastos mensuales y totales

El archivo utilizado en esta segunda etapa es:

datos_tratados.csv

Este dataset fue previamente limpiado y procesado en la **Parte 1 del proyecto**, eliminando inconsistencias y normalizando la información para facilitar el análisis y el modelado.

---


Descripción de los componentes:

**data/**  
Contiene el dataset procesado utilizado para el entrenamiento de los modelos.

**notebooks/**  
Incluye el notebook principal donde se desarrolla todo el proceso de análisis, visualización y modelado predictivo.

**images/**  
Carpeta destinada a almacenar visualizaciones generadas durante el análisis que pueden utilizarse en documentación.

**README.md**  
Documento que describe el proyecto, su estructura y los principales resultados obtenidos.

---

# Flujo del Análisis

El proyecto sigue un flujo típico de trabajo en ciencia de datos:

### 1. Carga de datos
Se importa el dataset previamente procesado para comenzar el análisis.

### 2. Exploración inicial
Se revisa la estructura del dataset, tipos de datos y estadísticas descriptivas.

### 3. Limpieza de datos
Se eliminan columnas irrelevantes como identificadores únicos que no aportan valor al modelo.

### 4. Análisis del balance de clases
Se analiza la proporción de clientes que cancelaron el servicio frente a aquellos que permanecen activos.

### 5. Transformación de variables categóricas
Se aplica **One-Hot Encoding** para convertir variables categóricas en variables numéricas compatibles con los algoritmos de Machine Learning.

### 6. Análisis exploratorio y visualización
Se generan visualizaciones para identificar patrones y relaciones entre variables relevantes.

### 7. Análisis de correlación
Se utiliza una matriz de correlación para identificar variables con mayor relación con la cancelación.

### 8. Preparación para modelado
Se separan las variables predictoras y la variable objetivo.

### 9. División del dataset
Se divide el conjunto de datos en entrenamiento y prueba para evaluar el rendimiento del modelo.

### 10. Normalización de variables
Se aplica estandarización a los datos para modelos sensibles a la escala.

---

# Modelos de Machine Learning

Para la predicción de cancelación se implementaron dos modelos de clasificación:

## Regresión Logística

La regresión logística es un modelo estadístico utilizado para problemas de clasificación binaria.

Este modelo permite interpretar cómo cada variable influye en la probabilidad de cancelación de un cliente.

## Random Forest

Random Forest es un modelo basado en múltiples árboles de decisión que permite capturar relaciones más complejas entre variables.

Este modelo también permite analizar la **importancia de las variables**, identificando cuáles tienen mayor impacto en la predicción.

---

# Evaluación de Modelos

Los modelos se evaluaron utilizando métricas estándar de clasificación:

- Accuracy (Exactitud)
- Precision
- Recall
- F1-score
- Matriz de confusión

Estas métricas permiten medir la capacidad del modelo para identificar correctamente a los clientes que cancelarán el servicio.

---

# Resultados y Hallazgos

El análisis permitió identificar factores importantes asociados con la cancelación de clientes.

Entre los hallazgos más relevantes destacan:

- Los clientes con contratos mensuales presentan mayor probabilidad de cancelar el servicio.
- Los clientes con menor tiempo de permanencia en la empresa muestran mayor riesgo de cancelación.
- El gasto mensual y los servicios adicionales contratados pueden influir en el comportamiento de cancelación.

Estos resultados permiten identificar segmentos de clientes con mayor riesgo y desarrollar estrategias orientadas a mejorar la retención.

---

# Conclusiones

El desarrollo de modelos predictivos permitió identificar patrones relevantes en el comportamiento de cancelación de clientes de Telecom X.

El uso de técnicas de Machine Learning demuestra cómo los datos pueden convertirse en una herramienta estratégica para anticipar problemas de negocio, en este caso la pérdida de clientes.

A partir de este análisis, la empresa podría implementar estrategias como:

- Programas de fidelización para clientes con contratos mensuales.
- Incentivos para clientes con menor tiempo de permanencia.
- Ofertas personalizadas dirigidas a clientes con alto riesgo de cancelación.

La aplicación de modelos predictivos permite a las organizaciones **anticiparse al churn**, mejorar la experiencia del cliente y reducir la pérdida de ingresos.

---

# Tecnologías Utilizadas

Las principales herramientas utilizadas en este proyecto fueron:

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

---

Proyecto desarrollado como parte de un desafío práctico de **Ciencia de Datos y Machine Learning**, enfocado en la aplicación de técnicas analíticas para resolver problemas empresariales reales.
