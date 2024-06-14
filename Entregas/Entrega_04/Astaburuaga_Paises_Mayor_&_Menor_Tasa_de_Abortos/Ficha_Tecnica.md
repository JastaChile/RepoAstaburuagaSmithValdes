# Ficha Técnica

## Característica de los datos

Los datos corresponden a estimaciones realizadas por la World Health Organization disponibles en [este enlace](https://www.who.int/data/gho/data/indicators/indicator-details/GHO/SRH_ABORTION_RATE). La página proporciona una estimación modelada del índice de abortos por cada 1000 mujeres en edad reproductiva (15-49 años) en diferentes países y territorios. Utiliza un modelo bayesiano para calcular estas tasas a partir de datos sobre necesidades y uso de anticonceptivos, métodos anticonceptivos, tasas de natalidad y datos de incidencia de abortos. Estos datos se desglosan en agregados regionales y globales, considerando dos intervalos de incertidumbre por país al 80% y al 95%.

## Sobre la visualización:

Se utilizó un gráfico de barras, en dónde el eje Y representa la tasa estimada de abortos por cada 1000 mujeres con una estimación al 95% de incertidumbre, y el eje X corresponde a cada uno de los países. Del lado izquierdo se muestran los 10 países con mayores tasas de aborto y del lado derecho los 10 países con menores tasas, ordenados todos de manera descendente. Además, se utiliza un código de color para cada conjunto, con morado para los países con mayores tasas y rojo para los que tienen una tasa menor.

## Variables incorporadas:

Para esta visualización, se utilizaron las siguientes variables

- Location: Nombre del pais.
- Value_95: Cantidad estimada de la tasa de abortos con 95% de incertidumbre.
