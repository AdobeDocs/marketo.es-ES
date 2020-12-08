---
unique-page-id: 3571807
description: Paso 2 de 3 - Configuración del usuario de sincronización de marketing en Dynamics (On-premies 2011) - Documentos de marketing - Documentación del producto
title: 'Paso 2 de 3: Configuración del usuario de sincronización de marketing en Dynamics (On-premies 2011)'
translation-type: tm+mt
source-git-commit: dc20aede0894a09e6c0bcd3d1580859b5fecb5f1
workflow-type: tm+mt
source-wordcount: '349'
ht-degree: 0%

---


# Paso 2 de 3: Configuración del usuario de sincronización de marketing en Dynamics (On-premies 2011) {#step-of-set-up-marketo-sync-user-in-dynamics-on-premises}

Bueno trabajo al completar los pasos anteriores, sigamos avanzando.

>[!NOTE]
>
>**Requisitos previos**
>
>* [Paso 1 de 3: Instalación de la solución de marketing (locales para 2011)](step-1-of-3-install.md)

>



## Asignar función de usuario de sincronización {#assign-sync-user-role}

Asigne la función de usuario de sincronización de marketing solo al usuario de sincronización de marketing. No es necesario asignarlo a ningún otro usuario.

>[!NOTE]
>
>Esto se aplica al complemento de marketing versión 4.0.0.14 y posterior. Para las versiones anteriores, todos los usuarios deben tener la función de sincronización de usuarios. Para actualizar Marketing, consulte [Actualización de la solución de marketing para Microsoft Dynamics](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution/upgrade-the-marketo-solution-for-microsoft-dynamics.md).

1. En el menú inferior izquierdo, seleccione **Configuración**.

   ![](assets/image2015-4-2-14-3a2-3a40.png)

1. En el árbol, seleccione **Administración**.

   ![](assets/image2015-4-2-14-3a3-3a30.png)

1. Seleccione **Usuarios**.

   ![](assets/image2015-4-2-14-3a4-3a37.png)

1. Aquí verá una lista de usuarios. Seleccione el usuario de sincronización de Marketing dedicado o póngase en contacto con el administrador de [Active Directory Federation Services (AFDS)](https://msdn.microsoft.com/en-us/library/bb897402.aspx) para crear un nuevo usuario dedicado a Marketing. Haga clic en **Administrar funciones**.

   ![](assets/image2015-4-2-14-3a11-3a7.png)

1. Marque **para sincronizar usuario** y haga clic en **Aceptar**.

   ![](assets/image2015-4-2-14-3a15-3a0.png)

   >[!TIP]
   >
   >Si no ve la función, vuelva al [paso 1 de 3](step-1-of-3-install.md) e importe la solución.

   >[!NOTE]
   >
   >Las actualizaciones realizadas en su CRM por el usuario de sincronización **no se sincronizarán** de nuevo con Marketing.

## Configurar la solución de marketing {#configure-marketo-solution}

¡Casi terminado! Solo tenemos algunas últimas piezas de configuración antes de pasar al siguiente artículo.

1. Seleccione **Configuración**. A continuación, seleccione **Configuración de marketing **en el árbol.

   ![](assets/image2015-4-2-14-3a20-3a51.png)

   >[!NOTE]
   >
   >Si falta la configuración de Marketing to, intente actualizar la página. Si el problema persiste, [publique de nuevo](step-1-of-3-install.md) la solución de marketing o cierre la sesión y vuelva a iniciarla.

1. Haga clic en **Predeterminado**.

   ![](assets/image2015-4-2-14-3a27-3a30.png)

1. Haga clic en ![](assets/image2015-4-2-14-3a29-3a1.png)

   ![](assets/image2015-4-2-14-3a28-3a40.png)

1. En la ventana emergente, seleccione el usuario de sincronización. A continuación, haga clic en **Aceptar**.

   ![](assets/image2015-4-2-14-3a32-3a43.png)

1. Haga clic en **Guardar** para guardar los cambios.

   ![](assets/image2015-4-2-14-3a34-3a15.png)

1. Haga clic en **Publicar todas las personalizaciones**.

   ![](assets/publish-all-customizations1.png)

## Antes de continuar con el paso 3 {#before-proceeding-to-step}

    * Si desea restringir el número de registros que sincroniza, [configure un filtro de sincronización personalizado](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md) ahora.
    * Ejecute el proceso [Validar Microsoft Dynamics Sync](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md). Verifica que la configuración inicial se realizó correctamente.
    * Inicie sesión en el usuario de sincronización de marketing en Microsoft Dynamics CRM.

¡bueno trabajo!

>[!NOTE]
>
>**Artículos relacionados**
>
>[Paso 3 de 3: Conectar Microsoft Dynamics con Marketing (On-situ 2011)](step-3-of-3-connect.md)

