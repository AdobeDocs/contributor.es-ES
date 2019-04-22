---
title: Guía del colaborador para la documentación de Adobe
seo-title: Descripción general de la guía del colaborador para documentación técnica
  de Adobe Experience Cloud
description: La guía describe cómo puede realizar sugerencias y aportaciones al sitio
  de documentación de Adobe.
seo-description: La guía describe cómo puede contribuir al Documentación técnica de
  [!UICONTROL Adobe Experience Cloud].
translation-type: tm+mt
source-git-commit: 4d8d741544e5fefe6d186e75ce4157ea127d5b16

---


# Descripción general de la Guía de colaborador para Documentación de Adobe

## ¿Qué es Documentación de colaboración?

Durante 2019, toda la documentación técnica y el contenido de activación de Adobe Experience Cloud se está migrando a una nueva plataforma, basada en los principios de código abierto, utilizando las soluciones Github, Markdown y Adobe Experience Cloud, incluidos Adobe Experience Manager, Analytics, Launch y Target.

Este modelo de código abierto mejora la calidad del contenido y la comunicación entre clientes, equipos de documentación y equipos de productos. En cada página ahora puede valorar la utilidad de contenido, los problemas de registro e incluso las sugerencias de contenido que contribuyen como solicitudes de extracción (PRS). Los equipos de documentación de Adobe supervisan diariamente las contribuciones y los problemas y realizan actualizaciones, interpolaciones y ajustes según sea necesario.

## Uso de documentación colaborativa

Como usuario de este material, independientemente de si es un empleado, socio, cliente o cliente potencial, tiene la opción de contribuir a la documentación de varias formas sencillas;

* valorar la ayuda de la página
* registrar un problema en una página específica
* incluso enviar rápidamente ediciones a la creación de artículos completos, completar con muestras de código y recursos

Esta guía describe todo lo que necesita saber para interactuar con este conjunto de materiales y contribuir a él.

<!--
> [!IMPORTANT]
> All repositories that publish to docs.adobe.com have adopted the [Adobe Open Source Code of Conduct](../code-of-conduct.md) or the [.NET Foundation Code of Conduct](https://dotnetfoundation.org/code-of-conduct). For more information, see the [Contributing](../contributing.md) article.
>
> Minor corrections or clarifications to documentation and code examples in public repositories are covered by the [Adobe Documentation Terms of Use](https://www.adobe.com/legal/terms.html). New or significant changes generate a comment in the pull request, asking you to submit an online Contribution License Agreement (CLA) if you are not an employee of Adobe. We need you to complete the online form before we can review or accept your pull request.
--->

## Realice ediciones rápidas en documentos existentes

Realizar ediciones rápidas es una buena manera de solucionar pequeños errores y omisiones en los documentos. Si un artículo incluye un botón de edición como se muestra a continuación, puede realizar una corrección rápida. Cuando edita el documento, envía una solicitud de extracción (PR) para enviarnos la solución/sugerencia y nosotros podremos vetarla, aprobarla y publicarla.

1. Firme el Contrato de licencia [de colaborador (CLA)](http://opensource.adobe.com/cla.html) si es aceptado.

   Solo necesita enviar un CLA de Adobe una vez.
1. Haga clic en ** en la columna derecha para ir al archivo Markdown de origen en GitHub.`Edit this page`**
1. Haga clic en el icono de lápiz para editar el artículo.

   > [!NOTE]
   > Si el icono de lápiz está deshabilitado, debe iniciar sesión en su cuenta de GitHub o crear una nueva cuenta.

   ![Ubicación del icono de lápiz](assets/edit-icon.png)

1. Realice los cambios en el editor web. Puede hacer clic en la pestaña **Vista previa de cambios** para comprobar el formato del cambio.
1. Una vez que haya realizado los cambios, desplácese hasta la parte inferior de la página. Introduzca un título y una descripción para su PR y haga clic en **Proponer cambio de archivo**, como se muestra en la siguiente ilustración:

   ![proposición de cambio](assets/submit-pull-request.png)

   >[!NOTE] Si recibe un mensaje de error de validación sobre cómo firmar un Acuerdo de licencia colaborador (CLA), haga clic **en Detalles** para abrir el contrato de licencia. Firme el acuerdo, si es aceptado. A continuación, cierre la solicitud de extracción y continúe.

Es así de sencillo. ¡Gracias! Los miembros del equipo de documentación revisarán y fusionarán la solicitud de extracción.

## Registrar un problema

Otra manera de comunicarnos fácilmente un problema en algún contenido es "Registrar un problema".

1. Si encuentra algún problema en un fragmento de contenido, haga clic en el vínculo `Log an Issue` en la parte inferior derecha de cualquier página. Consulte la siguiente figura:

   ![](assets/git_log_issue.png)

   > [!NOTE]
   > Para registrar un problema, debe iniciar sesión en su cuenta de GitHub o crear una nueva cuenta.

   Si hace clic en este vínculo, podrá registrar una solicitud rápida mediante la interfaz de problemas de GitHub.

1. La dirección URL de la página con el problema se rellenará automáticamente en el campo de descripción. Añada el título, escriba una breve descripción del problema y haga clic en *Enviar nuevo problema*.

   ![](assets/git_issue_example.png)

Enviar un problema notificará directamente al equipo de contenido de esta página quién podrá actuar. Cuando actualicemos el contenido, le avisaremos en la interfaz de problemas de GitHub y le notificaremos por correo electrónico cualquier actualización o cierre.

## Explicación de los permisos de GitHub

La edición de la interfaz de usuario de GitHub se adapta a sus permisos de repositorio. Las imágenes anteriores son las adecuadas para los colaboradores que no tienen permisos de escritura en el repositorio de destino. GitHub crea automáticamente una ramificación del repositorio de destino en su cuenta. Si tiene acceso de escritura al repositorio de destino, GitHub crea una rama nueva en dicho repositorio.

Adobe usa solicitudes de extracción para todos los cambios, incluso para los colaboradores que tienen acceso de escritura. La mayoría de los repositorios tienen la ramificación `master` protegida para que las actualizaciones deban enviarse como solicitudes de extracción.

La edición en el navegador es mejor para cambios menores o poco frecuentes. Si realiza grandes contribuciones o utiliza características de Git avanzadas, le recomendamos [que ramifique el repositorio y trabaje de forma local](setup/full-workflow.md).

## Proporcionar comentarios

Con un conjunto de soluciones tan grande como el de Adobe, la documentación siempre está en constante evolución. Si encuentra errores, registre un problema; si tiene sugerencias sobre el material, háganoslo saber. Díganos qué información estaba buscando. Si no encontró lo que necesitaba, háganoslo saber. Si tiene dificultades para completar su tarea, indíquenos cómo podemos ayudarle a conocer nuestras soluciones.

Gracias de parte del equipo de documentación colaborativa y de parte de todos los redactores y productores de contenido de [!UICONTROL Adobe Experience Cloud].
