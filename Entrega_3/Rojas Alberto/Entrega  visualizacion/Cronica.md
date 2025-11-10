# Comparativa de minutos jugados entre Sudamérica y Europa


Crónica explicativa del análisis comparativo

El objetivo del trabajo fue comparar el promedio de minutos jugados por selección en primera división entre las selecciones de Sudamérica y Europa, con el propósito de observar posibles diferencias en la participación de jugadores pertenecientes a cada región en las principales ligas del mundo.

Para ello, se elaboró una base de datos simplificada con el promedio de minutos jugados por distintas selecciones nacionales: Italia, Francia, Noruega, España y Ucrania por parte de Europa; y Argentina, Colombia, Brasil, Paraguay y Chile por Sudamérica. Estos datos se organizaron en tres columnas: el nombre de la selección, la región a la que pertenece y el promedio de minutos jugados.

El análisis se realizó mediante Python en Google Colab, utilizando las librerías pandas y matplotlib, que permiten trabajar con datos tabulares y generar visualizaciones gráficas, respectivamente.

En primer lugar, se cargaron los datos en un DataFrame de pandas, lo que permitió manipular la información de forma estructurada.

Posteriormente, se aplicó una agrupación por región (groupby) para calcular el promedio general de minutos jugados en Sudamérica y en Europa.

A partir de estos resultados, se calculó también la diferencia promedio entre ambas regiones.

Finalmente, se generaron dos gráficos con matplotlib:

Un gráfico de barras comparativo por región, que muestra de manera visual cuál es la diferencia promedio de minutos entre Sudamérica y Europa.

Un gráfico individual por selección, en el que cada barra representa el promedio de minutos de una selección específica, con un color distinto según su región.

Ambos gráficos fueron exportados como imágenes (.png) para su posterior uso en GitHub o informes académicos.

El análisis evidenció que, en promedio, las selecciones europeas presentan una cantidad significativamente mayor de minutos jugados en primera división respecto a las selecciones sudamericanas. Este resultado sugiere una mayor presencia o participación de futbolistas europeos en ligas de alto nivel, lo cual podría explicarse por factores como la localización geográfica de las principales competiciones, la infraestructura deportiva o la distribución de oportunidades profesionales entre continentes.

En conclusión, el procedimiento permitió visualizar de manera clara y cuantitativa una diferencia estructural entre regiones futbolísticas, mostrando cómo el análisis de datos y la visualización gráfica pueden contribuir al estudio comparativo del rendimiento y participación internacional de los jugadores.
