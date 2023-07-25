---
description: Caducidad de recursos locales - Documentos de Marketo - Documentación del producto
title: Caducidad de recurso local
exl-id: 603e3eee-0531-4139-a8f5-279831ad011f
feature: Programs
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '263'
ht-degree: 0%

---

# Caducidad de recurso local {#local-asset-expiration}

Establezca una fecha y hora de caducidad para cancelar la publicación de páginas de aterrizaje, desactivar campañas de déclencheur o detener campañas por lotes recurrentes.

## Conceder permiso de caducidad de recursos programados {#grant-schedule-asset-expiration-permission}

Para poder programar una caducidad de recursos, la función de Marketo debe tener habilitado el permiso adecuado.

>[!NOTE]
>
>**Permisos de administración necesarios**

1. En el [!UICONTROL Administrador] , haga clic en **[!UICONTROL Usuarios y funciones]**.

   ![](assets/local-asset-expiration-1.png)

1. Haga clic en **[!UICONTROL Funciones]** , seleccione el usuario al que desea conceder acceso y, a continuación, haga clic en **[!UICONTROL Editar rol]**.

   ![](assets/local-asset-expiration-2.png)

1. En [!UICONTROL Acceso a actividades de marketing], seleccione **[!UICONTROL Programar caducidad del recurso local]** y haga clic en **[!UICONTROL Guardar]**.

   ![](assets/local-asset-expiration-3.png)

## Establecer una fecha de caducidad {#set-an-expiration-date}

1. Haga clic con el botón derecho en el programa deseado y seleccione **[!UICONTROL Establecer caducidad del recurso local]**.

   ![](assets/local-asset-expiration-4.png)

1. Compruebe los recursos para los que desea establecer una fecha de caducidad y haga clic en **[!UICONTROL Definir caducidad]**.

   ![](assets/local-asset-expiration-5.png)

1. Elija una fecha de caducidad.

   ![](assets/local-asset-expiration-6.png)

1. Fije una hora. Debe programar una hora al menos 15 minutos en el futuro (no olvide introducir AM/PM). Clic **[!UICONTROL Confirmar]** cuando termine.

   ![](assets/local-asset-expiration-7.png)

>[!NOTE]
>
>* Para editar una fecha de caducidad existente, simplemente compruebe los recursos y haga clic en **[!UICONTROL Definir caducidad]**.
>* Una vez que un recurso haya caducado, ya no aparecerá en la cuadrícula Caducidad. La cuadrícula solo mostrará páginas de aterrizaje publicadas, campañas de déclencheur activas y campañas por lotes recurrentes.
>* Las caducidades programadas se eliminarán si el recurso se mueve a otro programa.

## Eliminar una fecha de caducidad {#remove-an-expiration-date}

1. Para eliminar una fecha de caducidad, compruebe los recursos y haga clic en **[!UICONTROL Eliminar caducidad]**.

   ![](assets/local-asset-expiration-8.png)

1. Revise los recursos afectados y haga clic en **[!UICONTROL Confirmar]**.

   ![](assets/local-asset-expiration-9.png)

>[!NOTE]
>
>Las fechas de caducidad inferiores a 15 minutos en el futuro no se pueden eliminar. Para &quot;eliminar&quot; la caducidad, debe esperar a que caduque el recurso y, a continuación, volver a aprobarlo o activarlo.
