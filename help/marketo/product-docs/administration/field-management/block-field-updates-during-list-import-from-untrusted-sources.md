---
unique-page-id: 2360335
description: Bloquear actualizaciones de campos durante la importación de listas desde fuentes que no son de confianza - Documentos de Marketo - Documentación del producto
title: Bloquear actualizaciones de campos durante la importación de listas desde orígenes que no son de confianza
exl-id: 0fd59f0c-6cb9-442c-937b-da18a4466873
source-git-commit: 20c41143d1e7839352dddbfea0951c2633987692
workflow-type: tm+mt
source-wordcount: '206'
ht-degree: 0%

---

# Bloquear actualizaciones de campos durante la importación de listas desde orígenes que no son de confianza {#block-field-updates-during-list-import-from-untrusted-sources}

Puede confiar más en los datos de algunas listas que en otras. A veces, tiene datos cuestionables y desea tomarlos si el campo está en blanco, pero no si hay un valor existente. Para ello, bloquee las actualizaciones de los campos de los campos clave.

>[!NOTE]
>
>**Permisos de administración necesarios**

## Bloqueo De Actualizaciones De Campos De Fuentes Que No Son De Confianza {#blocking-field-updates-from-untrusted-sources}

1. Vaya a la **[!UICONTROL Administrador]** área.

   ![](assets/blocking-field-updates-from-untrusted-sources-1.png)

1. Clic **[!UICONTROL Administración de campos]**.

   ![](assets/blocking-field-updates-from-untrusted-sources-2.png)

1. Busque el campo que desee, selecciónelo y, a continuación, en **[!UICONTROL Acciones de campo]**, haga clic en **[!UICONTROL Bloquear actualizaciones de campos]**.

   ![](assets/blocking-field-updates-from-untrusted-sources-3.png)

1. Marque **[!UICONTROL Importar origen que no es de confianza]** y haga clic en **[!UICONTROL Aplicar]**.

   ![](assets/blocking-field-updates-from-untrusted-sources-4.png)

>[!TIP]
>
>Puede mantener los campos a salvo de todas las listas, de confianza y no de confianza, comprobando también **[!UICONTROL Lista Importar origen de confianza]**.

Repita los pasos anteriores para cualquier otro campo que desee proteger de listas que no sean de confianza.

## Ejecución de una importación de lista que no es de confianza {#running-an-untrusted-list-import}

1. Al ejecutar la importación de la lista, asegúrese de seleccionar **[!UICONTROL No confiable]** si desea que todos los campos configurados en el paso anterior sean seguros.

   ![](assets/blocking-field-updates-from-untrusted-sources-5.png)

Para obtener instrucciones detalladas sobre la importación de listas, consulte [Importar una lista de personas](/help/marketo/getting-started/quick-wins/import-a-list-of-people.md).

¡Buen trabajo! Ahora sabe cómo mantener los campos clave a salvo de listas que no son de confianza.
