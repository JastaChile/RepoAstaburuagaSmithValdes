# Ficha Técnica

## Característica de los datos

Los datos corresponden a estimaciones realizadas por la World Health Organization disponibles en [este enlace](https://www.who.int/data/gho/data/indicators/indicator-details/GHO/SRH_ABORTION_RATE). La página proporciona una estimación modelada del índice de abortos por cada 1000 mujeres en edad reproductiva (15-49 años) en diferentes países y territorios. Utiliza un modelo bayesiano para calcular estas tasas a partir de datos sobre necesidades y uso de anticonceptivos, métodos anticonceptivos, tasas de natalidad y datos de incidencia de abortos. Estos datos se desglosan en agregados regionales y globales, considerando dos intervalos de incertidumbre por país al 80% y al 95%.

## Alcance metodológico

El alcance de estos datos abarca múltiples fuentes de información, incluyendo sistemas nacionales de información de salud y encuestas basadas en la población. Las estimaciones se publican cada cinco años y se utilizan para monitorear y evaluar la necesidad de cuidados relacionados con el aborto seguro, con el objetivo de prevenir la mortalidad y morbilidad maternas derivadas de abortos inseguros. La base de datos también proporciona agregados regionales y globales, clasificando los datos dentro de las regiones de los Objetivos de Desarrollo Sostenible (ODS) de la ONU.

## Variables incorporadas:

Las variables a destacar de la base son las siguientes:

- Location: Nombre del pais.
- Parent_Location: Continente al que pertenece el país.
- Value_80: Cantidad estimada de la tasa de abortos con 80% de incertidumbre.
- Value_95: Cantidad estimada de la tasa de abortos con 95% de incertidumbre.
- FactValueNumericLoq, FactValueNumericHigh: Para cada porcentaje de incertidumbre, estas columnas definen el intervalo de incertidumbre alrededor de la estimación de la tasa de abortos. Por ejemplo, si una tasa de aborto es estimada en 30 [20, 40], significa que la tasa estimada es 30 abortos por cada 1000 mujeres en edad reproductiva, pero podría estar entre 20 y 40.
