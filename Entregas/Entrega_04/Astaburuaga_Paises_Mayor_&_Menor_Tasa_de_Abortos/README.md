# Visualización Tasa de Aborto

## Descripción de los Datos

La base de datos de la OMS sobre la tasa de aborto incluye estimaciones de la tasa de aborto por cada 1000 mujeres en edad reproductiva (15-49 años) para varios países y territorios. Las estimaciones se proporcionan con intervalos de incertidumbre del 80% y del 95%, siendo esta últimaa estimación la utilizada para esta visualización.

## Pasos Realizados

### 1. Carga de datos y toma de decisiones

En primer lugar se cargaron los datos limpiados previamente en la entrega 2. Luego de considerar la dimensionalidad de los datos que disponibles en este set y teniendo en cuenta la historia que se busca contar, se toma la decisión de construir una visualización que permita realizar una comparación entre los valores más extremos del set. De esta forma podemos analizar el nivel de desigualdad en el mundo en cuánto a la métrica observada (tasas de aborto) y poder obtener conclusiones al buscar las causas de dicha desigualdad, creando así una visualización que entregue valor a la crónica que se está desarrollando.

### 2. Construcción de las primeras visualizaciones

En primer lugar construimos dos gráficos de barra que mostraran los países con las tasas más bajas y más altas de abortos disponibles en la base de datos. Para ello se utiliza la librería matplotlib de python en conjunto con la librería pandas para ordenar y filtrar el dataset.

### 3. Elaboración de la visualización final

Para la visualización final, se decide combinar los dos gráficos de barras mencionados anteriormente en una sola figura, con el objetivo de realizar una comparación más evidente y fácil de entender. Finalmente, esta es exportada tanto a formato html como png.

## Observaciones

Se decidió utilizar un gráfico de barras por su simpleza y eficacia al mostrar datos concretos como los de este conjunto de datos. Este tipo de gráfico facilita la comparación directa de las tasas de aborto entre los países, permitiendo identificar rápidamente las diferencias significativas gracias a su estructura sencilla y clara, basada en datos directos que muestran la tasa de abortos por país. Esta simplicidad facilita la comprensión inmediata de las grandes disparidades entre los países con las tasas más altas y más bajas de aborto para cualquier persona que observe la gráfica.

### Algunas de las preguntas que la visualización podría responder:

- ¿Tienen algo en común los países con mayores o menores tasas de aborto?

- ¿Cuál es la variabilidad de las tasas de aborto entre todos los países del set de datos?
