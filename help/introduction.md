---
title: Guía del colaborador para la documentación de Adobe
seo-title: Información general sobre la Guía del colaborador para la documentación técnica de Adobe Experience Cloud
description: La guía describe cómo puede realizar sugerencias y aportaciones al sitio de documentación de Adobe.
seo-description: La guía describe cómo puede contribuir a la documentación técnica de [!UICONTROL Adobe Experience Cloud].
translation-type: tm+mt
source-git-commit: 8943af2fdf406b2e33db037bb60dfea97df2959a
workflow-type: tm+mt
source-wordcount: '837'
ht-degree: 93%

---


# Información general sobre la Guía de colaborador para la documentación de Adobe

## ¿Qué es la documentación colaborativa?

Durante 2019, toda la documentación técnica y el contenido de capacitación de Adobe Experience Cloud se migrará a una nueva plataforma basada en los principios de código abierto y en la que se utilizarán GitHub, Markdown y las soluciones de Adobe Experience Cloud, incluidas Adobe Experience Manager, Analytics, Launch y Target.

Este modelo de código abierto mejora la calidad del contenido y la comunicación entre clientes, equipos de documentación y equipos de producto. Ahora, en cada una de las páginas es posible valorar la utilidad del contenido, registrar problemas e incluso contribuir con sugerencias de contenido mediante solicitudes de extracción (PR) Git. Los equipos de documentación de Adobe supervisan diariamente las contribuciones y los problemas, y realizan las actualizaciones, las modificaciones y los ajustes necesarios.

## Uso de la documentación colaborativa

Como usuario de este material, e independientemente de si es empleado, socio, cliente o incluso cliente potencial, tiene la opción de contribuir a la documentación de varias formas sencillas:

* Valorar la utilidad de la página
* Registrar un problema en una página específica
* Enviar desde pequeñas modificaciones hasta artículos completos con recursos y ejemplos de código

En esta guía se describe todo lo que necesita saber para interactuar con este conjunto de materiales y contribuir a su creación.

<!--
>[!IMPORTANT]
>All repositories that publish to docs.adobe.com have adopted the [Adobe Open Source Code of Conduct](../code-of-conduct.md) or the [.NET Foundation Code of Conduct](https://dotnetfoundation.org/code-of-conduct). For more information, see the [Contributing](../contributing.md) article.
>
> Minor corrections or clarifications to documentation and code examples in public repositories are covered by the [Adobe Documentation Terms of Use](https://www.adobe.com/legal/terms.html). New or significant changes generate a comment in the pull request, asking you to submit an online Contribution License Agreement (CLA) if you are not an employee of Adobe. We need you to complete the online form before we can review or accept your pull request.
-->

## Realice ediciones rápidas en documentos existentes

Realizar ediciones rápidas es una buena manera de solucionar pequeños errores y omisiones en los documentos. Si un artículo incluye un botón de edición como se muestra a continuación, puede realizar una corrección rápida. Cuando edita el documento, envía una solicitud de extracción (PR) para enviarnos la solución/sugerencia y nosotros podremos vetarla, aprobarla y publicarla.

1. Si le parece aceptable, firme el [Acuerdo de licencia para colaboradores (CLA)](http://opensource.adobe.com/cla.html).

   Solo es necesario que envíe el CLA de Adobe una vez.
1. Click the **`Edit this page`** icon in the right column to go to the markdown source file on GitHub.

   ![Editar el icono de esta página](/help/assets/git_edit.png)

1. Haga clic en el icono de lápiz para editar el artículo.

   >[!NOTE]
   >
   >Si el icono de lápiz está deshabilitado, debe iniciar sesión en su cuenta de GitHub o crear una nueva.

   ![Ubicación del icono de lápiz](assets/edit-icon.png)

1. Realice los cambios en el editor web. Puede hacer clic en la pestaña **Preview changes** para comprobar el formato del cambio.
1. Una vez que haya realizado los cambios, desplácese hasta la parte inferior de la página. Introduzca un título y una descripción para su PR y haga clic en **Propose file change**, como se muestra en la siguiente ilustración:

   ![Propuesta de cambio](assets/submit-pull-request.png)

   >[!NOTE]
   >
   >Si recibe un mensaje de error de validación relativo a la firma del Acuerdo de licencia para colaboradores (CLA), haga clic en **Detalles** para abrir el acuerdo de licencia. Si acepta las condiciones, firme el acuerdo. A continuación, cierre y abra la solicitud de extracción, y continúe.

Es así de sencillo. ¡Gracias! Los integrantes del equipo de documentación revisarán y fusionarán la solicitud de extracción.

## Registrar un problema

Otra manera de comunicarnos fácilmente un problema en algún contenido es &quot;Registrar un problema&quot;.

1. If you see a problem with a piece of content, click the **`Log an Issue`** icon in the right column.

   ![](assets/git_log_issue.png)

   >[!NOTE]
   >
   >Deberá iniciar sesión en su cuenta de GitHub o crear una nueva cuenta para registrar un problema.

   Si hace clic en este vínculo, podrá registrar una solicitud rápida mediante la interfaz de problemas de GitHub.

1. La dirección URL de la página con el problema se rellenará automáticamente en el campo de descripción. Añada el título, escriba una breve descripción del problema y haga clic en *Submit new issue*.

   ![](assets/git_issue_example.png)

Al enviar un problema, el equipo de contenido de esta página recibe una notificación para que se ponga manos a la obra. Cuando actualicemos el contenido, le avisaremos en la interfaz de problemas de GitHub y le notificaremos por correo electrónico cualquier actualización o cierre.

## Explicación de los permisos de GitHub

La edición de la interfaz de usuario de GitHub se adapta a sus permisos de repositorio. Las imágenes anteriores son las adecuadas para los colaboradores que no tienen permisos de escritura en el repositorio de destino. GitHub crea automáticamente una ramificación del repositorio de destino en su cuenta. Si tiene acceso de escritura al repositorio de destino, GitHub crea una rama nueva en dicho repositorio.

Adobe usa solicitudes de extracción para todos los cambios, incluso para los colaboradores que tienen acceso de escritura. La mayoría de los repositorios tienen la ramificación `master` protegida para que las actualizaciones deban enviarse como solicitudes de extracción.

La edición en el navegador es mejor para cambios menores o poco frecuentes. Si realiza grandes contribuciones o utiliza características de Git avanzadas, le recomendamos [que ramifique el repositorio y trabaje de forma local](setup/full-workflow.md).

## Proporcionar comentarios

Con un conjunto de soluciones tan grande como el de Adobe, la documentación siempre está en constante evolución. Si encuentra errores, registre un problema; si tiene sugerencias sobre el material, háganoslo saber. Díganos qué información estaba buscando. Si no encontró lo que necesitaba, háganoslo saber. Si tiene dificultades para completar su tarea, indíquenos cómo podemos ayudarle a conocer nuestras soluciones.

Gracias de parte del equipo de documentación colaborativa y de todos los redactores y productores de contenido de [!UICONTROL Adobe Experience Cloud].
