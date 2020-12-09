---
unique-page-id: 7504739
description: Instalación de Marketing para Dynamics 2015 On-Prem y 2016 365 On-Prem Paso 2 de 3 - Documentos de marketing - Documentación del producto
title: Instalación de Marketing para Dynamics 2015 On-Prem y 2016 365 On-Prem Paso 2 de 3
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '327'
ht-degree: 0%

---


# Paso 2 de 3

<!--Install Marketo for Dynamics 2015 On-Prem and 2016 365 On-Prem Step 2 of 3-->

Bueno trabajo que completa los pasos anteriores. Sigamos adelante.

>[!PREREQUISITES]
>
>* [Instalación de Marketing para Dynamics 2015 On-Prem y 2016 365 On-Prem Paso 1 de 3](step-1-of-3-install.md)

>



## Asignar función de usuario de sincronización {#assign-sync-user-role}

Asigne la función de usuario de sincronización de marketing solo al usuario de sincronización de marketing. No es necesario asignarlo a ningún otro usuario.

>[!NOTE]
>
>Esto se aplica a la versión 4.0.0.14 y posterior de Marketing. Para las versiones anteriores, todos los usuarios deben tener la función de sincronización de usuarios. Para actualizar el Marketing, consulte [Actualización de la solución de marketing para Microsoft Dynamics](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution/upgrade-the-marketo-solution-for-microsoft-dynamics.md).

1. En **Configuración**, haga clic en **Seguridad**.

   ![](assets/assign1.png)

1. Haga clic en **Usuarios**.

   ![](assets/assign2.png)

1. Aquí verá una lista de usuarios. Seleccione el usuario dedicado de Marketingto Sync o póngase en contacto con el administrador de [Active Directory Federation Services](https://msdn.microsoft.com/en-us/library/bb897402.aspx)(ADFS) para crear un usuario dedicado para Marketing.

   ![](assets/image2015-3-26-10-3a39-3a35.png)

1. Seleccione el usuario de sincronización. Haga clic en **Administrar funciones**.

   ![](assets/assign4.png)

   Seleccione Usuario de sincronización de marketing y haga clic en Aceptar.

   ![](assets/assign5.png)

   >[!TIP]
   >
   >Si no ve la función, vuelva al [paso 1 de 3](step-1-of-3-install.md) e importe la solución.

   >[!NOTE]
   >
   >Las actualizaciones realizadas en su CRM por el usuario de sincronización **no se sincronizarán** de nuevo con Marketing.

## Configurar la solución de marketing {#configure-marketo-solution}

¡Casi terminado! Solo tenemos algunas últimas piezas de configuración antes de pasar al siguiente artículo.

1. En **Configuración**, haga clic en Configuración **de marketing**.

   ![](assets/configure1.png)

   >[!NOTE]
   >
   >Si falta la configuración de Marketing to, intente actualizar la página. Si el problema persiste, [publique la solución](https://docs.marketo.com/pages/viewpage.action?pageId=3571822#publish-customizations) de marketing o intente cerrar la sesión y volver a iniciarla.

1. Haga clic en **Predeterminado**.

   ![](assets/configure2.png)

1. Haga clic en el campo Usuario **de** marketing y seleccione el usuario de sincronización.

   ![](assets/configure3.png)

1. Haga clic en el icono Guardar en la esquina inferior derecha.

   ![](assets/configure4.png)

1. Haga clic en **Publicar todas las personalizaciones**.

   ![](assets/publish-all-customizations1.png)

## Antes de continuar con el paso 3 {#before-proceeding-to-step}

* Si desea restringir el número de registros que sincroniza, [configure un filtro](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md) de sincronización personalizado ahora.
* Ejecute el proceso de [validación de Microsoft Dynamics Sync](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md) . Verifica que la configuración inicial se realizó correctamente.
* Inicie sesión en el usuario de sincronización de marketing en Microsoft Dynamics CRM.

>[!NOTE]
>
>**Artículos relacionados**
>
>[Instalación de Marketing para Dynamics 2015 On-Prem y 2016 365 On-Prem Paso 3 de 3](step-3-of-3-connect.md)
