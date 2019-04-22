---
lastModified: 28-6-2018
title: Uso de vínculos en la documentación
seo-title: Uso de vínculos en la documentación de Adobe Git/Markdown
description: Este artículo proporciona instrucciones para crear vínculos a contenido
  e imágenes.
seo-description: Este artículo proporciona instrucciones para crear vínculos a contenido
  e imágenes para documentación de Adobe.
translation-type: tm+mt
source-git-commit: 4d8d741544e5fefe6d186e75ce4157ea127d5b16

---


# Uso de vínculos en la documentación

Este artículo describe el uso de hipervínculos en páginas de documentación. Los vínculos son fáciles de agregar en Markdown con algunas convenciones distintas. Los vínculos envían a los usuarios al contenido en la misma página, en otras páginas vecinas o en sitios y direcciones URL externas.

> [!IMPORTANT]
> Idealmente, todos los vínculos deben ser vínculos seguros (`https` vs `http`) siempre que el objetivo lo admita (que la gran mayoría debería).

## Vínculo a direcciones URL

Las palabras que incluya en el texto del vínculo deben ser el título de la página a la que está vinculando o un texto específico y descriptivo.

**Ejemplos:**

- `For more information, see the [overview article](https://github.com/AdobeDocs/target.en/help/overview.md).`

- `For more details, see [Adobe Legal Concerns](https://www.adobe.com/legal).`

## Vínculo de un artículo a otro

Para crear un vínculo en línea desde un artículo a otro dentro del mismo repositorio, utilice la siguiente sintaxis de vínculo:

- Un artículo en un directorio vincula a otro artículo en el mismo directorio:

   `[link text](article-name.md)`

- Un artículo vincula desde un subdirectorio a un artículo en el directorio raíz:

   `[link text](../article-name.md)`

- Un artículo vincula desde un subdirectorio a un artículo en el directorio raíz:

   `[link text](../../article-name.md)`

- Un artículo en el directorio raíz vincula a un artículo en un subdirectorio:

   `[link text](./directory/article-name.md)`

- Un artículo en un subdirectorio vincula a un artículo en otro subdirectorio:

   `[link text](../directory/article-name.md)`

- Un artículo en un sub-subdirectorio vincula a un artículo en otro subdirectorio:

   `[link text](../../directory/article-name.md)`

## Vínculo a anclajes

No es necesario crear anclajes. Se generan automáticamente al publicar todos los encabezados H2. Lo único que debe hacer es crear vínculos a las secciones H2 (##).

- Para vincular a un encabezado dentro del mismo artículo:

   `[link](#the-text-of-the-level2-section-separated-by-hyphens)`

   `[Link to anchors](#links-to-anchors)`

- Para vincular a un anclaje en otro artículo del mismo subdirectorio:

   `[link text](article-name.md#anchor-name)`

   `[Configure your profile](overview.md#getting-started)`

- Para vincular a un anclaje en otro subdirectorio de servicio:

   `[link text](../directory/article-name.md#anchor-name)`

   `[Configure your profile](../overview.md#configure-your-profile)`

## Vínculo a imágenes

Como práctica recomendada, las imágenes y los archivos se almacenan en un directorio llamado `assets` en el mismo nivel que el archivo Markdown que vincula a él.

- Un artículo vincula a una imagen en el subdirectorio `assets`:

   `![alt text](assets/image-name.png)`

- Un artículo vincula a una imagen en el subdirectorio `assets/no-localize`:

   `![alt text](assets/no-localize/image-name.png)`

<!--
## Bob's link test

<table id="table_C27955F6B52A45B28BEEAAF14FFC86D8"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> File Type </th> 
   <th colname="col2" class="entry"> Description </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p> <span class="filepath"> .csv </span> </p> </td> 
   <td colname="col2"> <p>A comma-separated values file (such as one created in Excel). This is the file that contains the customer attribute data. See [Link TEST](/help/setup/full-workflow.md) </p> <p> <b>Naming requirements:</b> Ensure that file name extensions do not contain white spaces. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <span class="filepath"> .fin </span> </p> </td> 
   <td colname="col2"> <p>(Required) The <span class="filepath"> .fin </span> file tells the system that you are finished uploading data. The name of the <span class="filepath"> .fin </span> file must match the name of the <span class="filepath"> .csv </span> file. </p> <p>Adobe recommends creating an empty text file with a <span class="filepath"> .fin </span> extension. An empty file saves space and upload time. </p> <p> <p>Note:  Renaming a <span class="filepath"> .fin </span> file is not allowed after it is uploaded. The <span class="filepath"> .fin </span> file must be uploaded separately and cannot be a renamed, previously uploaded file. </p> </p> <p>After you upload the <span class="filepath"> .fin </span> file in the customer attributes FTP, the system retrieves data quickly (within one minute). This differs from other Adobe FTP-based systems, which pick up data less frequently (around once per hour). </p> <p>The <span class="filepath"> .fin </span> file is not required when using the drag-and-drop upload method. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <span class="filepath"> .gz </span> or <span class="filepath"> .zip </span> </p> </td> 
   <td colname="col2"> <p> <span class="filepath"> .gz </span> (gzip) or <span class="filepath"> .zip </span> - for compressed files. A <span class="filepath"> .zip </span> file cannot contain more than one file in the archive. </p> <p> <b>Naming requirements:</b> The name of the <span class="filepath"> .zip </span> or <span class="filepath"> .gz </span> should match the name of the <span class="filepath"> .csv </span>. For example, if your <span class="filepath"> .csv </span> file is <span class="filepath"> crm_small.csv </span>, the <span class="filepath"> .zip </span> file should be <span class="filepath"> crm_small.csv.zip </span>. </p> <p>The .fin file must match the .csv. </p> </td> 
  </tr> 
 </tbody> 
</table>
-->
