---
unique-page-id: 3571807
description: Obtenga información sobre cómo configurar el usuario de sincronización de Marketo en Dynamics 2011 local. Cree el usuario y asigne la función Usuario de sincronización de Marketo en Dynamics.
title: 'Paso 2 de 3: Configuración del usuario de sincronización de Marketo en  [!DNL Dynamics]  (local de 2011)'
exl-id: 807c8902-24a6-48b6-a5c9-96a72764fdef
feature: Microsoft Dynamics
TQID: https://experienceleague.adobe.com/g-yRCQWbdVo-5rBF--v8tmevwRkrQdiCQ3M0BB42nfE
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: b3b8a63f-51fc-40f6-a7d2-a31c5d49fb45
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 397
ht-degree: 0%

---

# Paso 2 de 3: Configuración del usuario de sincronización de Marketo en [!DNL Dynamics] (2011 local) {#step-of-set-up-marketo-sync-user-in-dynamics-on-premises}

Los pasos anteriores se han completado.

>[!PREREQUISITES]
>
>[Paso 1 de 3: Instalar la solución de Marketo (local de 2011)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-1-of-3-install-2011.md){target="_blank"}

## Asignar función de usuario de sincronización {#assign-sync-user-role}

Asigne la función Usuario de sincronización de Marketo únicamente al usuario de sincronización de Marketo. No es necesario asignarlo a ningún otro usuario.

>[!NOTE]
>
>Esto se aplica a la versión del complemento de Marketo 4.0.0.14 y posterior. Para las versiones anteriores, todos los usuarios deben tener la función de usuario de sincronización. Para actualizar Marketo, consulte [Actualizar la solución Marketo para [!DNL Microsoft Dynamics]](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md).

>[!IMPORTANT]
>
>La configuración de idioma del usuario de sincronización [&#x200B; debe establecerse en inglés](https://learn.microsoft.com/en-us/power-platform/admin/enable-languages){target="_blank"}.

1. En el menú inferior izquierdo, seleccione **[!UICONTROL Configuración]**.

   ![](assets/image2015-4-2-14-3a2-3a40.png)

1. En el árbol, seleccione **[!UICONTROL Administración]**.

   ![](assets/image2015-4-2-14-3a3-3a30.png)

1. Seleccione **[!UICONTROL Usuarios]**.

   ![](assets/image2015-4-2-14-3a4-3a37.png)

1. Aquí verá una lista de usuarios. Seleccione el usuario de sincronización de Marketo o póngase en contacto con el administrador de [Servicios de federación de Active Directory (AFDS)](https://msdn.microsoft.com/en-us/library/bb897402.aspx) para crear un nuevo usuario dedicado a Marketo. Haga clic en **[!UICONTROL Administrar roles]**.

   ![](assets/image2015-4-2-14-3a11-3a7.png)

1. Comprueba **[!UICONTROL el usuario de sincronización de Marketo]** y haz clic en **[!UICONTROL Aceptar]**.

   ![](assets/image2015-4-2-14-3a15-3a0.png)

   >[!TIP]
   >
   >Si no ve la función, vuelva al [paso 1 de 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-1-of-3-install-2011.md){target="_blank"} e importe la solución.

   >[!NOTE]
   >
   >Cualquier actualización hecha en su CRM por el usuario de sincronización _no_ se sincronizará de nuevo con Marketo.

## Configuración de la solución Marketo {#configure-marketo-solution}

Quedan algunas partes finales de la configuración antes de pasar al siguiente artículo.

1. Seleccione **[!UICONTROL Configuración]**. A continuación, seleccione **[!UICONTROL Configuración de Marketo]** en el árbol.

   ![](assets/image2015-4-2-14-3a20-3a51.png)

   >[!NOTE]
   >
   >Si falta la configuración de [!UICONTROL Marketo], intente actualizar la página. Si el problema persiste, [vuelva a publicar la solución de Marketo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-1-of-3-install-2011.md) o cierre la sesión y vuelva a iniciarla.

1. Haga clic en **[!UICONTROL Predeterminado]**.

   ![](assets/image2015-4-2-14-3a27-3a30.png)

1. Haz clic en ![](assets/image2015-4-2-14-3a29-3a1.png)

   ![](assets/image2015-4-2-14-3a28-3a40.png)

1. En la ventana emergente, seleccione el usuario de sincronización. Luego haz clic en **[!UICONTROL Aceptar]**.

   ![](assets/image2015-4-2-14-3a32-3a43.png)

1. Haga clic en **[!UICONTROL Guardar]** para guardar los cambios.

   ![](assets/image2015-4-2-14-3a34-3a15.png)

1. Haga clic en **[!UICONTROL Publicar todas las personalizaciones]**.

   ![](assets/publish-all-customizations1.png)

## Antes de continuar con el paso 3 {#before-proceeding-to-step}

    * Si desea restringir el número de registros que sincroniza, [configure un filtro de sincronización personalizado](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md) ahora.
    * Ejecute el proceso [Validate [!DNL Microsoft Dynamics] Sync](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md). Comprueba que las configuraciones iniciales se hayan realizado correctamente.
    * Inicia sesión en el usuario de sincronización de Marketo en [!DNL Microsoft Dynamics] CRM.


>[!MORELIKETHIS]
>
>[Paso 3 de 3: conectar [!DNL Microsoft Dynamics] con Marketo (local de 2011)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-3-of-3-connect-2011.md)
