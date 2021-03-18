---
unique-page-id: 7504739
description: Instalación de Marketo para Dynamics 2015 On-Prem y 2016 365 On-Prem Paso 2 de 3 - Marketo Docs - Documentación del producto
title: Instalación de Marketo para Dynamics 2015 On-Prem y 2016 365 On-Prem Paso 2 de 3
translation-type: tm+mt
source-git-commit: 9d8a6d9880de5d2af211906c2410f2057c1f454d
workflow-type: tm+mt
source-wordcount: '328'
ht-degree: 0%

---


# Paso 2 de 3 Configuración de Marketo para Dynamics (2015 On-Prem y 2016 365 On-Prem){#step-of-set-up-for-marketo-on-premises-and-365}

Bueno trabajo completando los pasos anteriores. Sigamos adelante.

>[!PREREQUISITES]
>
>[Instalación de Marketo para Dynamics 2015 On-Prem y 2016 365 On-Prem Paso 1 de 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2015-on-premises-2016-dynamics-365-on-premises/step-1-of-3-install.md)

## Asignar función de usuario de sincronización {#assign-sync-user-role}

Asigne la función de usuario de sincronización de Marketo únicamente al usuario de sincronización de Marketo. No es necesario asignarlo a ningún otro usuario.

>[!NOTE]
>
>Esto se aplica a Marketo versión 4.0.0.14 y posteriores. En versiones anteriores, todos los usuarios deben tener la función de sincronización de usuarios. Para actualizar su Marketo, consulte [Actualización de la solución Marketo para Microsoft Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md).

1. En **Configuración**, haga clic en **Seguridad**.

   ![](assets/assign1.png)

1. Haga clic en **Usuarios**.

   ![](assets/assign2.png)

1. Aquí puede ver una lista de usuarios. Seleccione el usuario dedicado de Marketo Sync o póngase en contacto con su administrador de [Servicios de federación de Active Directory](https://msdn.microsoft.com/en-us/library/bb897402.aspx) (ADFS) para crear un usuario dedicado para Marketo.

   ![](assets/image2015-3-26-10-3a39-3a35.png)

1. Seleccione el usuario de sincronización. Haga clic en **Administrar funciones**.

   ![](assets/assign4.png)

   Marketo Sync User y haga clic en OK.

   ![](assets/assign5.png)

   >[!TIP]
   >
   >Si no ve la función , vuelva al [paso 1 de 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2015-on-premises-2016-dynamics-365-on-premises/step-1-of-3-install.md) e importe la solución.

   >[!NOTE]
   >
   >Cualquier actualización realizada en su CRM por el usuario de sincronización **no** se sincronizará de nuevo con Marketo.

## Configurar la solución de Marketo {#configure-marketo-solution}

¡Casi terminado! Solo tenemos algunos últimos fragmentos de configuración antes de pasar al siguiente artículo.

1. En **Configuración**, haga clic en **Configuración de Marketo**.

   ![](assets/configure1.png)

   >[!NOTE]
   >
   >Si falta la configuración de Marketo, intente actualizar la página. Si el problema persiste, [publique la solución de Marketo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2015-on-premises-2016-dynamics-365-on-premises/step-1-of-3-install.md) o intente cerrar la sesión y volver a iniciarla.

1. Haga clic en **Default**.

   ![](assets/configure2.png)

1. Haga clic en el campo **Marketo User** y seleccione el usuario de sincronización.

   ![](assets/configure3.png)

1. Haga clic en el icono Guardar en la esquina inferior derecha.

   ![](assets/configure4.png)

1. Haga clic en **Publicar todas las personalizaciones**.

   ![](assets/publish-all-customizations1.png)

## Antes de continuar con el paso 3 {#before-proceeding-to-step}

* Si desea restringir el número de registros que sincroniza, [configure un filtro de sincronización personalizado](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md) ahora.
* Ejecute el proceso [Validate Microsoft Dynamics Sync](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md). Comprueba que la configuración inicial se haya realizado correctamente.
* Inicie sesión en el usuario de sincronización de Marketo en Microsoft Dynamics CRM.

>[!MORELIKETHIS]
>
>[Instalación de Marketo para Dynamics 2015 On-Prem y 2016 365 On-Prem Paso 3 de 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2015-on-premises-2016-dynamics-365-on-premises/step-3-of-3-connect.md)
