---
lastModified: 28-6-2018
title: Flujo de trabajo de contribución en GitHub para cambios importantes
seo-title: Flujo de trabajo de contribución en GitHub para cambios importantes en la documentación de Adobe
description: Este artículo muestra cómo utilizar el flujo de trabajo de colaborador "principal" para contribuir a la documentación de Adobe.
seo-description: Este artículo muestra cómo utilizar el flujo de trabajo del colaborador "principal" para contribuir en la documentación de Adobe.
translation-type: ht
source-git-commit: 4d8d741544e5fefe6d186e75ce4157ea127d5b16

---


# Flujo de trabajo de contribución en GitHub para cambios importantes

<!--
> [!IMPORTANT]
> All repositories that publish to docs.adobe.com have adopted the [Adobe Open Source Code of Conduct](../../code-of-conduct.md) or the [.NET Foundation Code of Conduct](https://dotnetfoundation.org/code-of-conduct). For more information, see the [Contributing](../../contributing.md) article.
>
> Minor corrections or clarifications to documentation and code examples in public repositories are covered by the [Adobe Documentation Terms of Use](https://www.adobe.com/legal/terms.html). New or significant changes generate a comment in the pull request, asking you to submit an online Contribution License Agreement (CLA) if you are not an employee of Adobe. We need you to complete the online form before we can review or accept your pull request.
--->

## Información general

Este flujo de trabajo es adecuado para un colaborador que necesita realizar un cambio importante o que sea colaborador frecuente en un repositorio. Los colaboradores frecuentes suelen tener en marcha cambios continuos que pasan por varios ciclos de compilación/validación/ensayo, o abarcan varios días antes de extraerse la solicitud de desactivación y fusión.

### Terminología

Antes de comenzar, vamos a revisar algunos de los términos de Git/GitHub usados en este flujo de trabajo.

| Nombre | Descripción |
|-----------|-------------|
| Fork (Ramificación) | Una ramificación es una copia de un repositorio principal de GitHub. En la práctica, una ramificación es otro repositorio más. Sin embargo, es especial en el sentido de que GitHub mantiene una conexión bidireccional con el repositorio principal/maestro. A veces se utiliza como verbo, como en "Primero debe ramificar el repositorio". |
| Remote (remoto) | Una conexión con nombre a un repositorio remoto, como el remoto "origin" o "upstream". Git hace referencia a estos elementos como remotos porque se utilizan para hacer referencia a un repositorio alojado en otro equipo. En este flujo de trabajo, un remoto es siempre un repositorio de GitHub. |
| Origin (origen) | Nombre asignado a la conexión entre el repositorio local y el repositorio desde el cual se clona. En este flujo de trabajo, el origen representa la conexión con la ramificación. A veces se utiliza como un alias para el repositorio de origen, como en "Recuerde insertar los cambios en el origen". |
| Upstream (ascendente) | Al igual que el origen remoto, upstream es una conexión con nombre a otro repositorio. En este flujo de trabajo, upstream representa la conexión entre el repositorio local y el repositorio principal, desde el cual se creó la ramificación. A veces se utiliza como un alias para el propio repositorio de upstream, como en "Recordar extraer los cambios desde upstream". |

Si no está familiarizado con conceptos de Git y GitHub, como un repositorio o rama, revise primero los [aspectos básicos de Git y GitHub](git-fundamentals.md).

## Flujo de trabajo

>[!IMPORTANT]
> Si aún no lo ha hecho, debe completar los pasos de la sección [Ajustes](github-signup.md).

En este flujo de trabajo, los cambios fluyen en un ciclo repetitivo. Desde el repositorio local del dispositivo se dirigen hasta su ramificación de GitHub, al repositorio principal de GitHub y regresan localmente a medida que incorporan los cambios de otros colaboradores.

### Utilizar el flujo de GitHub

Recuerde de los [aspectos básicos de Git y GitHub](git-fundamentals.md) que un repositorio de Git contiene una rama maestra, además de cualquier ramificación adicional de trabajo en curso que no se haya integrado en la rama maestra. Siempre que introduce un conjunto de cambios relacionados lógicamente, es recomendable crear una *rama de trabajo* para administrar los cambios a través del flujo de trabajo. Nos referimos a ella como rama de trabajo porque es un espacio de trabajo para repetir o pulir cambios, hasta que se puedan integrar de nuevo en la rama maestra.

Aislar los cambios relacionados en una rama específica permite controlar e introducir dichos cambios de forma independiente, dirigiéndolos a un tiempo de lanzamiento específico en el ciclo de publicación. En realidad, según el tipo de trabajo que realice, puede acabar fácilmente con varias ramas de trabajo en su repositorio. No es raro trabajar en varias ramas al mismo tiempo, representando cada una de ellas un proyecto diferente.

>[!NOTE]
>No es recomendable realizar los cambios en la rama *maestra*. Imagine que utiliza la rama maestra para introducir un conjunto de cambios para la publicación programada de una función. Finaliza los cambios y está esperando para publicarlos. Mientras tanto, recibe una solicitud urgente para corregir algo, por lo que realiza el cambio en un archivo de la rama maestra y después publica el cambio. En este ejemplo, publica inadvertidamente la corrección *y* los cambios que había retenido para publicar en una fecha específica.

El siguiente paso es crear una nueva ramificación de trabajo en el repositorio local para capturar los cambios propuestos. Cada cliente Git es diferente, así que le aconsejamos que consulte la ayuda de su cliente preferido. Puede ver información general del proceso en la Guía de GitHub sobre el [flujo de GitHub](https://guides.github.com/introduction/flow/).

## Procesamiento de solicitudes de extracción

Los cambios propuestos se envían agrupados en una nueva solicitud de extracción (PR) que se agrega a la cola de PR del repositorio de destino. Una solicitud de extracción habilita el modelo de colaboración de GitHub, solicitando que los cambios de la rama de trabajo se extraigan y se fusionen en otra rama. En la mayoría de los casos, esa otra rama es la rama predeterminada o maestra en el repositorio principal.

### Validación

Antes de poder fusionar la solicitud de extracción en su rama de destino, es posible que sea necesario pasar uno o más procesos de validación PR. Los procesos de validación pueden variar según el alcance de los cambios propuestos y las reglas del repositorio de destino. Una vez enviada la solicitud de extracción, se espera que el contenido se revise y, si procede, se fusione en el repositorio principal.

### Revisar y desconectar

Una vez completado el procesamiento de todas las PR, deberá revisar los resultados (comentarios PR, URL de vista previa, etc.) para determinar si son necesarios cambios adicionales en los archivos antes de desactivar la fusión. Si un revisor de PR ha revisado la solicitud de extracción, también puede realizar comentarios si quedan problemas o preguntas pendientes por resolver antes de la fusión.

Cuando en la solicitud de extracción no existen problemas y se desactiva, los cambios se vuelven a fusionar en la rama principal y se cierra la solicitud de extracción.

### Publicación

Recuerde, la solicitud de extracción debe fusionarse con un revisor de PR antes de que los cambios se puedan incluir en la siguiente ejecución de la publicación programada. Normalmente, las solicitudes de extracción se revisan o fusionan en el orden de envío. Si la solicitud de extracción requiere la fusión para la ejecución de una publicación específica, deberá trabajar con antelación con el revisor de PR para asegurarse de que la fusión se produzca antes de la publicación.

Una vez que las contribuciones se aprueban y fusionan, el proceso de publicación docs.microsoft.com las recoge. El tiempo de publicación puede variar dependiendo del equipo que administre el repositorio al que esté contribuyendo.
