---
unique-page-id: 2360335
description: Bloquear actualizaciones de campo durante la importación de Listas desde fuentes no confiables - Documentos de marketing - Documentación del producto
title: Bloquear actualizaciones de campo durante la importación de Listas desde fuentes no confiables
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '205'
ht-degree: 0%

---


# Bloquear actualizaciones de campo durante la importación de Listas desde fuentes no confiables {#block-field-updates-during-list-import-from-untrusted-sources}

Puede confiar más en los datos de algunas listas que en otras. A veces se tienen datos dudosos y se desea tomarlos si el campo está en blanco, pero no si hay un valor existente. Esto se puede lograr bloqueando las actualizaciones de campo en los campos clave.

>[!NOTE]
>
>**Se requieren permisos de administración**

## Bloqueo de actualizaciones de campo de fuentes no confiables {#blocking-field-updates-from-untrusted-sources}

1. Vaya a **Administración** y haga clic en **Administración de campos**.

   ![](assets/image2014-9-19-9-3a38-3a38.png)

1. Busque el campo que desee, selecciónelo y, a continuación, en **Acciones de campo**, haga clic en **Bloquear actualizaciones de campo**.

   ![](assets/image2014-9-19-9-3a39-3a40.png)

1. Marque **Importación de Listas de origen no confiable** y haga clic en **Aplicar**.

   ![](assets/blockupdates.png)

>[!TIP]
>
>Puede mantener los campos a salvo de todas las listas (de confianza y no de confianza) seleccionando también **Importación de Lista de origen de confianza**.

Repita los pasos anteriores para cualquier otro campo que desee mantener a salvo de listas que no sean de confianza.

## Ejecución de una importación de Lista no confiable {#running-an-untrusted-list-import}

1. Al ejecutar la importación de listas, asegúrese de seleccionar **No confiable **si desea que todos los campos configurados en el paso anterior sean seguros.

   ![](assets/importpersondetails.jpg)

Para obtener instrucciones detalladas sobre la importación de listas, consulte [Importar una Lista de personas](../../../getting-started/quick-wins/import-a-list-of-people.md).

¡Buen trabajo! Ahora sabe cómo mantener los campos clave a salvo de listas que no son de confianza.
