# Heart Disease Risk Prediction

Este proyecto tiene como objetivo analizar y comprender el riesgo de enfermedad cardíaca a partir de datos clínicos reales, utilizando un enfoque paso a paso y completamente explicativo. El énfasis principal no está en usar librerías automáticas, sino en **entender el proceso**, los datos y las decisiones que se toman durante el análisis.

El trabajo se desarrolla como parte de un laboratorio académico enfocado en **regresión logística**, análisis exploratorio de datos y evaluación del desempeño de modelos predictivos.

## Objetivo del proyecto

El objetivo principal es:

- Analizar un conjunto de datos reales de pacientes
- Identificar patrones asociados a la presencia de enfermedad cardíaca
- Construir un modelo de regresión logística desde cero
- Interpretar los resultados obtenidos de forma clara y razonada

## Dataset utilizado
Se utiliza el **Heart Disease Dataset**, un conjunto de datos ampliamente conocido que contiene información clínica de pacientes, como:
- Edad
- Presión arterial
- Colesterol
- Frecuencia cardíaca máxima
- Variables relacionadas con ejercicio y electrocardiogramas
- Variable objetivo que indica presencia o ausencia de enfermedad cardíaca

El dataset se encuentra almacenado en la carpeta:

## Desarrollo del análisis

Todo el desarrollo del proyecto se encuentra documentado y ejecutado en un cuaderno de Jupyter.

### NOTA IMPORTANTE

**El cuaderno de Jupyter donde se encuentra todo el desarrollo es el que se llama _Feature Selection_.**  
En este cuaderno se abordan de manera ordenada los siguientes puntos clave:

- Análisis Exploratorio de Datos (EDA)
- Completitud de datos y verificación de valores faltantes
- Preparación y transformación de variables
- Convergencia del algoritmo de regresión logística
- Evaluación del desempeño del modelo
- Interpretación de resultados
- Interpretación de coeficientes del modelo

## Contenido del análisis

### 1. Análisis Exploratorio de Datos 

En esta etapa se realiza una exploración inicial del dataset para:

- Comprender la estructura de los datos
- Identificar el tipo de variables disponibles
- Analizar la distribución de la variable objetivo
- Verificar si el dataset se encuentra balanceado

Se incluye una visualización clara de la distribución de pacientes con y sin enfermedad cardíaca.

<img width="711" height="708" alt="image" src="https://github.com/user-attachments/assets/3f083253-8e5c-48bd-8aa3-b4b609ed9c5b" />

- Gráfica de barras con la distribución de clases (0: ausencia, 1: presencia)

Ubicación recomendada:

---

### 2. Completitud de los datos

Se verifica si existen valores faltantes en el dataset y se confirma que los datos son adecuados para el entrenamiento del modelo sin necesidad de imputaciones complejas.

Este paso es fundamental para asegurar la calidad del análisis posterior.

---

### 3. Preparación de los datos

En esta fase se realiza:

- Conversión de la variable objetivo a formato binario
- Selección de variables relevantes
- Separación del conjunto de datos en entrenamiento y prueba (70% / 30%)
- Normalización de variables numéricas

Esto permite entrenar el modelo de manera estable y coherente.

---

### 4. Entrenamiento del modelo

Se implementa un modelo de **regresión logística desde cero**, siguiendo los conceptos vistos en clase:

- Función sigmoide
- Función de costo
- Algoritmo de gradiente descendente

Durante el entrenamiento se analiza la **convergencia del algoritmo**, observando cómo el costo disminuye a lo largo de las iteraciones.

<img width="873" height="689" alt="image" src="https://github.com/user-attachments/assets/f2848b6f-74bf-41cb-8e13-e13bc062ed9f" />

- Gráfica del costo en función de las iteraciones

Ubicación recomendada:


### 5. Evaluación del desempeño

Una vez entrenado el modelo, se evalúa su desempeño utilizando métricas como:

- Exactitud (accuracy)
- Precisión
- Recall
- F1-score

Estas métricas se analizan tanto en el conjunto de entrenamiento como en el de prueba para verificar la capacidad de generalización del modelo.

---

### 6. Interpretación de resultados

Se realiza un análisis interpretativo de los resultados obtenidos, explicando:

- Qué tan bien el modelo logra separar pacientes con y sin enfermedad
- Qué limitaciones presenta el enfoque lineal
- Qué tan confiables son las predicciones realizadas

---

### 7. Interpretación de coeficientes

Finalmente, se analizan los coeficientes del modelo para entender:

- Qué variables tienen mayor influencia en la predicción
- Cómo cambian las probabilidades de enfermedad ante variaciones en los factores clínicos
- La relación entre los datos médicos y la salida del modelo

Este punto permite conectar el modelo matemático con el contexto real de la salud.

### Visualización de Fronteras de Decisión
<img width="1173" height="335" alt="image" src="https://github.com/user-attachments/assets/982b8348-1fe0-49fa-9f87-695bc9434014" />
Para analizar la capacidad del modelo de regresión logística para separar las clases, se entrenaron modelos utilizando pares de variables y se visualizaron sus fronteras de decisión.
En la figura se muestran tres combinaciones de características:
Edad vs Colesterol
Presión arterial vs Frecuencia cardíaca máxima
Depresión del ST vs Número de vasos observados
Los puntos representan los datos de entrenamiento y prueba, mientras que la línea indica la frontera de decisión aprendida por el modelo.


## Evidencia visual del desarrollo

Durante el desarrollo del laboratorio se generaron distintas visualizaciones y ejecuciones del cuaderno.

- Ejecución correcta del notebook
- Resultados de entrenamiento
- Gráficas principales del análisis

## Estado del despliegue en la nube

El proyecto contempla una etapa de despliegue en AWS SageMaker.  
Sin embargo, **esta fase no se ha realizado aún** debido a restricciones de permisos en el entorno actual.

El trabajo queda preparado para continuar con el despliegue cuando se cuente con acceso completo a los servicios necesarios.

## Conclusión

Este proyecto permite comprender de manera práctica y progresiva cómo aplicar regresión logística a un problema real de salud, enfatizando la interpretación de los datos, el comportamiento del algoritmo y la explicación de los resultados, más allá de simplemente obtener una predicción.


## Autor

Samuel Antonio Gil Romero
