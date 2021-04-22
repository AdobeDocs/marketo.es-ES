---
unique-page-id: 2360335
description: Bloquear actualizaciones de campos durante la importación de listas desde fuentes no confiables - Documentos de Marketo - Documentación del producto
title: Bloquear actualizaciones de campo durante la importación de lista desde fuentes que no son de confianza
exl-id: 0fd59f0c-6cb9-442c-937b-da18a4466873
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '205'
ht-degree: 0%

---

# Bloquear actualizaciones de campo durante la importación de lista desde fuentes no confiables {#block-field-updates-during-list-import-from-untrusted-sources}

Puede confiar más en los datos de algunas listas que en otras. A veces, los datos son dudosos y se desea tomar si el campo está en blanco, pero no si hay un valor existente. Esto se puede lograr bloqueando las actualizaciones de campos en campos clave.

>[!NOTE]
>
>**Se requieren permisos de administrador**

## Bloqueo de actualizaciones de campos de fuentes no confiables {#blocking-field-updates-from-untrusted-sources}

1. Vaya a **Admin** y haga clic en **Administración de campos**.

   ![](assets/image2014-9-19-9-3a38-3a38.png)

1. Busque el campo que desee, selecciónelo y, en **Acciones de campo**, haga clic en **Bloquear actualizaciones de campo**.

   ![](assets/image2014-9-19-9-3a39-3a40.png)

1. Marque **List Import untrusted source** y haga clic en **Apply**.

   ![](assets/blockupdates.png)

>[!TIP]
>
>Puede mantener los campos a salvo de todas las listas, de confianza y sin confianza, marcando también **List Import trusted source**.

Repita los pasos anteriores para cualquier otro campo que desee mantener a salvo de listas que no sean de confianza.

## Ejecución de una importación de lista no fiable {#running-an-untrusted-list-import}

1. Al ejecutar la importación de lista, asegúrese de seleccionar **Untrusted** si desea que todos los campos configurados en el paso anterior sean seguros.

   ![](assets/importpersondetails.jpg)

Para obtener instrucciones detalladas sobre la importación de listas, consulte [Importar una lista de personas](/help/marketo/getting-started/quick-wins/import-a-list-of-people.md).

¡Buen trabajo! Ahora sabe cómo mantener los campos clave a salvo de listas que no sean de confianza.
