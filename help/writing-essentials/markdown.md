---
lastModified: 28-6-2018
title: Cómo utilizar Markdown para escribir documentación
seo-title: Cómo utilizar Markdown para escribir documentación de Adobe
description: En este artículo se proporcionan los conceptos básicos y la información de referencia del lenguaje Markdown utilizado para escribir artículos.
seo-description: En este artículo se proporcionan los conceptos básicos y la información de referencia del lenguaje Markdown utilizado para escribir artículos para la documentación de Adobe.
translation-type: ht
source-git-commit: e7382ef4aefc69c6b4e7d78b7f34eaf897596eaf

---


# Cómo utilizar Markdown para escribir documentación técnica

Los artículos técnicos de Adobe están escritos con un lenguaje de marcado ligero llamado [Markdown](https://daringfireball.net/projects/markdown/), que es fácil de leer y aprender.

Como el contenido Adobe Docs se almacena en GitHub, puede utilizar una versión de Markdown denominada [GitHub Flavored Markdown (GFM)](https://help.github.com/categories/writing-on-github/), que proporciona funcionalidad adicional para satisfacer necesidades comunes de aplicación de formato. Además, el Adobe Markdown ampliado proporciona varias formas que admiten determinadas funciones relacionadas con la ayuda, como notas, sugerencias y vídeos incrustados.

## Conceptos básicos de Markdown

### Encabezados

Para crear un encabezado, utilice el símbolo de almohadilla (#) al principio de una línea:

```
   # This is level 1 (article title)
   ## This is level 2
   ### This is level 3
   #### This is level 4
   ##### This is level 5
```

### Texto básico

En Markdown, un párrafo no requiere sintaxis especial.

Para aplicar **negrita** al texto, se escribe entre dos asteriscos. Para aplicar *cursiva* al texto, se escribe entre un solo asterisco:

```markdown
    This text is **bold**.
    This text is *italic*.
    This text is both ***bold and italic***.
```

<!--
To format superscript (H<sub>2</sub>O) and subscript (e=mc<sup>2</sup>) text:

```markdown
This is subscript H<sub>2</sub>O and superscript e=mc<sup>2</sup>.
```
-->

Para ignorar los caracteres de formato de Markdown, ponga \ antes del carácter:

```markdown
This is not \*italicized\* type.
```

### Listas numeradas y listas con viñetas

Para crear listas numeradas, empiece una línea con 1. o 1), pero no utilice ambos formatos dentro de la misma lista, puesto que se iniciará una nueva lista. No es necesario especificar los números. GitHub lo hace por usted.

```markdown
1. This is step 1.
1. This is the next step.
1. This is yet another step, the third.
```

Visualización:

1. Este es el paso 1.
1. Este es el paso siguiente.
1. Este es otro paso, el tercero.

<!-- markdownlint-disable MD037 -->
Para crear listas de viñetas, empiece una línea con \*, - o +, pero no mezcle los formatos dentro de la misma lista. (Si combina los formatos, como \* y \+, se inicia una lista nueva).
<!-- markdownlint-disable MD037 -->

```markdown
- First item in an unordered list.
- Another item.
- Here we go again.
```

Visualización:

- Primer elemento de una lista desordenada.
- Otro elemento.
- Y otro más.

También puede incrustar listas dentro de listas y añadir contenido entre elementos de la lista.

```markdown
1. Set up your table and code blocks.
1. Perform this step.

   ![screen](assets/no-localize/adobe_standard_logo.png)
1. Make sure that your table looks like this: 

    | Hello | World |
    |---|---|
    | How | are you? |  
1. This is the fourth step.

   >[!NOTE]
   >
   >This is note text.
1. Do another step.
```

Visualización:

1. Configure la tabla y los bloques de código.
1. Realice este paso.

   ![pantalla](assets/no-localize/adobe_standard_logo.png)
1. Asegúrese de que la tabla tenga este aspecto:

   | Hola | mundo |
   |---|---|
   | ¿Cómo | estás? |
1. Este es el cuarto paso.

   >[!NOTE]
   >
   >Este es el texto de la nota.
1. Realice otro paso.

### Tablas

Las tablas no forman parte de la especificación principal de Markdown, pero Adobe las admite en cierta medida. Markdown no admite listas de líneas múltiples en celdas. Lo mejor es evitar el uso de varias líneas en las tablas. Puede crear tablas utilizando la barra vertical (|) para definir columnas y filas. Los guiones crean el encabezado de cada columna, mientras que las barras verticales separan las columnas. Incluya una línea en blanco antes de la tabla para que se muestre correctamente.

```markdown
| Header | Another header | Yet another header |
|------------|:---------------:|-----------------------:|
| row 1 | centered column 2 | right-aligned column 3 |
| row 2 | row 2 column 2 | row 2 column 3 |
```

Visualización:

| Encabezado | Otro encabezado | Y otro encabezado |
|------------|:---------------:|-----------------------:|
| fila 1 | columna centrada 2 | columna alineada a la derecha 3 |
| fila 2 | fila 2 columna 2 | fila 2 columna 3 |

Las tablas sencillas funcionan correctamente en Markdown. Sin embargo, es difícil trabajar con tablas que incluyen varios párrafos o listas dentro de una celda. Para dicho contenido, recomendamos utilizar un formato diferente, como encabezados y texto.

Para obtener más información sobre cómo crear tablas, consulte:

- [Organización de información con tablas de GitHub](https://help.github.com/articles/organizing-information-with-tables/)
- Aplicación web [Markdown Tables Generator](https://www.tablesgenerator.com/markdown_tables)
- [Conversión de tablas HTML a Markdown](https://jmalarcon.github.io/markdowntables/)

### Vínculos

La sintaxis Markdown para un vínculo en línea consiste en la parte `[link text]`, que es el texto que se va a hipervincular, seguido de la parte `(file-name.md)`, que es la URL o el nombre de archivo al que se va a vincular:

`[link text](file-name.md)`

```markdown
[Adobe](https://www.adobe.com) or <https://www.adobe.com>
```

Visualización:

[Adobe](https://www.adobe.com) o <https://www.adobe.com>

Para vínculos a artículos (referencias cruzadas) dentro del repositorio, utilice vínculos relativos. Puede utilizar todos los operandos de vínculos relativos, como ./ (directorio actual), ../ (atrás un directorio) y ../../ (atrás dos directorios).

```markdown
See [Overview example article](../../overview.md)
```

Para obtener más información sobre la vinculación, consulte el artículo [Vínculos](linking.md) de esta guía sobre las sintaxis de los vínculos.

### Imágenes

```markdown
![Adobe Logo](assets/no-localize/adobe_standard_logo.png "Hover text")
```

Visualización:

![Logotipo de Adobe](assets/no-localize/adobe_standard_logo.png "Texto sobre el que se puede colocar el ratón")

### Bloques de código

Markdown admite la colocación de bloques de código tanto en línea como en un bloque &quot;delimitado&quot; independiente entre frases. Para obtener más información, consulte [Compatibilidad nativa de Markdown para bloques de código (en inglés).](https://daringfireball.net/projects/markdown/syntax#precode)

Utilice una comilla invertida (\`) para crear estilos de código en línea dentro de un párrafo. Para crear un bloque de código multilínea específico, agregue tres comillas invertidas (\`\`\`) antes y después del bloque de código (denominado &quot;bloque de código delimitado&quot; en Markdown y &quot;componente de bloque de código&quot; en AEM). Para bloques de código delimitado, agregue el lenguaje del código después del primer conjunto de comillas invertidas para que Markdown resalte correctamente la sintaxis del código. Ejemplo: \`\`\` javascript

Ejemplos:

```markdown
This is `inline code` within a paragraph of text.
```

Visualización:

Esto es `inline code` dentro de un párrafo de texto.

Este es un bloque de código delimitado:

```markdown
\```javascript
function test() {
 console.log("notice the blank line before this function?");
\```
```

Visualización:

```javascript
function test() {
 console.log("notice the blank line before this function?");
```

Puede especificar propiedades para los bloques de código a fin de desactivar los números de línea (activado de forma predeterminada) o agregar un ajuste de línea (desactivado de forma predeterminada). Utilice {line-numbers=&quot;no&quot;} y {line-wrap=&quot;yes&quot;}. Estas propiedades son extensiones personalizadas de Markdown.

\`\`\`javascript {line-numbers=&quot;no&quot;}
function test() {
console.log(&quot;¿se ha fijado en la línea en blanco que hay antes de esta función?&quot;);
\`\`\`

### Listas de definición

Una lista de definiciones es una extensión de Markdown que admite el componente Lista de definición en AEM. Una lista de definición consiste en un término y su definición.

<!--

```markdown
Frog
: An amphibious green creature. Likes flies.

Cat
: A less amphibious creature than frogs.
```

Displayed:

Frog
: An amphibious green creature. Likes flies.

Cat
: A less amphibious creature than frogs.
--->

#### Observaciones y comentarios

Los comentarios (observaciones) no aparecen en los artículos de ayuda públicos. Sin embargo, los comentarios aparecen en los archivos públicos de Markdown que los usuarios pueden ver y editar.

## Extensiones de Markdown personalizadas

En los artículos de Adobe se utiliza la puntuación estándar para la mayoría de los formatos de artículo, como párrafos, vínculos, listas y encabezados. Para obtener un formato enriquecido, los artículos pueden utilizar funciones ampliadas de Markdown, como:

- Bloques de notas
- Vídeos incrustados
- No localizar
- Propiedades del componente, como asignar un ID de encabezado diferente a un encabezado

Utilice el símbolo de citas de bloque de Markdown (&gt;) al principio de cada línea para enlazar un componente ampliado, como una nota. Si necesita utilizar subcomponentes dentro de componentes, agregue un nivel adicional de citas de bloque (&gt;  &gt;) para esa sección de subcomponentes. Por ejemplo, una NOTA dentro de una sección DONOTLOCALIZE debe comenzar por &gt;    &gt;.

Algunos elementos comunes de Markdown, como encabezados y bloques de código, incluyen propiedades ampliadas. Si necesita cambiar las propiedades predeterminadas, agregue los parámetros entre llaves /{ /} después del componente. Las propiedades ampliadas se describen en contexto.

### Bloques de notas

Puede elegir entre cuatro tipos de bloques de notas para llamar la atención sobre un contenido específico:

- `[!NOTE]`
- `[!CAUTION]`
- `[!TIP]`
- `[!IMPORTANT]`

En general, los bloques de notas deben usarse con moderación porque pueden resultar molestos. Aunque también se admiten bloques de código, imágenes, listas y vínculos, intente que los bloques de notas sean simples y directos.


```markdown
>[!NOTE]
>This is a standard NOTE block.
```

Visualización:

>[!NOTE]
>Este es un bloque NOTE estándar.

```markdown
>[!TIP]
>This is a standard tip.
```

Visualización:

>[!TIP]
>Esta es una sugerencia estándar.

### Vídeos

Los vídeos incrustados no se representan de forma nativa en Markdown, pero puede utilizar esta extensión de Markdown.

```markdown
>[!VIDEO](https://www.youtube.com/watch?v=A0EcD2AxvJE)
```

Visualización:

>[!VIDEO](https://www.youtube.com/watch?v=A0EcD2AxvJE)

### Más como esto

El componente &quot;Más como esto&quot; de AEM aparece al final de un artículo. Muestra vínculos relacionados. Cuando se representa el artículo, se le puede dar el mismo formato que a los encabezados de nivel 2 (##) sin que se agreguen al mini-TOC.

<!--
```markdown
>[!MORE]
>* [Article 1](https://helpx.adobe.com/support/analytics.html)
>* [Article 2](https://helpx.adobe.com/support/audience-manager.html){target="new-window"}
```

Displayed:

>[!MORE]
>* [Article 1](https://helpx.adobe.com/support/analytics.html)
>* [Article 2](https://helpx.adobe.com/support/audience-manager.html){target="new-window"}
-->

### DNL (no localizar) y UICONTROL

En algunos casos, es necesario marcar ciertas secciones del contenido de un artículo para que solo estén en inglés.
Es necesario declarar palabras, frases y otros elementos en nuestros sistemas de traducción, lo que crea la capacidad para gestionar léxico controlado.

Para palabras o frases que no deban localizarse, utilice la extensión `[!DNL]` para ajustar la palabra o sección.

Para los elementos de la interfaz de usuario y los menús de una solución, se utiliza la extensión ``.

**Ejemplo:**

En [!DNL Adobe Target] puede crear pruebas directamente en una página habilitada para [!DNL Target].

**Fuente:**

```markdown
In [!DNL Adobe Target] you can create your tests directly on a [!DNL Target]-enabled page.
```

**Ejemplo**

Use el [!UICONTROL Visual Experience Composer] en [!DNL Target] para crear la prueba directamente en una página.

**Fuente:**

```markdown
Use the [!UICONTROL Visual Experience Composer] in [!DNL Target] to create your test directly on a page.
```

## Problemas y soluciones

### Texto alternativo

El texto alternativo que contiene guiones bajos no se representa correctamente. Por ejemplo, en lugar de poner esto:

```markdown
![Settings_Step_2] (/assets/settings_step_2.png)
```

Lo mejor es utilizar guiones (-) en lugar de guiones bajos (_) en los nombres de archivo.

```markdown
![Settings-Step-2] (/assets/settings-step-2.png)
```

### Apóstrofes y comillas

Si copia texto en un editor de Markdown, el texto puede contener apóstrofos &quot;inteligentes&quot; (curvos) o comillas. Deben codificarse o cambiarse por apóstrofos básicos o comillas. De lo contrario, aparecerán caracteres extraños como este cuando se publique el archivo: Itâ€™s

Estas son las codificaciones para las versiones &quot;inteligentes&quot; de estos signos de puntuación:

- Comilla tipográfica izquierda (apertura): `&#8220;`
- Comilla tipográfica derecha (cierre): `&#8221;`
- Comilla tipográfica derecha simple (cierre) a la derecha o apóstrofo: `&#8217;`
- Comilla tipográfica izquierda simple (apertura; poco usada): `&#8216;`

### Antilambdas

Si utiliza antilambdas en un texto (que no sea código) del archivo, por ejemplo, para denotar un marcador de posición, debe codificarlos manualmente. De lo contrario, Markdown considera que se trata de una etiqueta HTML.

Por ejemplo, codifique `<script name>` como `&lt;script name&gt;`

### El símbolo &quot;et&quot; en los títulos

El símbolo &quot;et&quot; (&amp;) no se permite en los títulos. Utilice &quot;y&quot; o la codificación `&amp;`.

## Consulte también

### Recursos de Markdown

- [Introducción a Markdown](https://daringfireball.net/projects/markdown/syntax)
- [Fundamentos de Markdown para GitHub](https://help.github.com/articles/markdown-basics/)
