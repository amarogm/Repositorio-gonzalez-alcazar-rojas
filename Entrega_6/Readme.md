# Análisis de diseño de la historia – Estadio de Datos

## 1. Estructura narrativa y recorrido del usuario

La webstory está construida como un recorrido progresivo desde el contexto general hacia el detalle:

1. **Portada (index.html)**  
   - Presenta el título, la bajada y una imagen principal asociada al Mundial Sub-20 Chile 2025.  
   - Introduce la pregunta central: ¿qué papel juegan los minutos y la experiencia previa en el rendimiento de las selecciones juveniles?

2. **Introducción (“¿Cómo partió todo?”)**  
   - Explica el origen de la duda periodística: la idea de “ritmo competitivo” y su peso real en un torneo Sub-20.  
   - Plantea que, en lugar de quedarse en la intuición, el proyecto decide entrar al terreno de los datos.

3. **Secciones temáticas del index**  
   - **Jugadores**: abre la mirada a nivel individual, invitando a explorar quiénes son los protagonistas del torneo y cómo llegaban en términos de minutos, edad y posición.  
   - **País por país**: cambia la escala y permite ver cómo se compone cada plantel, con especial énfasis en promedios y líderes internos.  
   - **Comparaciones**: cruza regiones, confederaciones y contextos, enriqueciendo la mirada global del torneo.  
   - **Top’s**: resume la información en rankings que ayudan a identificar extremos (más/minutos, más/menos experiencia, etc.).  
   - **Metodología y conclusiones**: transparentan el proceso y elaboran una interpretación abierta para el lector.

4. **Páginas internas (jugadores, país, comparaciones, tops)**  
   Cada pestaña replica el estilo visual del index (header con fondo verde/negro, navegación fija, hero con imagen) y profundiza en un tipo de análisis:  
   - `jugadores.html`: foco en el individuo.  
   - `pais.html`: foco en los planteles.  
   - `comparaciones.html`: foco en las diferencias entre regiones y modelos de desarrollo.  
   - `tops.html`: foco en extremos y liderazgos estadísticos.

El recorrido propuesto para el usuario puede ser lineal (desde el index hacia las páginas internas) o modular (entrar directamente a la sección que más le interese), pero la narrativa está pensada para que cada capa se apoye en la anterior.

---

## 2. Diseño de la información e interacción

### a) Organización de la información

- El contenido se agrupa en **bloques temáticos claros**: contexto, jugadores, países, comparaciones, tops, metodología, conclusiones.  
- Cada bloque combina **texto narrativo** y **visualizaciones**, de forma que los datos no aparezcan aislados, sino siempre acompañados de interpretación periodística.
- Las visualizaciones se insertan dentro de secciones con títulos y subtítulos descriptivos, seguidos de un **análisis en párrafos espaciados**, lo que facilita la lectura y evita el “ruido visual”.

### b) Interacción y navegación

- El menú principal (`nav`) se mantiene consistente en todas las páginas, lo que permite moverse entre secciones sin perder el contexto.
- Se utilizan **llamados a la acción internos** (`→`) para invitar a abrir páginas específicas (por ejemplo, “País por país →”).
- El botón inferior (“pito”) y el uso de anclas (`#top`) permite regresar fácilmente al inicio, reforzando la sensación de recorrido controlado.
- La presencia de **iframes para cada visualización** mantiene la experiencia integrada: el usuario no tiene que salir del sitio para ver los gráficos.

---

## 3. Estilo narrativo y decisiones textuales

### a) Tono periodístico–interpretativo

Los textos no solo describen lo que se ve en los gráficos, sino que:

- Formulan **preguntas** (“¿Es más fácil para ciertas ligas integrar juveniles al profesionalismo?”, “¿Cuánto determinan realmente los minutos el rendimiento en un Sub-20?”).  
- Evitan presentar la hipótesis como una verdad absoluta, dejando espacio a la interpretación del lector.  
- Alternan entre **explicación técnica** (minutos, promedios, dispersión) y **lenguaje narrativo** (“los líderes ocultos detrás del Mundial”, “mirar el torneo desde arriba”).

### b) Estructura de los textos

- Cada visualización va acompañada de un **título informativo** y un análisis dividido en párrafos cortos, con clases como `spaced` para mejorar la legibilidad.  
- La **conclusión general** no cierra la historia con una afirmación categórica, sino con una invitación al lector a reflexionar sobre la relación entre datos y rendimiento deportivo.

---

## 4. Decisiones visuales y su significado

### a) Paleta de colores

- El sitio utiliza una paleta basada en **verdes oscuros, negros y grises**, que remiten directamente al imaginario del fútbol:  
  - Verde = cancha, pasto, juego.  
  - Negro / gris oscuro = pizarras tácticas, foco en el análisis.  
- El uso de brillos y sombras en verde (`var(--verde-pasto)`) refuerza la idea de estar “bajo las luces del estadio”, pero en clave de datos.

### b) Tipografías

- **Oswald**: para títulos, da un aire deportivo, fuerte y directo.  
- **Montserrat / Lato**: para el cuerpo de texto, priorizando la legibilidad en pantalla y dando una sensación moderna, propia de medios digitales.

Esta combinación busca un equilibrio entre **estética periodística** y **lenguaje visual deportivo**, coherente con un reportaje de datos sobre fútbol.

### c) Logo y elementos gráficos

- El logo de “Estadio de Datos” y las imágenes de balones, estadios y jugadores funcionan como **anclas visuales**: recuerdan constantemente al usuario que, aunque está mirando gráficos, sigue en el contexto del Mundial Sub-20.
- El “pito” como botón de retorno al inicio agrega un guiño lúdico al diseño, manteniendo la identidad futbolera sin romper el tono serio del análisis.

### d) Coherencia visual entre páginas

- Todas las pestañas (index, jugadores, país, comparaciones, tops) comparten:  
  - El mismo **header con fondo degradado** verde–negro.  
  - La misma **estructura de hero** (título + subtítulo + imagen).  
  - El mismo estilo de `section` y `ed-section__content`.  

Esto refuerza la idea de que cada página no es un sitio independiente, sino un **capítulo dentro de una misma historia**.

---

## 5. Cómo el diseño refuerza la historia de las visualizaciones

- Las visualizaciones no están “sueltas”, sino insertas en un relato que:  
  - Presenta primero el contexto (qué es el Mundial, por qué mirar minutos).  
  - Luego baja a jugadores, sube a países, compara regiones y finalmente resume en rankings.  
- El diseño visual acompaña esta progresión:  
  - Los **colores oscuros y el verde** aportan una sensación de profundidad y análisis, casi como ver el torneo desde la cabina de prensa o desde el VAR de los datos.  
  - Las animaciones suaves (`fade-in`, `float-soft`) hacen que los elementos aparezcan de forma progresiva, reforzando la idea de ir descubriendo capas de información.  
  - Los textos estructurados por bloques narrativos y análisis de gráficos le dan al usuario una **ruta clara de lectura**, aún cuando la historia es compleja.

En conjunto, el diseño y la narrativa están pensados para que el usuario no solo vea gráficos, sino que **entienda por qué importan** y cómo se conectan con la pregunta central del reportaje:  
> **¿Qué papel juega realmente la experiencia —medida en minutos— en el rendimiento de un Mundial Sub-20?**
## Tabla de Autoría

## Tabla de Autoría

| Integrante        | Rol Principal                                | Aportes Específicos                                                                                     |
|------------------|------------------------------------------------|-----------------------------------------------------------------------------------------------------------|
| **Amaro González** | Creador y diseñador de la página web; creador de bases de datos | Desarrollo completo de la webstory; diseño visual y estructural; redacción narrativa; integración de visualizaciones; experiencia de usuario; coherencia estética y narrativa; creación total de las bases de datos utilizadas en el proyecto. |
| **Alberto Rojas** | Creador de gráficos y visualizaciones         | Generación de los gráficos utilizados en el reportaje; apoyo parcial en la elaboración de la primera base de datos; participación en el análisis estadístico vinculado a las visualizaciones. |
