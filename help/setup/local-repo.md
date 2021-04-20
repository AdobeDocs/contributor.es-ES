---
title: Configurar el repositorio de Git localmente
description: Este artículo proporciona indicaciones para crear su repositorio local de Git y contribuir a la documentación de Adobe, incluidos los procesos de ramificación y clonación.
exl-id: 679c07a2-030b-4a30-ba14-7780f88dae11
translation-type: ht
source-git-commit: dad1df81797e6078645449501ed0661cf4bcf3ce
workflow-type: ht
source-wordcount: '653'
ht-degree: 100%

---

# Configure el repositorio de Git localmente para la documentación

Este artículo describe los pasos para configurar un repositorio de Git en el equipo local, con la intención de contribuir a la documentación de Adobe. Los colaboradores pueden utilizar un repositorio clonado localmente para agregar nuevos artículos, realizar ediciones importantes en artículos existentes o cambiar ilustraciones.

>[!IMPORTANT]
>Si solo realiza cambios menores en un artículo, *no* necesita completar los pasos que aquí se explican. Puede simplemente hacer clic en el icono Editar y editar el texto en el navegador.

## Información general

Para contribuir a la documentación de Adobe, puede ramificar el repositorio apropiado en su cuenta de GitHub para obtener permisos de lectura y escritura. A continuación, puede crear y editar archivos Markdown localmente mediante la clonación del repositorio de documentación correspondiente. A continuación, utilice solicitudes de extracción para fusionar (enviar) los cambios en el repositorio compartido central de solo lectura.

* Determinar el repositorio adecuado
* Ramificar el repositorio a su cuenta de GitHub
* Seleccione una carpeta local para los archivos clonados
* Clone el repositorio en el equipo local
* Configure el valor remoto del flujo ascendente

## Determine el repositorio

El repositorio adecuado se ramifica a su cuenta de GitHub para obtener permisos de lectura y escritura con el fin de almacenar los cambios propuestos. La documentación de [!UICONTROL Adobe Experience Cloud] reside en varios repositorios distintos en [github.com](https://www.github.com/adobedocs).

1. Si no está seguro del repositorio que debe utilizar, visite el artículo con su explorador Web. Seleccione el vínculo **Editar** (icono de lápiz) en la esquina superior derecha del artículo. (Si no ve un vínculo Editar, significa que ese contenido aún no está disponible en GitHub.)

Para contribuir a la documentación de Adobe, puede crear y editar archivos Markdown localmente mediante la clonación del repositorio de documentación correspondiente. A continuación, utilice solicitudes de extracción para fusionar cambios en el repositorio compartido central de solo lectura.

<!---
![GitHub Triangle](/assets/git-and-github-initial-setup.png)

If you're new to GitHub, watch the following video for a conceptual overview of the forking and cloning process:

>[!VIDEO https://channel9.msdn.com/Blogs/CoolMoose/Git-Repository-Setup/player]
-->

## Ramificar el repositorio

Utilizando el repositorio adecuado, cree una ramificación del repositorio en su cuenta de GitHub en el sitio web de GitHub.

Se requiere una ramificación personal, ya que todos los repositorios de documentación principales proporcionan acceso de solo lectura, lo que significa que no puede realizar cambios directamente en el contenido de los repositorios. Para realizar cambios, debe enviar una solicitud de extracción (PR) desde la ramificación al repositorio principal. Para facilitar este proceso, primero necesita su propia copia del repositorio, en la que tiene acceso de escritura. Una *ramificación* de GitHub sirve para ese propósito.

1. Vaya a la página del repositorio principal de GitHub y haga clic en el botón **Fork** en la esquina superior derecha.

   ![Ramificación en GitHub](assets/fork-simple.png)

1. Si se le solicita, seleccione el mosaico de su cuenta de GitHub como destino donde se debe crear la ramificación. Este mensaje crea una copia del repositorio en su cuenta de GitHub, conocida como una ramificación.

1. Elija un nombre de carpeta fácil de recordar y escribir.

   Algunos de los repositorios pueden ser grandes. Elija una ubicación con espacio disponible en el disco.

   >[!NOTE]
   >
   >Evite seleccionar una ruta de carpeta local anidada dentro de otra ubicación de carpeta del repositorio de Git. Aunque es aceptable almacenar las carpetas clonadas de Git contiguas, anidar carpetas de Git dentro de otras causa errores para el seguimiento de archivos.

## Crear un clon local del repositorio

Al crear un clon del repositorio ramificado, se descarga una copia de los archivos en su ordenador. Cuando esté listo, puede enviar ediciones desde la unidad local al repositorio ramificado en el servidor. A continuación, puede enviar una solicitud de extracción para fusionar las ediciones en la rama ascendente al repositorio principal.

Estos pasos dan por sentado que está utilizando GitHub Desktop. Si utiliza otro cliente, realice los ajustes correspondientes.

1. Haga clic en **Clone or download** y, a continuación, elija **Open in Desktop** para extraer una copia del repositorio (su ramificación) en su ordenador, en el directorio actual.

  ![Clonar repo](assets/clone-pulldown.png)

1. Utilice GitHub Desktop para mantener los archivos locales sincronizados con el repositorio ramificado.

Para obtener más información, consulte [Documentación de GitHub Desktop](https://help.github.com/desktop/).
