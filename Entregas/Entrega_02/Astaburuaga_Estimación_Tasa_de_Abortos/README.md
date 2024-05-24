# Proceso de Limpieza de Datos de la Tasa de Aborto

## Breve descripción de los Datos
La base de datos de la OMS sobre la tasa de aborto incluye estimaciones de la tasa de aborto por cada 1000 mujeres en edad reproductiva (15-49 años) para varios países y territorios. Las estimaciones se proporcionan con intervalos de incertidumbre del 80% y del 95%.

## Pasos Realizados

### 1. Cargar los Datos
En primer lugar, se descargaron los datos desde [este link](https://www.who.int/data/gho/data/indicators/indicator-details/GHO/SRH_ABORTION_RATE), los cuales venían en formato csv. Este archivo fue subido a un notebook en google colab para trabajar correctamente con él.

### 2. Eliminar Columnas con Valores Constantes
Inicialmente se cargan los datos desde el archivo CSV a un DataFrame de pandas. Eliminamos todas las columnas en las que el valor es el mismo para todas las filas. Esto incluye las columnas donde todos los valores son NaN (no disponibles) o constantes. Este paso es crucial para reducir la cantidad de datos redundantes y enfocarnos en la información relevante.

### 3. Separar y Renombrar Estimaciones de Incertidumbre
Para cada país, hay dos filas: una con una estimación del 80% de incertidumbre y otra con una del 95%. Creamos dos DataFrames separados para estas estimaciones. Luego, renombramos las columnas que cambian (como las estimaciones numéricas bajas y altas, y el valor de la tasa) para diferenciarlas claramente entre las estimaciones del 80% y del 95%.

### 4. Combinar los DataFrames
Utilizamos las columnas comunes a ambos DataFrames (como `ParentLocation`, `SpatialDimValueCode` y `Location`) para combinarlos en un solo DataFrame. Esto nos permite tener todas las estimaciones para un país específico en una sola fila, con las columnas diferenciadas para las estimaciones del 80% y del 95%.

### 5. Limpiar Columnas de Valores
Para las columnas que contienen los valores de las estimaciones (denominadas `Value_80` y `Value_95`), extraemos solo el primer número antes de cualquier rango de incertidumbre que pueda estar entre corchetes. Este paso asegura que los valores sean consistentes y numéricos, eliminando información redundante.

### 6. Guardar los Datos Limpios
Finalmente, exportamos el DataFrame limpio a un nuevo archivo CSV. Este archivo contiene todos los datos relevantes, organizados y listos para su análisis posterior.

## Observaciones
Este proceso de limpieza asegura que los datos estén en un formato óptimo para análisis posteriores, manteniendo únicamente las columnas esenciales y eliminando duplicados o valores constantes innecesarios. Específicamente, se retienen solo las columnas que se refieren a la identificación del país, la región continental, y los valores de las dos estimaciones de tasas de aborto, junto con sus respectivos intervalos de incertidumbre. La decisión de conservar ambas estimaciones de tasas para cada país permite realizar un análisis más completo y detallado de la situación. Al mantener tanto las estimaciones al 80% como al 95% de incertidumbre, se proporciona una visión más rica y precisa de la variabilidad y fiabilidad de los datos, lo que es crucial para comprender las dinámicas subyacentes y apoyar la toma de decisiones informadas en políticas de salud pública y reproductiva. Este enfoque integral nos capacita para identificar patrones, evaluar riesgos y diseñar intervenciones más efectivas y contextualizadas para abordar las necesidades de salud reproductiva a nivel global y regional.
