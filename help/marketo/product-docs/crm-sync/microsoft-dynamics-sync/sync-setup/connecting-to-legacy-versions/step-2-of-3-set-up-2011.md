---
unique-page-id: 3571807
description: 'Paso 2 de 3: Configuración del usuario de sincronización de Marketo en Dynamics (2011 local): Documentos de Marketo: documentación del producto'
title: 'Paso 2 de 3: Configuración del usuario de sincronización de Marketo en Dynamics (2011 local)'
exl-id: 807c8902-24a6-48b6-a5c9-96a72764fdef
feature: Microsoft Dynamics
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '369'
ht-degree: 0%

---

# Paso 2 de 3: Configuración del usuario de sincronización de Marketo en Dynamics (2011 local) {#step-of-set-up-marketo-sync-user-in-dynamics-on-premises}

Bueno trabajo que complete los pasos anteriores, sigamos adelante.

>[!PREREQUISITES]
>
>[Paso 1 de 3: Instalar la solución de Marketo (local de 2011)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-1-of-3-install-2011.md)

## Asignar función de usuario de sincronización {#assign-sync-user-role}

Asigne la función Usuario de sincronización de Marketo únicamente al usuario de sincronización de Marketo. No es necesario asignarlo a ningún otro usuario.

>[!NOTE]
>
>Esto se aplica al complemento de Marketo versión 4.0.0.14 y posteriores. Para las versiones anteriores, todos los usuarios deben tener la función de usuario de sincronización. Para actualizar Marketo, consulte [Actualizar la solución de Marketo para Microsoft Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md).

>[!IMPORTANT]
>
>La configuración de idioma del usuario de sincronización [debe establecerse en inglés](https://portal.dynamics365support.com/knowledgebase/article/KA-01201/en-us).

1. En el menú inferior izquierdo, seleccione **Configuración**.

   ![](assets/image2015-4-2-14-3a2-3a40.png)

1. En el árbol, seleccione **Administration**.

   ![](assets/image2015-4-2-14-3a3-3a30.png)

1. Seleccionar **Usuarios**.

   ![](assets/image2015-4-2-14-3a4-3a37.png)

1. Aquí verá una lista de usuarios. Seleccione el usuario de sincronización de Marketo específico o póngase en contacto con su [Servicios de federación de Active Directory (AFDS)](https://msdn.microsoft.com/en-us/library/bb897402.aspx) para crear un nuevo usuario dedicado a Marketo. Clic **Administrar funciones**.

   ![](assets/image2015-4-2-14-3a11-3a7.png)

1. Marque **Usuario de sincronización de Marketo** y haga clic en **OK**.

   ![](assets/image2015-4-2-14-3a15-3a0.png)

   >[!TIP]
   >
   >Si no ve la función, vuelva a [paso 1 de 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-1-of-3-install-2011.md) e importe la solución.

   >[!NOTE]
   >
   >Cualquier actualización realizada en su CRM por el usuario de sincronización **no** se sincronizarán de nuevo con Marketo.

## Configuración de la solución Marketo {#configure-marketo-solution}

¡Ya casi terminamos! Solo tenemos unas pocas piezas de configuración antes de pasar al siguiente artículo.

1. Seleccionar **Configuración**. A continuación seleccione **Configuración de Marketo** en el árbol.

   ![](assets/image2015-4-2-14-3a20-3a51.png)

   >[!NOTE]
   >
   >Si falta la configuración de Marketo, intente actualizar la página. Si el problema persiste, [vuelva a publicar la solución de Marketo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-1-of-3-install-2011.md) o cierre la sesión y vuelva a iniciarla.

1. Clic **Predeterminado**.

   ![](assets/image2015-4-2-14-3a27-3a30.png)

1. Haga clic en ![](assets/image2015-4-2-14-3a29-3a1.png)

   ![](assets/image2015-4-2-14-3a28-3a40.png)

1. En la ventana emergente, seleccione el usuario de sincronización. Luego haga clic en **OK**.

   ![](assets/image2015-4-2-14-3a32-3a43.png)

1. Clic **Guardar** para guardar los cambios.

   ![](assets/image2015-4-2-14-3a34-3a15.png)

1. Clic **Publicar todas las personalizaciones**.

   ![](assets/publish-all-customizations1.png)

## Antes de continuar con el paso 3 {#before-proceeding-to-step}

    * Si desea restringir el número de registros que sincroniza, [configure un filtro de sincronización personalizado](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md) ahora.
    * Ejecute el proceso [Validar sincronización de Microsoft Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md). Comprueba que las configuraciones iniciales se hayan realizado correctamente.
    * Inicie sesión en el usuario de sincronización de Marketo en Microsoft Dynamics CRM.

¡bueno trabajo!

>[!MORELIKETHIS]
>
>[Paso 3 de 3: Conexión de Microsoft Dynamics con Marketo (2011 local)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-3-of-3-connect-2011.md)
