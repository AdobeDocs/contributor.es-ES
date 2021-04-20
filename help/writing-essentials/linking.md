---
lastModified: 2018-06-28T00:00:00Z
title: Uso de los vínculos en la documentación
seo-title: Uso de los vínculos en la documentación de Adobe Git/Markdown
description: En este artículo se explica cómo crear vínculos a contenido e imágenes.
seo-description: En este artículo se explica cómo crear vínculos a contenido e imágenes para la documentación de Adobe.
exl-id: f9d61aa9-931c-4654-ab21-c6e47936954e
translation-type: ht
source-git-commit: dad1df81797e6078645449501ed0661cf4bcf3ce
workflow-type: ht
source-wordcount: '340'
ht-degree: 100%

---

# Uso de los vínculos en la documentación

En este artículo se describe el uso de los hipervínculos en las páginas de la documentación. Los vínculos son fáciles de agregar en Markdown con algunas convenciones distintas. Los vínculos envían a los usuarios al contenido en la misma página, en otras páginas vecinas o en sitios y direcciones URL externas.

>[!IMPORTANT]
>Por norma general, los vínculos deben ser seguros (`https`, no `http`) siempre que el objetivo los admita (y la gran mayoría debería admitirlos).

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
