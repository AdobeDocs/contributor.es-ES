---
lastModified: 2018-06-28T00:00:00Z
title: Creación de guías de estilo para colaboradores externos
description: Obtenga información sobre la creación y las directrices editoriales para colaboradores externos para Experience League.
exl-id: 874f88d7-18ad-4ac8-bfa3-737255652bbc
source-git-commit: 03d46c9ffb664824f9526f781d776069d486f271
workflow-type: tm+mt
source-wordcount: '2227'
ht-degree: 8%

---

# Creación de guías de estilo para colaboradores externos{#guidelines}

Esta página proporciona directrices editoriales para autores externos que crean contenido o actualizan contenido existente en el Experience League. Antes de empezar, asegúrese de que:

* Familiarícese con [Markdown](markdown.md) creación
* Compruebe la ortografía y la gramática de sus artículos
* Utilice un tono cordial, una presentación coherente y frases sencillas para mejorar la traducción automática
* Seguir [prácticas recomendadas](#writing-tips) y los estándares editoriales en esta página

## Directrices de estilo{#style-guidelines}

Tenga en cuenta lo siguiente al escribir documentación.

* **Escriba de forma concisa**: no malgaste palabras. Utilice frases cortas y concisas. Mantenga el artículo centrado. Utilice un número mínimo de notas.
* **Céntrese en la audiencia y el fin**: antes de comenzar a escribir, determine claramente quién es el cliente y qué tarea intenta llevar a cabo. Escriba el artículo para ayudar a ese cliente a realizar esa tarea.
* **Utilice ejemplos**: ponga ejemplos para explicar los conceptos.
* **Organice el contenido**: cree secciones para dividir las instrucciones en grupos de pasos más manejables. Utilice una captura de pantalla para aclarar cuestiones.

## Prácticas recomendadas de escritura técnica{#writing-tips}

La escritura técnica, especialmente para la documentación de software, es una industria especializada. Incluso el novelista más prolífico se entusiasma cuando intenta escribir técnicas, no porque el material sea complejo o técnico, sino porque no es fácil hacer información técnica compleja _simple_. Para tener éxito, el contenido debe ser estructuralmente coherente, analizable, reutilizable y fluir por la canalización de publicación sin errores de estructura y sintaxis.

Las secciones siguientes describen problemas comunes que los nuevos escritores deben tener en cuenta:

### Encabezados no separados por texto (encabezados dobles){#double-headings}

Si tiene dos encabezados sin texto que los separe, agregue el texto que falta (para introducir el segundo encabezado del tema). O bien, puede quitar uno de los encabezados. La segunda es probablemente innecesaria.

Por ejemplo, _Información general_ no sirve de nada:

![Encabezados dobles](assets/headings-double.png)

* Además, si el segundo encabezado resulta ser _Información general_, probablemente sea innecesario. Su H1 y el primer párrafo sirven como información general conceptual sobre el tema del artículo.

* Del mismo modo, para fines de SEO, los encabezamientos independientes como _Información general_ y _Introducción_ no son útiles por sí mismos. Asigne un nombre al producto o la función que está introduciendo. (Ejemplo: _Resumen de informes de visitas en el orden previsto_)

### Encabezados de referencia cruzados incoherentes{#maps}

Uso _Más información_ encabezados para listas de referencias cruzadas (o mapas). Ejemplo:

![Lista de referencias cruzadas](assets/headings-more-info.png)

**Directrices para listas de referencias cruzadas**

* Usar una lista con viñetas para las referencias cruzadas
* Utilice cursiva para los nombres formales de las guías o los nombres de página (cuando no utilice texto de vínculo)
* No escriba guiones en el encabezado (ni en ningún encabezado)
* Evitar números en encabezados

### Coincidencia errónea de entrada de TDC, ruta de exploración y nombre de página{#toc}

Debido a que administramos manualmente el archivo TOC (tabla de contenido), estas discrepancias son errores fáciles. Asegúrese de que la entrada de TDC coincide con el nombre de su página (H1). Además, asegúrese de que coincida estrechamente con la ruta de exploración.

**Directrices sobre tablas de contenido y listas**

* Es posible que tenga que acortar la entrada de TDC, pero debe estar claramente relacionado con el nombre de página y la ruta de exploración.
* Las rutas de exploración se extraen de los metadatos del título, por lo que pueden diferir (con fines de SEO).

### Comillas en lugar de cursiva{#quotes}

Es difícil resistirse a agregar comillas alrededor de una palabra o frase. Sin embargo, las comillas están pensadas para citar un discurso y casi nunca se utilizan en la documentación del producto.

**Directrices sobre las comillas**

* Normalmente, la cursiva funciona mejor que las comillas (para mensajes de error, palabras únicas o extranjeras, etc.).
* Para los elementos de la interfaz, utilice negrita y UICONTROL.

### Procedimientos{#steps}

Escritura de un procedimiento (el _tarea_ tipo de contenido) no es un talento con el que nacemos. La creación de un procedimiento legible y claro lleva a la práctica.

**Directrices para los pasos**

* Un procedimiento es una serie de pasos. Un paso es breve, numerado, _una sola oración_ comando.
* Empiece cada paso con un verbo o con el _Hasta_ infinitivo (para orientar al lector hacia el objetivo, como en, _Para permanecer conectado, habilite **Permanecer conectado**_). Si un paso tiene un objetivo específico dentro del procedimiento general, mencione el objetivo antes de la acción.
* Si tiene información sobre el paso (un tipo de contenido llamado _información del paso_, añádalo después del paso (con sangría en el paso ) o después del recurso (una captura de pantalla, un vídeo o una lista de descripciones de la interfaz).
* Si el paso tiene dos acciones (por ejemplo, _Seleccione esto y luego que_), escribirlo como una sola frase breve.
* Limite la tarea a entre siete y diez pasos. Si va a crear más de diez pasos en una tarea, es probable que tenga que dividirla en dos tareas. Use su mejor criterio aquí.
* En la documentación del producto, no utilice encabezados como pasos. (Excepción a continuación para tutoriales).
* Para tutoriales de varias páginas, se pueden permitir encabezados como pasos. Sin embargo, no los numere. En su lugar, escriba _Paso 1:_, _Paso 2:_, etc.

**Procedimiento de ejemplo**

Este es un procedimiento bien estructurado para iniciar sesión en el Adobe:

Para iniciar sesión en el Adobe:

1. Activado `Adobe.com`, seleccione **Experience Cloud**.
1. Select **Inicio de sesión**.
1. Select **Cuenta personal**.
1. Para mantener la sesión iniciada, seleccione **Permanecer registrado**.
1. Escriba su nombre y contraseña.
1. Select **Inicio de sesión**.

### Listas paralelas{#lists}

El uso de la construcción paralela para listas facilita la lectura y el escaneo. Las listas incluyen una tabla de contenido (tabla de contenido), listas con viñetas (sin ordenar) o listas numeradas.

Ejemplo de tabla de contenido con entradas paralelas:

![TDC paralelo](assets/parallel-toc.png)

La tabla de contenido anterior es un buen ejemplo porque:

* Las entradas principales conceptuales son sustantivos o frases noun
* Los procedimientos (tareas) son verbos activos (no gerunds)
* Todas las entradas utilizan mayúsculas de las frases

## Metadatos de título y descripción{#metadata}

_Título_ y _descripción_ los metadatos son importantes para SEO, la detección de contenido y las puntuaciones de calidad de contenido en el Experience League.

Aquí hay ejemplos de títulos y descripciones:

**Descripciones de los artículos de concepto**

* _Obtenga información sobre los segmentos en Adobe Analytics. Obtenga ayuda sobre la configuración del panel Segmentación en un espacio de trabajo._
* _Busque ayuda sobre el uso de segmentos en un informe de vistas de página en Adobe Analytics._

**Descripciones de los artículos de procedimientos/tareas**

* _Obtenga información sobre cómo crear un segmento en Adobe Analytics._
* _Cree un segmento en Adobe Analytics. Obtenga información sobre cómo seleccionar, configurar y ejecutar un informe en función del segmento que cree._

El que utilice depende del tamaño y el alcance del artículo.

**Título para un artículo de concepto**

* _Segmentos en informes de vistas de página_

**Título para un artículo de procedimiento/tarea**

* _Creación de un segmento para un informe de vistas de página_

(Recuerde que la barra vertical y el nombre del producto se añaden automáticamente a los títulos).

## Formas de mejorar la claridad (y puntuaciones de Acrolinx){#tips}

A continuación se indican formas sencillas de mejorar el diseño, la claridad y la legibilidad del contenido. También ayudan a mejorar las puntuaciones de estilo Acrolinx y las puntuaciones de CQI en ExL.

| Guía | Acerca de  |
|---|---|
| Utilizar voz activa | Cambiar voz pasiva a voz activa |
| Uso presente tenso | **Débil:** *Campaign v8 se lanzará en junio.* <p>**Fuerte:** *Versiones de Campaign v8 en junio.*<p>El tiempo presente siempre es más fácil de leer para los clientes. |
| Evite los anunciantes débiles e innecesarios | *Muy*, *extremadamente*, *increible*.... <p>Los anuncios son palabras adicionales que no agregan significado significativo si utiliza verbos, cláusulas y adjetivos fuertes y precisos. |
| Use verbos fuertes para títulos y [Entradas de TOC](#using-toc) | Ejemplos:<p>**Débil:** *Creación y administración de características* <p>**Fuerte:** *Crear y administrar características* |
| Usar frase [capitalización](https://docs.microsoft.com/en-us/style-guide/capitalization) | Cuando haya dudas, no capitalicen. En los encabezados, utilice mayúsculas y minúsculas. Ponga en mayúsculas los sustantivos adecuados y la primera palabra después de dos puntos. En los procedimientos, utilice mayúsculas y minúsculas para las coincidencias que se ven en la interfaz. |
| Conozca estos pequeños consejos para una mayor claridad | <ul><li>Evitar *Para* (no añade significado). Todo lo que necesitas es *a.*</li><li>Evitar *Utilice.* Puede sonar más técnico, pero no lo es. *Utilizar* significa *para hacer un buen uso de, especialmente de algo que no estaba destinado a este fin pero que servirá*.</li><li>Evite los punto y coma: Utilice un punto en su lugar y comience una nueva oración. Los punto y coma introducen complejidad innecesaria.</li><li>Dos puntos: Utilice dos puntos para introducir una lista. Utilice dos puntos con moderación dentro de las frases. Ponga en mayúscula la primera palabra después de dos puntos en una frase.</li><li>Utilice la coma de Oxford (tres comas en una lista).</li><li>Mantenga la longitud de la oración por debajo de 39 palabras.</li><li>Navegación: use _vaya a_ o _vaya a_.</li><li>Evite el texto sin procesar de la dirección URL (utilice texto de vínculo descriptivo) a menos que mostrar la ruta sea información importante.</li></ul> |
| Uso de un corrector ortográfico en VSC | Instale la revisión de ortografía de código (extensión) en el código de Visual Studio. |
| Cambiar _click_ a _vaya a_ o _select_ | _Haga clic en_ es una palabra específica del dispositivo (con problemas de accesibilidad) y la tendencia es alejarse de ella. A continuación se ofrecen sugerencias para cambiarlo:<ul><li>Navegación: _Vaya a Archivo > Imprimir_.</li><li>Haciendo clic en: _Seleccione Archivo > Imprimir_ o _Seleccione Aceptar_. </li></ul>Consulte [Descripción de las interacciones con la interfaz de usuario](https://docs.microsoft.com/en-us/style-guide/procedures-instructions/describing-interactions-with-ui) para obtener más ideas sobre la mejor opción de palabras en diversas situaciones. |
| Ejecutar Acrolinx en VSC | Acrolinx comprueba los problemas de estilo y gramática. Comprueba las direcciones URL, la terminología, la ortografía, etc. Le ayuda a mejorar su claridad y mejora la traducción del contenido del Experience League. |

{style=&quot;table-layout:auto&quot;}

Algunas prácticas recomendadas y recursos más:

* [Contenido escaneado](https://docs.microsoft.com/en-us/style-guide/scannable-content/): Ayude a los lectores a encontrar lo que necesitan rápidamente, o reconozcan tan rápido cuando no están donde necesitan estar. Escribir para facilitar el escaneo puede ayudar.
* **Números:** En el texto del cuerpo, escriba números enteros entre cero y nueve y utilice números para 10 o buenos. Consulte [Números](https://docs.microsoft.com/en-us/style-guide/numbers).
* Escriba como habla, proyecte la simpatía y llegue rápidamente al punto.

Consulte [Principales 10 consejos de escritura](https://docs.microsoft.com/en-us/style-guide/top-10-tips-style-voice) en el [Guía de estilo de Microsoft®](https://docs.microsoft.com/en-us/style-guide/welcome/) para obtener más información.

## Texto alternativo{#alt-text}

Agregue texto alternativo significativo a sus recursos (imágenes). Considere el texto alternativo que coincida:

* El objetivo que los clientes pueden lograr (nombre de tarea o concepto)
* La función o página que está mostrando
* El nombre del icono que está mostrando

Google considera el texto alternativo en los resultados de SEO.

## Localización: DNL y UICONTROL{#localization}

No es necesario preocuparse de si el producto está localizado o de los idiomas que utiliza ExL. Sin embargo, puede mejorar la calidad de la localización mediante la aplicación de las dos etiquetas Markdown siguientes (obligatorio) cuando corresponda:

* `DNL`

   DNL significa _no localizar_. Usted lo utiliza sólo para nombres de productos de Adobe de marca comercial, todos los cuales deben permanecer en inglés.

   Ejemplos de sintaxis: `[!DNL Adobe Campaign]` o `[!DNL Workfront]`

   DNL no está diseñado para nombres de archivo ni URL.

* `UICONTROL`

   UICONTROL indica un control de interfaz (como una opción, campo, ficha, página, grupo de opciones o nombre de función en la interfaz de usuario).

   Ejemplo de sintaxis: `Select **[!UICONTROL Project]**, then select **[!UICONTROL Save]**.`

>[!IMPORTANT]
>
>Debe aplicar estas etiquetas antes de localizar el contenido.

### Uso de Adobe en nombres de productos{#product-names}

Para la identidad corporativa, normalmente incluimos _Adobe_ en la primera referencia de un producto a nivel de guía. En función del espacio, puede soltar el Adobe en un encabezado, pero la primera referencia de la copia de cuerpo debe incluir el nombre completo. Algunos productos, como _Adobe Audition_ y _Adobe Premiere Pro_, requieren el uso de Adobes sobre la primera o más destacada referencia en cada parte de la garantía, ya que forma parte del nombre legal de la marca comercial.

## Primeros párrafos{#firstparas}

El primer párrafo debe definir el tema y describir lo que el lector aprende al leer el artículo.

Primer párrafo de muestra (concepto):

_Las audiencias son recopilaciones de visitantes (una lista de ID de visitantes). El servicio de audiencia de Adobe administra la traducción de datos del visitante en segmentación de audiencia. De este modo, la creación y gestión de audiencias es similar a la creación y uso de segmentos, con la capacidad añadida de compartir segmentos de audiencia en Experience Cloud._

Primer párrafo de muestra (tarea):

_Crear un origen de atributos del cliente (archivos CSV y FIN) y cargar los datos. Puede activar el origen de los datos cuando esté preparado. Una vez que esté listo el origen de los datos, comparta los datos del atributo con Analytics y Target._

### Sugerencias de SEO para primeros párrafos{#seo}

* Incluir términos de búsqueda en los primeros párrafos.
* Utilice términos que utilizan los lectores.
* Incluya sinónimos y, si es necesario, uso previo de los términos. Por ejemplo, &quot;El servicio de ID de Experience Cloud (ECID), anteriormente conocido como _ID de visitante_ o como acrónimos como MID, MCVID, proporciona un ID universal y persistente que identifica a los visitantes&quot;.
* Incluya términos SEO en los vínculos.
* Evite colocar términos esenciales en tablas complejas. Las tablas complejas no arrojan resultados de búsqueda fiables. El texto de las imágenes no se busca. Se buscan los subtítulos.

## Capitalización{#capitalization}

* El estilo de Adobe utiliza mayúsculas y minúsculas al estilo de frase para todos los títulos, encabezados, subencabezados y elementos de navegación de la página.
* Todas las palabras están en minúsculas, excepto la primera palabra y los nombres adecuados, como los nombres de marcas, soluciones y servicios.
* Haga coincidir las mayúsculas y minúsculas en los nombres de producto de las herramientas, las opciones, los elementos de menú, los cuadros de diálogo y los campos.

## Tabla de contenido{#using-toc}

La variable `TOC.md` es su tabla de contenido. Cada guía debe tener una.

**Guía editorial para una tabla de contenido**

* Capitalización: Utilice siempre mayúsculas y minúsculas para cada entrada (sin incluir acrónimos). Ponga en mayúsculas únicamente los nombres de productos formales o los elementos de la interfaz (páginas, pestañas, campos, opciones, etc.). Coincida con la IU al hacer referencia a ella.
* Forma verbal y paralelismo: Utilice el verbo imperativo y evite los gerundos. Las tablas de contenido son listas, por lo que siempre intente mantener las listas paralelas la mayor parte del tiempo. Hay excepciones que a veces no se pueden evitar. Para las páginas conceptuales, utilice sustantivos y frases noun. Para las tareas, utilice verbos.

**Guía de sintaxis**

* Un encabezado de sección (principal) de la tabla de contenido no puede ser un vínculo; no tiene una página con contenido. Debe contener un anclaje como `{#processing-rules}`.
* Debe utilizar la sintaxis adecuada para los encabezados de sección de TDC (por ejemplo, `+ Processing rules {#processing-rules}`) y vínculos a artículos de TDC (por ejemplo, `+ [Article name](article.md)`).
* Las entradas de artículos de la tabla de contenido pueden ser una versión abreviada del título del artículo. Siga los estándares para escribir descripciones generales, conceptos y tareas en este documento.
* Evite agregar el mismo archivo varias veces a una tabla de contenido (o a varias tablas de contenido). Hacerlo causa un comportamiento extraño.
* Si el repositorio contiene varias guías del usuario, los directorios de guías del usuario deben estar en el mismo nivel, como los subdirectorios dentro de la variable `help` directorio. Cada directorio de guía del usuario debe tener un archivo TOC. No anidar guías de usuario.

## Negrita y cursiva{#bold}

* Utilice texto en negrita solo para los elementos de interfaz en los que haga clic en un procedimiento (y con UICONTROL).
* Utilice cursiva para dar énfasis o cuando una palabra sea confusa sin ella. Por ejemplo, una palabra externa, o cuando se describe una palabra o se define un término.
