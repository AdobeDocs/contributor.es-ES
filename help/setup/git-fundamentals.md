---
title: Aspectos básicos de la documentación de Git y GitHub
description: En este artículo se ofrece una descripción general de Git, del repositorio de GitHub y de cómo se organiza el contenido, así como las convenciones de nomenclatura utilizadas para la documentación de Adobe.
exl-id: 2b2ec764-4201-4bcd-802d-a034d6675793
translation-type: ht
source-git-commit: 1b1678b33059f4bc8f7aff4690f1d775e6aee2d6
workflow-type: ht
source-wordcount: '660'
ht-degree: 100%

---

# Aspectos básicos de la documentación de Git y GitHub

## Información general

Si solo necesita hacer cambios menores de texto en los artículos, no necesita comprender los detalles de este artículo. Este artículo describe el flujo de trabajo para realizar ediciones importantes, como la creación de nuevos artículos y la adición de imágenes, o para la realización de ediciones continuas en la documentación de Adobe.

Como colaborador del contenido de documentación de Adobe, puede interactuar con varias herramientas y procesos. Puede trabajar en paralelo con otros colaboradores del mismo proyecto, posiblemente en el mismo contenido e incluso al mismo tiempo. Todo esto es posible a través del software Git y GitHub.

Git es un sistema de código abierto de control de versiones que permite la colaboración. Varios colaboradores pueden trabajar en archivos que residen en *repositorios*.

GitHub es un servicio de alojamiento basado en la web para repositorios Git, como los que se usan para almacenar contenido de [docs.adobe.com](https://docs.adobe.com). En un proyecto, GitHub aloja el repositorio principal desde el cual los colaboradores pueden crear copias para realizar su propio trabajo.

## Git

Git ofrece un flujo de trabajo de contribución único y una terminología propia que hacen posible su modelo distribuido. Por ejemplo, no existen los bloqueos de archivo que normalmente se asocian con las operaciones de check-out/check-in. Git permite resolver los cambios de manera aún más precisa, comparando archivos byte a byte.

Git también utiliza una estructura jerárquica para almacenar y administrar el contenido de un proyecto:

- *Repositorio*: también denominado *repo*, es la unidad de almacenamiento más alta. Un repositorio puede contener tanto una como varias ramas.
- *Rama*: todos los repositorios contienen una rama predeterminada (generalmente denominada “maestra”) y una o varias ramas que se van a volver a fusionar con la maestra. La rama maestra sirve como la versión y la fuente actual desde la que se publica el contenido. Es el nivel superior desde el que se crean todas las demás ramas del repositorio.

Los colaboradores interactúan con Git para actualizar y manipular repositorios en los niveles local y GitHub:

- Localmente a través de herramientas como GitHub Desktop.
- A través de [www.github.com](https://www.github.com), que integra Git para administrar la reconciliación de las contribuciones que regresan al repositorio principal.

## GitHub

Todos los flujos de trabajo comienzan y finalizan en el nivel de GitHub, donde se almacena el repositorio principal de cualquier proyecto de documentación de Adobe. Las copias que los colaboradores crean para su propio uso se distribuyen entre varios ordenadores. Al final, estas copias se reconcilian nuevamente en el repositorio de GitHub principal del proyecto.

### Organización del directorio

La rama maestra o predeterminada de un proyecto sirve como la versión actual del contenido del proyecto. El contenido en la rama maestra (y en las ramas creadas a partir de ella) se organiza como se expone en los temas del artículo. Los subdirectorios se utilizan para organizar contenido y recursos de imagen.

Normalmente, se puede encontrar un directorio `help` principal en la raíz del repositorio. El directorio de artículos contiene un conjunto de subdirectorios. Los artículos de los subdirectorios tienen el formato de archivos Markdown que utilizan la extensión *.md*.

Dentro de la raíz de este directorio, puede encontrar artículos generales relacionados con el servicio general o el producto. Es habitual encontrar otra serie de subdirectorios que coinciden con las características, servicios o escenarios comunes.

### Directorio de recursos

Los directorios de guías del usuario contienen subdirectorios `/assets` para archivos de imagen a los que se hace referencia dentro de un directorio.

<!--

### Markdown file template

For convenience, the root directory of each repository typically contains a Markdown template file named `template.md`. You can use this template file as a "starter file" if you need to create a new article for submission to the repository. The file contains:

- A **metadata header** at the top of the file, delineated by two, 3-hyphen lines. It contains the various tags used for tracking information related to the article. It also includes SEO optimizations and reporting processes that Adobe uses to evaluate the performance of the content. So the metadata is important!
- Various **examples of using Markdown** to format the elements of an article.
- General **instructions on the use of Markdown extensions**, which you can use for various types of alerts.
- Examples of **embedding video** by using an iframe.
- General **instructions on the use of docs.adobe.com extensions**, which you can use for special controls such as buttons and selectors.

-->

## Solicitudes de extracción

Una *solicitud de extracción* permite a un colaborador proponer un conjunto de cambios que se aplicarán a la rama predeterminada. Los cambios (también conocidos como *commits*) se almacenan en la rama de un colaborador, por lo que GitHub puede modelar primero el impacto de la *fusión* en la rama predeterminada. Una solicitud de extracción también sirve como mecanismo para proporcionar al colaborador comentarios desde un proceso de generación/validación, y al revisor de la solicitud de extracción para resolver posibles problemas o preguntas antes de que los cambios se fusionen en la rama predeterminada.

Existen dos formas de contribuir por solicitud de extracción, según el tamaño de los cambios que desee proponer. Explicaremos esto en detalle más adelante, en la sección [Flujo de trabajo de GitHub](local-repo.md) de esta guía.
