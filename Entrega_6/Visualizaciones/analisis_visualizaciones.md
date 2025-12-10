# Análisis General de Visualizaciones  
## *Proyecto: Estadio de Datos – Copa Mundial Sub-20 Chile 2025*

Este documento resume y explica el rol narrativo y técnico de las visualizaciones utilizadas en el reportaje *Estadio de Datos*, organizadas según las cuatro pestañas del sitio web: **Jugadores**, **País por País**, **Comparaciones** y **Top’s**.  
El objetivo es transparentar el proceso detrás de cada grupo de gráficos y mostrar cómo aportan al entendimiento del Mundial Sub-20 desde una perspectiva basada en datos.

---

#  1. Sección: *Jugadores*

###  Propósito narrativo  
Esta sección busca comprender el Mundial desde su nivel más micro: cada futbolista. A través de visualizaciones centradas en minutos jugados, edad y experiencia, se analiza qué tan preparados llegaron los jugadores al torneo.

###  Visualizaciones incluidas  
- Tabla general con todos los jugadores del campeonato

###  Dimensiones analizadas  
- Minutos jugados por temporada  
- Edad del plantel  
- País
- Posición  

###  Mensaje principal  
Las visualizaciones revelan patrones como:
- Selecciones con planteles homogéneos (Marruecos, Francia).  
- Países que dependen de un jugador muy experimentado (Corea, Japón).  
- Planteles completos con pocos minutos (Nueva Zelanda, Panamá).  

Esto permite observar el peso que tiene la experiencia previa en el rendimiento individual y cómo se distribuye dentro de cada equipo.

###  Generación técnica  
- Librerías: **Python + Plotly Express**  
- Archivos exportados: **HTML interactivo**  
- Procesos: limpieza de datos, cálculo de métricas, agregaciones por jugador  

---

#  2. Sección: *País por País*

###  Propósito narrativo  
Esta sección realiza una radiografía de cada selección, permitiendo comparar edad promedio, minutos jugados y experiencia interna por país. Busca entender qué tan equilibrados, jóvenes o experimentados eran los planteles.

###  Visualizaciones incluidas  
- Minutos promedio por selección  
- Edad promedio del plantel  
- Jugador más experimentado de cada equipo  

###  Dimensiones analizadas  
- Minutos promedio del plantel  
- Edad promedio  
- Minutos del jugador con mayor experiencia  

###  Mensaje principal  
Los gráficos muestran que:
- Marruecos, Francia y Colombia tienen los promedios más altos de minutos.  
- Chile y Japón presentan planteles más jóvenes.  
- Algunos países dependen de un jugador con muchos minutos, mientras que otros tienen rodajes más balanceados.  

Esta mirada país por país revela diferentes modelos de formación y exposición al profesionalismo.

###  Generación técnica  
- Bases de datos por selección  
- Cálculo de estadísticas agregadas  
- Visualizaciones creadas con **Plotly**  
- Exportación de gráficos HTML  

---

#  3. Sección: *Comparaciones*

###  Propósito narrativo  
Toma distancia del caso individual o de cada país y compara regiones completas. Busca responder:  
**¿Qué tan diferentes son los contextos formativos entre continentes?**

###  Visualizaciones incluidas  
- América vs Europa: minutos promedio  
- Experiencia en primera división por continente  
- Caso Marruecos: curva de rodaje del campeón  
- Chile vs semifinalistas  

###  Dimensiones analizadas  
- Minutos promedio por confederación  
- Cantidad de jugadores con experiencia profesional  
- Ritmo competitivo comparado  

###  Mensaje principal  
Las comparaciones revelan que:
- Europa tiene la mayor regularidad en experiencia previa.  
- América combina potencias (Argentina, Colombia) con equipos menos expuestos.  
- Marruecos se posiciona entre los planteles con mejor rodaje del torneo.  
- Chile queda por debajo del promedio de semifinalistas.  

Estas diferencias permiten sugerir que los contextos competitivos influyen fuertemente en cómo llega cada selección.

###  Generación técnica  
- Agrupación continental del dataset  
- Operaciones estadísticas por región  
- Exportación en HTML como gráficos interactivos  

---

#  4. Sección: *Top’s*

###  Propósito narrativo  
Esta sección sintetiza patrones clave mediante rankings. Busca mostrar quiénes destacan en términos de experiencia, continuidad o minutos acumulados.

###  Visualizaciones incluidas  
- Top 8 selecciones con más minutos promedio  
- Top 10 jugadores con más minutos jugados  
- Top 3 planteles más y menos experimentados  
- Dispersión de minutaje por selección  

###  Dimensiones analizadas  
- Minutos promedio por selección  
- Minutos individuales por jugador  
- Homogeneidad del plantel  
- Planteles con mayor o menor dispersión interna  

###  Mensaje principal  
Los gráficos permiten observar que:
- Marruecos (campeón) y Francia (semifinalista) están entre los equipos más experimentados del Mundial.  
- México y Brasil son las únicas selecciones no europeas en el top 10 de minutos individuales.  
- Italia aparece como una selección muy experimentada pese a un rendimiento deportivo modesto.  
- Entre las selecciones con menor dispersión están Marruecos y Argentina, los dos finalistas.  
- Entre las más irregulares están Noruega, España, México e Italia, y la mayoría quedó eliminada temprano.  

Estos rankings permiten visualizar la relación entre experiencia previa y desempeño real.

###  Generación técnica  
- Procesos de ranking mediante **pandas**  
- Cálculo de agregaciones para promedios, máximos y desviaciones  
- Exportación interactiva en HTML  

---

#  Conclusión General

Las visualizaciones, organizadas por pestañas, construyen una mirada amplia y profunda del Mundial Sub-20 Chile 2025. En cada nivel —jugador, selección, continente y ranking— aparecen patrones que permiten interpretar el rendimiento deportivo desde su base competitiva.

Si bien los minutos jugados no explican por completo el éxito de una selección, sí muestran tendencias claras:
- los equipos más estables,  
- los planteles más homogéneos,  
- y los jugadores con mayor rodaje  

tendieron a rendir mejor en el torneo.

El lector queda invitado a preguntarse:  
**¿Hasta qué punto la experiencia previa determina el destino de un equipo Sub-20?**

---

