
<!-- Este .md fue generado a partir del .Rmd homónimo. Edítese el .Rmd -->

# Programa de “Geomorfología” <br/> Licenciatura en Geografía <br/> Universidad Autónoma de Santo Domingo (UASD)

Enero 2020 <br/> *José Ramón Martínez Batlle*

## Básicos:

  - Correo: <jmartinez19@uasd.edu.do>
  - Lugar y horario: FC-203, Martes de 2 a 6 pm

## URLs del contenido del curso:

  - [Programa (hipervínculo recursivo)](programa-geomorfologia.md)
  - [¿Cómo realizar una asignación?](ref/como-hacer-una-asignacion.md)
  - [Guía mínima de RMarkdown](ref/guia-minima-de-rmarkdown.md)
  - [Introducción a R](ref/introduccion-a-r.md)

## Descripción

> Earth’s landscapes are sculpted by a suite of geomorphic processes
> that vary with position on the Earth and with time due to changes in
> the climate. Landscapes contain signatures of the principal active
> processes that we would like to learn to read (Anderson & Anderson,
> 2010).

> Los paisajes de la Tierra son esculpidos \[modelados\] por un conjunto
> de procesos geomorfológicos que cambian según la posición en el
> planeta y en el tiempo debido a cambios en el clima. Los paisajes
> contienen “firmas” \[registros\] del **principal proceso activo**, el
> cual “nos \[te\] interesa \[para aprobar o para lo que veas\]”
> aprender a leer (Anderson & Anderson, 2010).

Guarda ésto: “…el principal proceso activo en la configuración del
paisaje…”, y quédate también con esta otra cita:

> La Geomorfología, como otras ramas de la ciencia, necesita pasar de la
> simple descripción a la cuantificación y para ello tiene que utilizar
> métodos de otras áreas científicas, fundamentalmente la Física
> (Gutiérrez Elorza, 2008)

Tricart (1956) auguraba que la Geomorfología debía apoyarse en el
estudio de los procesos y también en la morfogénesis antrópica. No se
equivocó, porque desde mediados del siglo XX hasta la actualidad, la
geomorfología de procesos ha sido la nota dominante. Este enfoque se
preocupa más por el proceso que por la forma, lo cual deja de lado la
evolución de los grandes conjuntos de relieve (Gutiérrez Elorza, 2008).

Dos grupos de procesos geomorfológicos convergen en la superficie del
planeta:

1.  Las rocas de la superficie son movidas por procesos geofísicos
    profundos.

2.  La atmósfera es movida por una distribución desigual de la radiación
    solar.

Aunque seguiré un guión de geomorfología de procesos, no olvidaré
aproximaciones geomorfológicas tradicionales que, de otra manera,
quedarían excluidas del programa (e.g. geomorfología litológica y
evolutiva).

La geomorfología de procesos no sería posible sin el avance de los
últimos siglos en matemáticas. Igualmente, sin la irrupción de la
tecnología y el desarrollo de la programación en la segunda mitad del
siglo XX, tampoco sería posible estudiar procesos a escalas grandes.
Estas herramientas han permitido que la geomorfología dé respuestas cada
vez más precisas a problemas de ciencias de la Tierra, como los riesgos
de desastres.

Puedes presuponer seguiré un esquema de geomorfología de procesos
(to’eta plepla no e’de’barde), pero en esta edición además introduciré
soporte matemático y aplicaciones tecnológicas usando software de código
abierto, centrando el aprendizaje en asignaciones y en un manuscrito que
escribirás.

**Me apoyaré en [R](https://www.r-project.org/) y en [GRASS
GIS](https://grass.osgeo.org/)** (las vainas del tali), y tienes la
opción de usar Python. Para visualizar salidas, opcionalmente podrás
usar [QGIS](https://qgis.org/es/site/) (por ejemplo, localmente en una
PC tuya o en las del SIGCART). Con suerte, y si alcanza el tiempo, verás
posibles usos de [OpenDroneMap](https://www.opendronemap.org/) en
geomorfología.

En cuanto a escribir código, te adelanto que para superar las
dificultades y los desafíos que te supongan las asignaciones y el
manuscrito, tendrás que:

1.  Sufrir. Nadie dijo que fajarse con R, GRASS o Python iba a ser como
    una sesión de coaching. Cuesta esfuerzo y mucho. Lo mismo aplica a
    la redacción; escribir con concisión apoyándote en tus resultados es
    tarea complicada. Por lo tanto, sufre, pero con un motivo.

2.  Recibir tutorías. Estoy de lunes a jueves, de 8 am a 1 pm en la
    pecera del piso 7 (Facultad de Ciencias) del “Edificio
    Administrativo”. No necesitas cita previa, pero recomiendo que me
    escribas (jmartinez19@uasd.edu.do) por si tuviese compromisos fuera
    el día que elijas visitarme.

3.  Aprender a pedir ayuda. Elimina esta expresión de tu cabeza: “Da
    error”. Con eso nadie puede ayudarte. Lo importante es qué error
    obtienes al ejecutar qué cosa. Por ello, cuando pidas ayuda, por
    ejemplo, mediante *issues* de GitHub, deberás ofrecer un ejemplo
    reproducible. Evita las capturas de pantalla y prefiere código
    reproducible + error.

No tendrás que preocuparte por el hardware (ya me ensucio yo las manos
con esa cosa tan mundana llamada computadora), pero ocúpate por razonar
bien las asignaciones y, especialmente, lo que escribas en tu
manuscrito. Dispondrás de un servidor de RStudio de modestas
prestaciones habilitado por mí, con los paquetes requeridos en el curso
ya pre-instalados. Así podrás realizar tus asignaciones sin preocuparte
de instalaciones ni dependencias.

Parecería “natural” utilizar interfaz gráfico de usuario para analizar
datos geomorfológicos, pero verás a lo largo de esta asignatura que lo
razonable es utilizar código. Realizar de manera eficiente análisis
reproducibles sólo se logra escribiendo y ejecutando código. Igualmente,
para visualizar patrones espaciales se requiere de herramientas
versátiles, que tanto R como otros lenguajes proveen normalmente a
través de paquetes.

## Manuscrito

> El plagio y la falsificación de datos supondrán la reprobación
> inmediata de la asignatura.

### Presentación oral

Dispondrás de 15 minutos para presentar oralmente tu trabajo al final de
la asignatura. Valoraré el dominio que muestres sobre tu trabajo.

### Código informático reproducible

Este es el fuerte de la asignatura, y es imprescindible para culminar
con éxito tu proyecto. Por correo electrónico, te enviaré asignaciones
que te ayudarán a construir tu código reproducible. Las podrás realizar
utilizando el servidor RStudio habilitado por el profesor (sólo
necesitarás una PC con conexión a Internet y un navegador), o utilizando
tu propia PC, pero en este último caso tendrás que instalar R, RStudio y
los paquetes requeridos.

Orientaré con ejemplos y soluciones a través de *issues* que abrirás tú
o yo en el GitHub. De esta forma las discusiones quedarán disponibles
para otras personas. Evita preguntar por correo electrónico, porque
cualquier consulta que realices, así como las posibles soluciones que
surjan, quedarán en privado y sólo serán aprovechables por ti.

Al abrir un *issue* de GitHub debes plantear el problema al que te
enfrentas, cómo has intentado resolverlo o qué soluciones has probado.
Si se trata de cuestiones relacionadas con programación o análisis de
datos, deberás aportar **código reproducible y mensaje de error (si lo
hubiere)**. Evita el típico comentario “da error”, puesto que no conduce
a nada.

## Examen basado en código

Bueno, sobre ésto tengo poco que decir, sólo que preferiría no evaluar
por medio de exámenes.

## Contenido de la asignatura

El típico “temario” de la asignatura, AKA “teoría”, el cual impartiré
con breves introducciones, pero principalmente por medio de
asignaciones. En la medida de lo posible, haré que este contenido sea de
utilidad para los proyectos.

1.  Datos espaciales, y datos espaciales en R (tipos, importar,
    exportar). Capítulo 1 de Loonis & Bellefon (2018), capítulos 1 a 3
    de Lovelace, Nowosad, & Muenchow (2019), capítulos 1 y 2 de Bivand,
    Pebesma, & Gomez-Rubio (2008), capítulo 3 y 4 de Mas (2013).

2.  Manipulación de datos espaciales (operaciones con atributos y
    geométricas). Capítulos 2, 4 y 5 de Bivand et al. (2008), capítulos
    3 a 5 de Lovelace et al. (2019), capítulo 5 de Mas (2013), capítulo
    10 de Olaya (2014).

3.  Vecindad y autocorrelación espacial (análisis exploratorio,
    funciones de homogeneidad espacial, tipos de vecindad, ponderadores,
    índices). Sección 9.2 de Bivand et al. (2008), Capítulos 2 y 3 de
    Loonis & Bellefon (2018), capítulo 12 de Olaya (2014), capítulos B.2
    y B.3 de Fischer & Getis (2009).

4.  Datos puntuales, geoestadística (funciones aleatorias, variograma,
    kriging). Capítulo B.6 de Fischer & Getis (2009), Capítulos 1, 2, 5
    y 6 de Hengl (2009), capítulos 4 y 5 de Loonis & Bellefon (2018),
    capítulos 7 y 8 de Bivand et al. (2008), capítulo 7 de Mas (2013),
    capítulo 13 de Olaya (2014),

5.  Modelización de entidades poligonales. Capítulo 9 de Bivand et al.
    (2008), capítulos 6 a 9 de Loonis & Bellefon (2018), capítulos C.1 a
    C.7 de Fischer & Getis (2009).

## Referencias

<div id="refs" class="references">

<div id="ref-anderson2010geomorphology">

Anderson, R. S., & Anderson, S. P. (2010). *Geomorphology: The mechanics
and chemistry of landscapes*. Cambridge University Press.

</div>

<div id="ref-bivand2008applied">

Bivand, R. S., Pebesma, E. J., & Gomez-Rubio, V. (2008). *Applied
spatial data analysis with R* (Vol. 747248717). Springer.

</div>

<div id="ref-fischer2009handbook">

Fischer, M. M., & Getis, A. (2009). *Handbook of applied spatial
analysis: Software tools, methods and applications*. Springer Science &
Business Media.

</div>

<div id="ref-gutierrez2008geomorfologia">

Gutiérrez Elorza, M. (2008). *Geomorfologı'a*.

</div>

<div id="ref-hengl2009practical">

Hengl, T. (2009). *A practical guide to geostatistical mapping*.

</div>

<div id="ref-loonis2018handbook">

Loonis, V., & Bellefon, M.-P. de. (2018). *Handbook of spatial
analysis*.

</div>

<div id="ref-lovelace2019geocomputation">

Lovelace, R., Nowosad, J., & Muenchow, J. (2019). *Geocomputation with
R*. Retrieved from <https://geocompr.robinlovelace.net/>

</div>

<div id="ref-mas2013analisis">

Mas, J.-F. (2013). *Análisis espacial con R. Usa R como un sistema de
información geográfica*. European Scientific Institue (ESI).

</div>

<div id="ref-olaya2014sistemas">

Olaya, V. (2014). *Sistemas de informacion geográfica*. Retrieved from
<https://volaya.github.io/libro-sig/>

</div>

<div id="ref-tricart1956geomorphologie">

Tricart, J. (1956). *La géomorphologie et la pensée marxiste*. La
Pensée.

</div>

</div>