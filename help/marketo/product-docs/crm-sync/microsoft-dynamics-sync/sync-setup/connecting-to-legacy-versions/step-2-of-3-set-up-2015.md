---
unique-page-id: 7504739
description: 'Instalación de Marketo para Microsoft Dynamics 2015 local, paso 2 de 3: documentos de Marketo: documentación del producto'
title: Instale Marketo para Microsoft Dynamics 2015 local, paso 2 de 3
exl-id: 39f00749-4ba3-47f1-b2e3-72cbaa7caf2e
feature: Microsoft Dynamics
source-git-commit: 821d69736b1cbeac0c80718c58a7a3c471387545
workflow-type: tm+mt
source-wordcount: '371'
ht-degree: 0%

---

# Paso 2 de 3: Configuración de Marketo para Dynamics (local de 2015){#step-of-set-up-for-marketo-on-premises-2015}

Buen trabajo completando los pasos anteriores. Vamos a seguir avanzando a través de esto.

>[!PREREQUISITES]
>
>[Instalar Marketo para Microsoft Dynamics 2015 local, paso 1 de 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-1-of-3-install-2015.md){target="_blank"}

## Asignar función de usuario de sincronización {#assign-sync-user-role}

Asigne la función Usuario de sincronización de Marketo únicamente al usuario de sincronización de Marketo. No es necesario asignarlo a ningún otro usuario.

>[!NOTE]
>
>Esto se aplica a la versión 4.0.0.14 y posteriores de Marketo. Para las versiones anteriores, todos los usuarios deben tener la función de usuario de sincronización. Para actualizar su Marketo, consulte [Actualizar la solución de Marketo para Microsoft Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md){target="_blank"}.

>[!IMPORTANT]
>
>La configuración de idioma del usuario de sincronización [ debe establecerse en inglés](https://portal.dynamics365support.com/knowledgebase/article/KA-01201/en-us){target="_blank"}.

1. En **[!UICONTROL Configuración]**, haga clic en **[!UICONTROL Seguridad]**.

   ![](assets/assign1.png)

1. Haga clic en **[!UICONTROL Usuarios]**.

   ![](assets/assign2.png)

1. Aquí verá una lista de usuarios. Seleccione al usuario de sincronización de Marketo o póngase en contacto con el administrador de [Servicios de federación de Active Directory](https://msdn.microsoft.com/en-us/library/bb897402.aspx){target="_blank"} (ADFS) para crear un usuario dedicado para Marketo.

   ![](assets/image2015-3-26-10-3a39-3a35.png)

1. Seleccione el usuario de sincronización. Haga clic en **[!UICONTROL Administrar roles]**.

   ![](assets/assign4.png)

1. Compruebe el usuario de sincronización de Marketo y haga clic en **[!UICONTROL Aceptar]**.

   ![](assets/assign5.png)

   >[!IMPORTANT]
   >
   >El usuario de sincronización debe tener permiso de lectura para la configuración de Marketo.

   >[!TIP]
   >
   >Si no ve la función, vuelva al [paso 1 de 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-1-of-3-install-2015.md){target="_blank"} e importe la solución.

   >[!NOTE]
   >
   >Cualquier actualización hecha en su CRM por el usuario de sincronización _no_ se sincronizará de nuevo con Marketo.

## Configuración de la solución Marketo {#configure-marketo-solution}

¡Ya casi terminamos! Solo tenemos unas pocas piezas de configuración antes de pasar al siguiente artículo.

1. En **[!UICONTROL Configuración]**, haga clic en **[!UICONTROL Configuración de Marketo]**.

   ![](assets/configure1.png)

   >[!NOTE]
   >
   >Si falta la configuración de Marketo, intente actualizar la página. Si el problema persiste, [publique la solución de Marketo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-1-of-3-install-2015.md){target="_blank"} o intente cerrar la sesión y volver a iniciarla.

1. Haga clic en **[!UICONTROL Predeterminado]**.

   ![](assets/configure2.png)

1. Haga clic en el campo **[!UICONTROL Usuario de Marketo]** y seleccione el usuario de sincronización.

   ![](assets/configure3.png)

1. Haga clic en el icono de guardar en la esquina inferior derecha.

   ![](assets/configure4.png)

1. Haga clic en **[!UICONTROL Publish All Customization]**.

   ![](assets/publish-all-customizations1.png)

   >[!NOTE]
   >
   >El usuario de sincronización debe tener permiso de lectura para la configuración de Marketo.

## Antes de continuar con el paso 3 {#before-proceeding-to-step}

* Si desea restringir el número de registros que sincroniza, [configure ahora un filtro de sincronización personalizado](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md){target="_blank"}.
* Ejecute el proceso [Validar sincronización de Microsoft Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md){target="_blank"}. Comprueba que las configuraciones iniciales se hayan realizado correctamente.
* Inicie sesión en el usuario de sincronización de Marketo en Microsoft Dynamics CRM.

>[!MORELIKETHIS]
>
>[Instalar Marketo para Microsoft Dynamics 2015 local, paso 3 de 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-3-of-3-connect-2015.md){target="_blank"}
