<h1 align="center">✈️ Análisis de Clientes y Vuelos — Programa de Fidelidad</h1> <p align="center"> <img width="104" height="156" alt="Professional_code_RUTH" src="https://github.com/user-attachments/assets/ee5f7c67-1167-4098-aae1-2e215979c0cb" /> </p>
<p align="center"><strong>Evaluación final del Módulo 3 — Data Analytics</strong>

<p align="center"> Realizada por RUTH PÉREZ SEGOVIA (Bootcamp Adalab).</p>
<p align="center">Proyecto centrado en análisis exploratorio, estadística descriptiva y visualización de datos.</p>

## Badges
[![Status](https://img.shields.io/badge/status-entregado-yellow)](./)
[![Made with Python](https://img.shields.io/badge/made%20with-Python-3776AB?logo=python&logoColor=white)](https://www.python.org/)
[![Pandas](https://img.shields.io/badge/library-pandas-150458?logo=pandas&logoColor=white)](https://pandas.pydata.org/)
[![Matplotlib](https://img.shields.io/badge/viz-matplotlib-11557c?logo=plotly&logoColor=white)](https://matplotlib.org/)
[![Seaborn](https://img.shields.io/badge/viz-seaborn-4c72b0)](https://seaborn.pydata.org/)
[![Last updated](https://img.shields.io/badge/última%20actualización-2026--01--23-brightgreen)](./)


## Descripción
Este repositorio contiene la resolución de la evaluación final del Módulo 3 (EDA + Estadística + Visualización) del Bootcamp de Data Analytics de Adalab.

El proyecto trabaja con dos datasets de un programa de lealtad de una aerolínea:

-Customer-Flight-Activity.csv: actividad de vuelos de los clientes (vuelos reservados, distancia, puntos acumulados y redimidos, etc.).

-Customer-Loyalty-History.csv: información demográfica y de fidelización (ubicación, educación, salario, estado civil, tipo de tarjeta, CLV, fechas de alta y cancelación).

El objetivo principal es practicar un flujo completo de análisis de datos: exploración, limpieza, análisis estadístico, visualización e interpretación en lenguaje de negocio.

## Objetivos del proyecto
Unir y limpiar dos fuentes de datos de clientes de aerolínea.
Realizar análisis exploratorio de variables numéricas y categóricas.
Detectar valores nulos y posibles outliers, asegurando la calidad del dataset.
Construir visualizaciones con Matplotlib y Seaborn para responder preguntas de negocio concretas.
Evaluar si existen diferencias relevantes en las reservas de vuelos según el nivel educativo de los clientes.
Documentar el flujo de trabajo y las decisiones tomadas como lo haría una analista de datos en un contexto profesional.

## Estructura del análisis
1️⃣ Fase 1 — Exploración y limpieza

Carga de los dos ficheros CSV y revisión de tipos, nulos y distribuciones básicas.
Unión de los datasets a través de Loyalty Number para construir una vista consolidada del cliente.
Normalización de tipos (fechas, numéricos, categóricos) y tratamiento de nulos en columnas clave (por ejemplo, educación, salario, vuelos y puntos).
Comprobación de consistencia entre variables (años y meses de alta/cancelación, rangos de distancia, etc.).

2️⃣ Fase 2 — Estadística descriptiva

Cálculo de estadísticas descriptivas (media, mediana, desviación estándar, percentiles) para variables como Flights Booked, Distance, Points Accumulated, Salary.
Identificación de posibles valores atípicos en métricas de vuelos y puntos.
Exploración de correlaciones entre variables numéricas (por ejemplo, distancia vs. puntos acumulados, CLV vs. salario).

3️⃣ Fase 3 — Visualización de datos

Se construyen visualizaciones específicas para responder a las preguntas del enunciado:

*Vuelos por mes:
Bar chart de Flights Booked agregados por Month para analizar la estacionalidad en las reservas.

*Distancia vs. puntos acumulados:
Diagrama de dispersión entre Distance y Points Accumulated, donde se observa una relación lineal positiva muy marcada (más distancia, más puntos).

*Distribución geográfica:
Gráfico de barras de clientes por Province, mostrando fuerte concentración en Ontario, British Columbia y Quebec.

*Salario por nivel educativo:
Bar chart del salario promedio por Education, donde se aprecia un incremento claro al subir el nivel educativo (Doctor > Master > Bachelor > High School).

*Proporción por tipo de tarjeta de fidelidad:
Pie chart para Loyalty Card, destacando la tarjeta Star como la más frecuente (en torno a la mitad de los clientes).

*Estado civil y género:
Gráfico de barras agrupadas (Marital Status en el eje X y Gender como hue) para estudiar el equilibrio entre hombres y mujeres en cada estado civil.

Cada visualización incluye una breve interpretación orientada a negocio, más allá del simple número.

4️⃣ Fase 4 — Vuelos reservados por nivel educativo

Preparación de un DataFrame con solo Flights Booked y Education.

Agrupación por Education y cálculo de media, desviación estándar y tamaño de muestra del número de vuelos reservados.

Resultado principal: las medias de vuelos reservados son muy similares entre niveles educativos (≈ 4 vuelos en todos los grupos), con variabilidad también comparable, lo que sugiere que el nivel educativo no parece asociarse a grandes diferencias en vuelos reservados en este dataset.

## Tecnologías utilizadas

Python 3

Pandas para manipulación de datos.

Numpy para operaciones numéricas.

Matplotlib y seaborn para visualización.

Jupyter Notebook / VS Code para el desarrollo del análisis.

Git y GitHub para control de versiones y entrega.

## Cómo ejecutar el proyecto

Clonar el repositorio:
bash

git clone (https://github.com/Adalab/bda-modulo-3-evaluacion-final-Ruthpsegovia.git)


## Autoría

Proyecto desarrollado por Ruth Pérez Segovia

Bootcamp de Data Analytics — Adalab

GitHub: Ruthpsegovia

LinkedIn: https://www.linkedin.com/in/ruthpsegovia/
