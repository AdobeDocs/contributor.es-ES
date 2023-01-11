---
lastModified: 2018-06-28T00:00:00Z
title: Creación de guías de estilo para colaboradores externos
description: Obtenga información sobre la creación y las directrices editoriales para colaboradores externos para Experience League.
exl-id: 874f88d7-18ad-4ac8-bfa3-737255652bbc
source-git-commit: 03d46c9ffb664824f9526f781d776069d486f271
workflow-type: ht
source-wordcount: '2227'
ht-degree: 100%

---

# Creación de guías de estilo para colaboradores externos {#guidelines}

Esta página proporciona directrices editoriales para autores externos que crean contenido o actualizan contenido existente en Experience League. Antes de empezar, asegúrese de lo siguiente:

* Familiarícese con la creación de [Markdown](markdown.md) 
* Compruebe la ortografía y la gramática de sus artículos
* Utilice un tono cordial, una presentación coherente y frases sencillas para mejorar la traducción automática.
* Seguir [prácticas recomendadas](#writing-tips) y los estándares editoriales en esta página

## Directrices de estilo {#style-guidelines}

Tenga en cuenta lo siguiente al escribir documentación.

* **Escriba de forma concisa**: no malgaste palabras. Utilice frases cortas y concisas. Mantenga el artículo centrado. Utilice un número mínimo de notas.
* **Céntrese en la audiencia y el fin**: antes de comenzar a escribir, determine claramente quién es el cliente y qué tarea intenta llevar a cabo. Escriba el artículo para ayudar a ese cliente a realizar esa tarea.
* **Utilice ejemplos**: ponga ejemplos para explicar los conceptos.
* **Organice el contenido**: cree secciones para dividir las instrucciones en grupos de pasos más manejables. Utilice una captura de pantalla para aclarar cuestiones.

## Prácticas recomendadas para la escritura técnica {#writing-tips}

La escritura técnica, especialmente para la documentación de software, es una industria especializada. Incluso el novelista más prolífico se entusiasma cuando intenta escribir técnicas, no porque el material sea complejo o técnico, sino porque no es fácil hacer información técnica compleja _simple_. Para tener éxito, el contenido debe ser estructuralmente coherente, analizable, reutilizable y fluir por la canalización de publicación sin errores de estructura y sintaxis.

Las secciones siguientes describen problemas comunes que los nuevos escritores deben tener en cuenta lo siguiente:

### Encabezados no separados por texto (encabezados dobles) {#double-headings}

Si tiene dos encabezados sin texto que los separe, agregue el texto que falta (para introducir el segundo encabezado del tema). O bien, puede quitar uno de los encabezados. La segunda es probablemente innecesaria.

Por ejemplo, _Información general_ no sirve de nada:

![Encabezados dobles](assets/headings-double.png)

* Además, si el segundo encabezado resulta ser _Información general_, probablemente sea innecesario. Su H1 y el primer párrafo sirven como información general conceptual sobre el tema del artículo.

* Del mismo modo, para fines de la optimización de los motores de búsqueda (SEO), los encabezamientos independientes como _Información general_ e _Introducción_ no son útiles por sí mismos. Asigne un nombre al producto o la función que está presentando. (Por ejemplo: _información general de los de informes de visitas en orden previsto_)

### Encabezados de referencia cruzados incoherentes {#maps}

Use encabezados de _Más información_ para las listas de referencias cruzadas (o mapas). Por ejemplo:

![Lista de referencias cruzadas](assets/headings-more-info.png)

**Directrices para las listas de referencias cruzadas**

* Usar una lista con viñetas para las referencias cruzadas
* Utilice cursiva para los nombres formales de las guías o los nombres de página (cuando no utilice textos de vínculos)
* No escriba guiones en el encabezado (ni en ningún encabezado)
* Evitar números en encabezados

### Falta de coincidencia entre la entrada del índice, la ruta de exploración y el nombre de la página. {#toc}

Debido a que administramos manualmente el archivo del índice (tabla de contenido), estas discrepancias son fáciles de cometer. Asegúrese de que su entrada de índice coincida con el nombre de su página (H1). Además, asegúrese de que coincida estrechamente con la ruta de exploración.

**Orientación sobre el índice y las listas**

* Es posible que tenga que acortar la entrada del índice, pero debe estar claramente relacionado con el nombre de página y la ruta de exploración.
* Las rutas de exploración se extraen de los metadatos del título, por lo que pueden diferir (con fines de la SEO).

### Comillas en lugar de cursivas {#quotes}

Es difícil resistirse a agregar comillas alrededor de una palabra o frase. Sin embargo, las comillas están pensadas para citar un discurso y casi nunca se utilizan en la documentación del producto.

**Directrices sobre las comillas**

* Normalmente, la cursiva funciona mejor que las comillas (para mensajes de error, palabras únicas o extranjeras, etc.).
* Para los elementos de la interfaz, utilice negrita y UICONTROL.

### Procedimientos {#steps}

La redacción de un procedimiento (el tipo de contenido de la _tarea_) no es un talento con el que nacemos. La creación de un procedimiento legible y claro lleva práctica.

**Directrices para los pasos**

* Un procedimiento es una serie de pasos. Un paso es breve, numerado, un comando de una _sola oración_.
* Empiece cada paso con un verbo o con el infinitivo _Para_ (para orientar al lector hacia el objetivo, como en, _Para permanecer conectado, habilite **Permanecer conectado**_). Si un paso tiene un objetivo específico dentro del procedimiento general, mencione el objetivo antes de la acción.
* Si tiene información sobre el paso (un tipo de contenido llamado _información del paso_), añádalo después del paso (con sangría en el paso) o después del recurso (una captura de pantalla, un vídeo o una lista de descripciones de la interfaz).
* Si el paso tiene dos acciones (por ejemplo, _Seleccione esto y luego_), escríbalo como una sola frase breve.
* Limite la tarea entre siete y diez pasos. Si va a crear más de diez pasos en una tarea, es probable que tenga que dividirla en dos tareas. Use su mejor criterio aquí.
* En la documentación del producto, no utilice encabezados como pasos. (La excepción para tutoriales se detalla a continuación).
* Para tutoriales de varias páginas, se pueden permitir encabezados como pasos. Sin embargo, no los numere. En su lugar, escriba _Paso 1:_, _Paso 2:_, etc.

**Procedimiento de ejemplo**

Este es un procedimiento bien estructurado para iniciar sesión en Adobe:

Para iniciar sesión en Adobe, haga lo siguiente:

1. En `Adobe.com`, seleccione **Experience Cloud**.
1. Seleccione **Inicio de sesión**.
1. Seleccione **Cuenta personal**.
1. Para mantener la sesión iniciada, seleccione **Permanecer conectado**.
1. Escriba su nombre y contraseña.
1. Seleccione **Inicio de sesión**.

### Listas paralelas {#lists}

El uso de la construcción paralela de listas facilita la lectura y la búsqueda. Las listas incluyen un índice (tabla de contenido), listas con viñetas (sin ordenar) o listas numeradas.

Ejemplo de índice con entradas paralelas:

![Índice paralelo](assets/parallel-toc.png)

El índice anterior es un buen ejemplo porque:

* Las entradas principales sobre conceptos son sustantivos o frases sustantivadas
* Los procedimientos (tareas) son verbos activos (no gerundios)
* Todas las entradas utilizan mayúsculas de las frases

## Metadatos de títulos y descripciones {#metadata}

Los metadatos de los _Títulos_ y las _descripciones_ son importantes para la optimización de los motores de búsqueda, la detección de contenido y las puntuaciones de calidad de contenido en Experience League.

Aquí hay ejemplos de títulos y descripciones:

**Descripciones de los artículos de conceptos**

* _Obtenga información sobre los segmentos en Adobe Analytics. Obtenga ayuda sobre la configuración del panel Segmentación en un espacio de trabajo._
* _Busque ayuda sobre el uso de segmentos en un informe de vistas de página en Adobe Analytics._

**Descripciones de los artículos de procedimientos/tareas**

* _Aprenda a crear un segmento en Adobe Analytics._
* _Cree un segmento en Adobe Analytics. Obtenga información sobre cómo seleccionar, configurar y ejecutar un informe en función del segmento que cree._

El que utilice depende del tamaño y el alcance del artículo.

**Título para un artículo de concepto**

* _Segmentos en informes de vistas de página_

**Título para un artículo de procedimiento/tarea**

* _Creación de un segmento para un informe de vistas de página_

(Recuerde que la barra vertical y el nombre del producto se añaden automáticamente a los títulos).

## Formas de mejorar la claridad (y puntuaciones de Acrolinx) {#tips}

A continuación se indican formas sencillas de mejorar el diseño, la claridad y la legibilidad del contenido. También ayudan a mejorar las puntuaciones de estilo Acrolinx y las puntuaciones de CQI en ExL.

| Guía | Acerca de  |
|---|---|
| Utilizar la voz activa | Cambiar la voz pasiva a la activa |
| Utilizar el tiempo presente | **Débil:** *la versión 8 de Campaign se lanzará en junio.* <p>**Fuerte:** *la versión 8 de Campaign se lanza en junio.*<p>El tiempo presente siempre es más fácil de leer para los clientes. |
| Evite los adverbios débiles e innecesarios | *Muy*, *extremadamente*, *increíblemente*.... <p>Los adverbios son palabras adicionales que no agregan significado significativo si utiliza oraciones con verbos y adjetivos fuertes y precisos. |
| Use verbos fuertes para los títulos y las [entradas del índice](#using-toc) | Ejemplos:<p>**Débil:** *Creación y administración de características* <p>**Fuerte:** *Crear y administrar características* |
| Usar [mayúsculas](https://docs.microsoft.com/es-es/style-guide/capitalization) en la oración | Cuando haya dudas, no use mayúsculas. En los títulos, utilice mayúsculas como en una oración. Ponga en mayúsculas los sustantivos propios y la primera palabra después de dos puntos. En los procedimientos, utilice mayúsculas y minúsculas para las coincidencias que se ven en la interfaz. |
| Conozca estos pequeños consejos para una mayor claridad | <ul><li>Evite la frase *Con el finde de* (no aporta significado). Todo lo que necesita es *Para*.</li><li>Evite la palabra *Utilizar.* Puede sonar más técnica, pero no la es. *Utilizar* significa *hacer un buen uso, especialmente de algo que no estaba destinado a este fin, pero que servirá para eso*.</li><li>Evite los punto y coma: use un punto en su lugar y comience una nueva oración. Los punto y coma plantean una complejidad innecesaria.</li><li>Dos puntos: utilice dos puntos para presentar una lista. Utilice dos puntos con moderación dentro de las frases. Ponga en mayúscula la primera palabra después de dos puntos en una frase.</li><li>Utilice la coma de Oxford (tres comas en una lista).</li><li>Mantenga la longitud de la oración por debajo de 39 palabras.</li><li>Navegación: use _Vaya a_ o _Navegue a_.</li><li>Evite el texto URL sin formato (utilice un texto de vínculo fácil de usar) a menos que mostrar la ruta sea información importante.</li></ul> |
| Uso de un corrector ortográfico en VSC | Instale el corrector ortográfico de código (extensión) en Visual Studio Code. |
| Cambie _hacer clic_ por _ir a_ o _seleccionar_. | _Hacer clic_ es una palabra específica del dispositivo (con problemas de accesibilidad) y la tendencia es no usarla. A continuación se ofrecen sugerencias para cambiarla:<ul><li>Navegación: _Vaya al Archivo > Imprimir_.</li><li>Haga clic en: _Seleccionar Archivo > Imprimir_ o _Seleccionar OK_. </li></ul>Consulte [Descripción de las interacciones con la interfaz de usuario](https://docs.microsoft.com/es-es/style-guide/procedures-instructions/describing-interactions-with-ui) para obtener más ideas sobre la mejor opción de palabras en diversas situaciones. |
| Ejecutar Acrolinx en VSC | Acrolinx comprueba los problemas de estilo y gramática. Comprueba las direcciones URL, la terminología, la ortografía, etc. Le ayuda a mejorar su claridad y la traducción del contenido de Experience League. |

{style=&quot;table-layout:auto&quot;}

Más prácticas recomendadas y recursos:

* [Contenido que se puede escanear](https://docs.microsoft.com/es-es/style-guide/scannable-content/): ayude a los lectores a encontrar lo que necesitan rápidamente, o reconozcan rápido cuando no están donde necesitan estar. Escribir para facilitar el escaneo puede ayudar.
* **Números:** en el texto independiente, escriba números enteros entre cero y nueve y utilice números para 10 o más. Consulte [Números](https://docs.microsoft.com/es-es/style-guide/numbers).
* Escriba como habla, con simpatía y establezca rápidamente el punto.

Consulte [Los diez consejos principales para la redacción](https://docs.microsoft.com/es-es/style-guide/top-10-tips-style-voice) en la [Guía de estilo de Microsoft®](https://docs.microsoft.com/es-es/style-guide/welcome/) para obtener más información.

## Texto alternativo {#alt-text}

Agregue texto alternativo significativo a sus recursos (imágenes). Considere el texto alternativo que coincida con lo siguiente:

* El objetivo que los clientes pueden lograr (nombre de tarea o concepto)
* La función o página que está mostrando
* El nombre del icono que está mostrando

Google considera el texto alternativo en los resultados de la SEO.

## Localización: DNL y UICONTROL {#localization}

No es necesario preocuparse por si el producto está localizado o por los idiomas que utiliza ExL. Sin embargo, puede mejorar la calidad de la localización mediante la aplicación de las dos etiquetas de Markdown siguientes (obligatorias) cuando corresponda:

* `DNL`

   DNL significa _no localizar_. Usted lo utiliza solo para nombres de productos de Adobe de marca comercial, todos los cuales deben permanecer en inglés.

   Ejemplos de sintaxis: `[!DNL Adobe Campaign]` o `[!DNL Workfront]`

   DNL no aplica para nombres de archivo ni para las URL.

* `UICONTROL`

   UICONTROL indica un control de interfaz (como una opción, campo, pestaña, página, grupo de opciones o nombre de función en la interfaz de usuario).

   Ejemplo de sintaxis: `Select **[!UICONTROL Project]**, then select **[!UICONTROL Save]**.`

>[!IMPORTANT]
>
>Debe aplicar estas etiquetas antes de localizar el contenido.

### Uso de Adobe en nombres de productos {#product-names}

Para la identidad corporativa, normalmente incluimos _Adobe_ en la primera referencia de un producto en cuanto a la guía. En función del espacio, puede colocar Adobe en un encabezado, pero la primera referencia de la copia de cuerpo debe incluir el nombre completo. Algunos productos, como _Adobe Audition_ y _Adobe Premiere Pro_, requieren el uso de Adobe en la referencia primera o en la más destacada en cada parte de la documentación y el material adjunto, ya que forma parte del nombre legal de la marca comercial.

## Primeros párrafos {#firstparas}

El primer párrafo debe definir el tema y describir lo que el lector aprende al leer el artículo.

Primer párrafo de muestra (concepto):

_Las audiencias son recopilaciones de visitantes (una lista de ID de visitantes). Los servicios de audiencia de Adobe administran la traducción de datos sobre visitantes en segmentación de audiencia. De este modo, la creación y gestión de audiencias es similar a la creación y uso de segmentos, con la capacidad añadida de compartir segmentos de audiencia en Experience Cloud._

Primer párrafo de muestra (tarea):

_Crear un origen de atributos del cliente (archivos CSV y FIN) y cargar los datos. Puede activar el origen de los datos cuando esté preparado. Una vez que esté listo el origen de los datos, comparta los datos del atributo con Analytics y Target._

### Sugerencias de SEO para los primeros párrafos {#seo}

* Incluya términos de búsqueda en los primeros párrafos.
* Use términos que utilicen los lectores.
* Incluya sinónimos y, si es necesario, uso previo de los términos. Por ejemplo, “El servicio Experience Cloud ID (ECID), anteriormente conocido como _ID de visitante_ o como acrónimos como MID, MCVID, proporciona un ID universal y persistente que identifica a los visitantes”.
* Incluya términos SEO en los vínculos.
* Evite colocar términos esenciales en tablas complejas. Las tablas complejas no arrojan resultados de búsqueda fiables. El texto de las imágenes no se puede buscar. Se buscan los subtítulos.

## Uso de mayúsculas {#capitalization}

* El estilo de Adobe utiliza mayúsculas como en una oración para todos los títulos, encabezados, subtítulos y elementos de navegación de la página.
* Todas las palabras están en minúsculas, excepto la primera palabra y los sustantivos propios, como los nombres de marcas, soluciones y servicios.
* Se colocan las mayúsculas en los nombres de los productos de herramientas, opciones, elementos de menú, cuadros de diálogo y campos.

## Índice {#using-toc}

El `TOC.md` es su índice. Cada guía debe tener uno.

**Guía editorial para un índice**

* Uso de mayúsculas y minúsculas: utilice siempre mayúsculas y minúsculas en todas las entradas (sin incluir los acrónimos). Ponga mayúsculas únicamente en los nombres de productos formales o los elementos de la interfaz (páginas, pestañas, campos, opciones, etc.). Coincida con la IU al hacer referencia a ella.
* Forma verbal y paralelismo: utilice el verbo imperativo y evite los gerundios. Los índices son listas, por lo que siempre intente mantener las listas de forma paralela la mayor parte del tiempo. Hay excepciones que a veces no se pueden evitar. Para las páginas conceptuales, utilice sustantivos y frases sustantivadas. Para las tareas, utilice verbos.

**Guía de sintaxis**

* Un encabezado de sección (principal) del índice no puede ser un vínculo; no tiene una página con contenido. Debe contener un anclaje como `{#processing-rules}`.
* Debe utilizar la sintaxis adecuada para los encabezados de sección del índice (por ejemplo, `+ Processing rules {#processing-rules}`) y vínculos a artículos del índice (por ejemplo, `+ [Article name](article.md)`).
* Las entradas del artículo del índice pueden ser una versión abreviada del título del artículo. Siga los estándares para escribir descripciones generales, conceptos y tareas en este documento.
* Evite añadir el mismo archivo varias veces a un índice (o a varios). Hacerlo causa un comportamiento extraño.
* Si el repositorio contiene varias guías del usuario, los directorios de las guías del usuario deben estar en el mismo nivel, como los subdirectorios dentro de la variable directorio `help`. Cada directorio de guía del usuario debe tener un archivo con índice. No anidar guías de usuario.

## Negrita y cursiva {#bold}

* Utilice texto en negrita solo para los elementos de interfaz en los que haga clic en un procedimiento (y con UICONTROL).
* Utilice cursiva para dar énfasis o cuando una palabra sea confusa. Por ejemplo, una palabra extranjera, o cuando se describe una palabra o se define un término.
