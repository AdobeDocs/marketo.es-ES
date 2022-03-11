---
description: Caducidad de los recursos locales - Documentos de Marketo - Documentación del producto
title: Caducidad del recurso local
exl-id: 603e3eee-0531-4139-a8f5-279831ad011f
source-git-commit: 48a49faa6a1fde1e9ac391c2bf0800123f6a5bac
workflow-type: tm+mt
source-wordcount: '263'
ht-degree: 0%

---

# Caducidad del recurso local {#local-asset-expiration}

Establezca una fecha y hora de caducidad para cancelar la publicación de páginas de aterrizaje, desactivar campañas de déclencheur o detener campañas por lotes recurrentes.

## Conceder permiso de caducidad del recurso de programación {#grant-schedule-asset-expiration-permission}

Para poder programar la caducidad de un recurso, la función de Marketo debe tener habilitados los permisos adecuados.

>[!NOTE]
>
>**Se requieren permisos de administrador**

1. En el [!UICONTROL Administrador] área, haga clic en **[!UICONTROL Usuarios y funciones]**.

   ![](assets/local-asset-expiration-1.png)

1. Haga clic en el **[!UICONTROL Funciones]** , seleccione el usuario al que desea conceder acceso y, a continuación, haga clic en **[!UICONTROL Editar función]**.

   ![](assets/local-asset-expiration-2.png)

1. En [!UICONTROL Acceso a las actividades de marketing], seleccione **[!UICONTROL Programar la caducidad del recurso local]** y haga clic en **[!UICONTROL Guardar]**.

   ![](assets/local-asset-expiration-3.png)

## Establecer una fecha de caducidad {#set-an-expiration-date}

1. Haga clic con el botón derecho en el programa deseado y seleccione **[!UICONTROL Establecer caducidad del recurso local]**.

   ![](assets/local-asset-expiration-4.png)

1. Marque los recursos para los que desee establecer una fecha de caducidad y haga clic en **[!UICONTROL Configurar caducidad]**.

   ![](assets/local-asset-expiration-5.png)

1. Elija una fecha de caducidad.

   ![](assets/local-asset-expiration-6.png)

1. Establezca una hora. Debe programar una hora de al menos 20 minutos en el futuro (no olvide entrar a la AM/PM). Haga clic en **[!UICONTROL Confirmar]** cuando haya terminado.

   ![](assets/local-asset-expiration-7.png)

>[!NOTE]
>
>* Para editar una fecha de caducidad existente, simplemente marque los recursos y haga clic en **[!UICONTROL Configurar caducidad]**.
>* Una vez que un recurso haya caducado, ya no se mostrará en la cuadrícula Caducidad . La cuadrícula solo muestra las páginas de aterrizaje publicadas, las campañas de déclencheur activas y las campañas por lotes recurrentes.
>* Las caducidades programadas se eliminarán si el recurso se mueve a otro programa.


## Eliminar una fecha de caducidad {#remove-an-expiration-date}

1. Para eliminar una fecha de caducidad, marque los recursos y haga clic en **[!UICONTROL Eliminar caducidad]**.

   ![](assets/local-asset-expiration-8.png)

1. Revise los recursos afectados y haga clic en **[!UICONTROL Confirmar]**.

   ![](assets/local-asset-expiration-9.png)

>[!NOTE]
>
>Las fechas de caducidad que hayan pasado menos de 15 minutos en el futuro no se pueden eliminar. Para &quot;quitar&quot; la caducidad, tendrá que esperar a que caduque el recurso y, a continuación, volver a aprobarlo o reactivarlo.
