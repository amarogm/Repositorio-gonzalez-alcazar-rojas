# Documentación de la visualización – Mundial Sub-20

## 1. Proceso de visualización

1. **Selección de datos:** Se utilizaron las nóminas oficiales de las selecciones participantes en el Mundial Sub-20.  
2. **Preparación de datos:** Se extrajo el promedio de minutos jugados de cada jugador en fútbol profesional, calculando un promedio por selección.  
3. **Limpieza de datos:** Se verificaron valores faltantes y se corrigieron formatos de número. Se eliminaron duplicados y se revisó que todos los nombres de selecciones estuvieran correctamente escritos.  
4. **Visualización:** Se utilizó **Altair en Python** para crear un gráfico de barras mostrando las selecciones y sus promedios de minutos jugados.  
5. **Exportación:** Se generó un archivo **HTML interactivo** (`visualizacion_minutos.html`) y un **JPG** (`visualizacion_minutos.jpg`) para incluir en la crónica.

---

## 2. Ficha técnica de la base de datos

- **Variables:**

| Variable           | Descripción                                           |
|-------------------|-------------------------------------------------------|
| Seleccion          | Nombre de la selección participante                 |
| Minutos_promedio   | Promedio de minutos jugados por los jugadores       |

- **Observaciones:**  
  - Los datos corresponden a minutos acumulados en partidos profesionales antes del Mundial Sub-20.  
  - No se incluyeron jugadores sin minutos registrados.  
  - Debido a que un compañero dejó el ramo, **nos faltaron algunas variables que originalmente queríamos agregar**.  
  - Ahora, como el Mundial está finalizando, planeamos **buscar una fuente adicional de datos** para complementar la base y que la visualización sea más completa.  
  - La base de datos fue seleccionada por su relevancia directa para la hipótesis sobre experiencia y desempeño.

---

## 3. Ejemplos de preguntas que puede responder la visualización

1. ¿Qué selecciones tienen jugadores más experimentados antes del inicio del torneo?  
2. ¿Cómo se sitúa Chile en comparación con otras selecciones en términos de experiencia profesional?  
3. ¿Existen diferencias regionales o continentales en la cantidad de minutos jugados por los jugadores?  
4. ¿La experiencia de los jugadores (minutos jugados) se relaciona con los resultados finales del Mundial Sub-20?  
