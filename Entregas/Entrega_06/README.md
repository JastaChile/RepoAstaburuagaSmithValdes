# Explicación del proyecto

[Página web](https://jastachile.github.io/RepoAstaburuagaSmithValdes/)

El propósito de esta página web es comparar la relación entre penalización y legalización del aborto con respecto la tasa de embarazos no deseados en cada país.

Para esto, se utilizaron tres bases de datos para recopilar información. En primera instancia, se utilizó una base de datos de la OMS que indica la penalización y legalización del aborto en cada país, y se seleccionaron los siguientes países de Europa y Latinoamérica: Francia, Alemania, Italia, Suiza Finlandia, Holanda, Reino Unido, España, Portugal, Dinamarca, Grecia, Noruega, Argentina, Bolivia, Chile, Colombia, Ecuador, Uruguay, Perú, República Dominicana y Cuba.

Después, se utilizó una base de datos de World Health Organization que muestra los embarazos no deseados cada mil embarazos, alrededor del mundo entre el año 2015 y el 2019, que cuenta con un intervalo de confianza del 95%. Para limpiar la base de datos se seleccionaron los siguientes países ubicados en Europa y Latinoamérica: Francia, Alemania, Italia, Suiza Finlandia, Holanda, Reino Unido, España, Portugal, Dinamarca, Grecia, Noruega, Argentina, Bolivia, Chile, Colombia, Ecuador, Uruguay, Perú, República Dominicana y Cuba.

Finalmente, se utilizó una base de datos sobre la tasa de aborto, incluyendo estimaciones de la tasa de aborto por cada 1000 mujeres en edad reproductiva (15-49 años) para varios países y territorios. Las estimaciones se proporcionan con intervalos de incertidumbre del 95%.

Con la primera base de datos, se construyó un mapa interactivo que indica en qué países seleccionados de Europa y Latinoamérica está legalizado el aborto, marcados por un círculo verde, y en qué países está penalizado el aborto, marcados por un círculo rojo. Esto con el fin de contrastar la tendencia entre Europa hacia la legalización y la tendencia en Latinoamérica hacia la penalización, a excepción de Argentina, Cuba y Uruguay. En el caso de Europa, corresponden a poses desarrollados, con una mejor economía, acceso educacional y salud. Los países de Latinoamérica en donde el aborto está legalizado, son justamente los países en donde la salud y la educación son gratis.

Entonces, en base a esta diferencia en las leyes abortivas, analizamos la tasa de embarazos no deseados existente en cada uno de estos países. Para esto se construyó un gráfico de barras horizontales, y se ordenaron los datos de forma decreciente, para poder dimensionar que los países que presentan una mayor tasa son los países de Latinoamérica.

Si se observa la cantidad de embarazos no deseados que existen en cada continente, considerando la penalización o legalización del aborto, es posible dimensionar a través de este gráfico, que la tendencia está en Latinoamérica, pero los países que presentan una tasa menor de embarazos no deseados son los países Europeos y los países de Latinoamérica en donde el aborto está legalizado.

Es decir que existe una relación directa entre la legalización, penalización y la cantidad de embarazos no deseados. Países en donde el aborto está legalizado, presenta una menor tasa de embarazos no deseados y países donde el aborto está penalizado, presenta una mayor tasa de embarazos no deseados.

Utilizamos información de la base de datos de la OMS acerca de las mayores y menores tasas de aborto en el mundo, para descartar la hipótesis de que Europa pudiese presentar una menor tasa de embarazos no deseados, debido a que existan mas abortos por el derecho legal de abortar. Sin embargo, se construyó un gráfico que demuestra que los países europeos son los que presentan menores tasas de aborto a nivel mundial.
Entonces, la relación que se construye es que los países en donde el aborto está legalizado, presentan una menor tasa de embarazos no deseados y al mismo tiempo las menores tasas de aborto, es decir, que la mayoría de los embarazos gestados son deseados.

En un país donde el aborto está legalizado, existen embarazos más responsables, por ende una menor tasa de embarazos no deseados. Y esto se debe a la presencia de educación sexual.

Para evidenciar la calidad de educación sexual, se utilizaron
datos de la UNESCO, OMS Y UNSFPA, que consideran factores como amplitud y profundidad del currículo de educación sexual, obligatoriedad de la educación sexual en el sistema educativo, edad de inicio de la educación sexual, formación de los educadores en temas de sexualidad, políticas nacionales sobre educación sexual y salud reproductiva y reportes de organizaciones, y miden una escala de calidad de educación sexual de 0-100, en donde 0 representa la ausencia total y 100 representa una educación sexual integral, obligatoria y basada en evidencia científica.

De esta manera, se construyó un gráfico que combina estos datos, con resultados de las tasas de embarazos no deseados, en donde es posible visualizar que existe una línea decreciente en calidad de educación sexual, a medidas que crece que la tasa de embarazos no deseados. Esto quiere decir que hay una relación inversamente proporcional entre la calidad de educación sexual y la tasa de embarazos no deseados.
Entonces, se puede concluir que:

Los países en donde está legalizado el aborto, suelen ser países europeos, que cuentan con acceso gratuito a anticonceptivos, con una alta calidad en materias de educación sexual y tienen una menor tasa de embarazados no deseados.
Los países en donde está penalizado el aborto, suelen ser países latinoamericanos, a excepción de Argentina, Uruguay y Cuba, donde la educación y la salud es gratuita, presentan a acceso a anticonceptivos, pero una baja calidad en materias de educación sexual y, finalmente, presentan una mayor tasa de embarazados no deseados.

El factor común es el acceso gratuito a anticonceptivos, pero los países que cuentan con una legalización del aborto invierten más recursos en educación sexual, y los países en donde está penalizado invierten menos.
Eso se ve reflejado en las tazas de embarazados no deseados, en donde existe una tendencia en la medida en que la educación sexual es de baja calidad

## DISEÑO DE PÁGINA

Disclaimer: Tanto el estilo de la página cómo las funcionalidades de código fueron implementadas directamente en el archivo index.html, por lo que no se utilizan scripts extras de tipo CSS ni JavaScript.

- Paleta de colores: #DF6C92, #DEF6CA, #6457A6, #1B1B3A

- Tipografía de letra: IBM Plex Sans

### Contenido del index.html:

Estructura del Documento:

```
<!DOCTYPE html>
```

- Declara el tipo de documento y la versión de HTML.

```
<html lang="es">
```

- Define el lenguaje del documento como español.

```
Leaflet: Biblioteca para crear mapas interactivos.
Plotly: Biblioteca para gráficos interactivos.
Chart.js: Biblioteca para gráficos.
Metaetiquetas: Define la codificación de caracteres y la vista para dispositivos móviles.
Título: "Aborto en Europa y Latinoamérica".
Estilos CSS: Incluye estilos para la página, tales como la tipografía, el diseño de contenedores de gráficos, y el diseño de las tarjetas del equipo.
```

- Enlaces a Estilos y Scripts.

```
<header>
```

- Contiene el logo del proyecto.

```
<main>
```

- Sección principal con varios bloques de contenido.

```
<section>
```

- Diferentes secciones para mostrar el análisis. Acá se encuentran los gráficos y el contenido principal del reportaje.

```
<footer>

```

- Contiene información de contacto y un enlace al repositorio del proyecto en GitHub.

### Scripts JavaScript

- Leaflet Map: Crea un mapa interactivo con puntos que representan países donde el aborto es legal o penalizado.

#### Plotly Graphs:

- Tasa de Embarazos No Deseados: Gráfico de barras que muestra la tasa de embarazos no deseados por país.
- Tasa de Aborto por País: Gráfico de barras que muestra la tasa de aborto por país.
- Chart.js Graph: Crea un gráfico de barras para la tasa de embarazos no deseados y la calidad educativa.

## Ponderador de autoría

Una X señala que el/la integrante trabajó más en el elemento correspondiente:

| Elemento  | Astaburuaga | Smith | Valdés |
| :-------- | :---------- | :---- | :----- |
| Gráfico 1 |             | X     |        |
| Gráfico 2 |             |       | X      |
| Gráfico 3 | X           |       |        |
| Gráfico 4 | X           | X     | X      |
