---
unique-page-id: 7511512
description: Instalación y configuración de Marketo Sales Insight en Salesforce1 - Marketo Docs - Documentación del producto
title: Instalar y configurar Marketo Sales Insight en Salesforce1
exl-id: 9f26e90b-3199-4ef8-92bc-95e8bd81f1c5
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '367'
ht-degree: 0%

---

# Instalar y configurar Marketo Sales Insight en Salesforce1 {#install-and-configure-marketo-sales-insight-in-salesforce}

>[!NOTE]
>
>Clientes existentes, [Actualizar el paquete MSI](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md) antes de continuar!

>[!PREREQUISITES]
>
>Si tiene Salesforce Enterprise/Unlimited:
>
>* [Paso 1 de 3: Agregar campos de Marketo a Salesforce (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited.md)
>* [Paso 2 de 3: Crear un usuario de Salesforce para Marketo (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md)
>* [Paso 3 de 3: Conectar Marketo y Salesforce (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-3-of-3-connect-marketo-and-salesforce-enterprise-unlimited.md)
>* [Configurar la perspectiva de ventas de Marketo en Salesforce Enterprise/Unlimited](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md)
>
>Si tiene Salesforce Professional:
>
>* [Configurar Marketo Sales Insight en Salesforce Professional Edition](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md)
>


>[!NOTE]
>
>La perspectiva de ventas de Marketo en Salesforce1 incluye: Mejores apuestas, Fuente de posibles clientes, Momentos interesantes y Añadir a Marketo Campaign.

## Habilitar la aplicación móvil de Salesforce1 {#enable-the-salesforce1-mobile-app}

1. Haga clic en **Configuración** y luego **Administración de móviles**.

   ![](assets/image2015-4-21-15-3a29-3a22.png)

1. Haga clic en **Salesforce1**.

   ![](assets/image2015-4-21-15-3a30-3a51.png)

1. Haga clic en **Configuración de Salesforce1**.

   ![](assets/image2015-4-21-15-3a32-3a21.png)

1. Haga clic en **Habilitar la aplicación de navegador móvil Salesforce1**.

   ![](assets/image2015-4-21-15-3a34-3a27.png)

1. Haga clic en **Guardar**.

   ![](assets/image2015-4-21-15-3a42-3a48.png)

1. Select **Administración de móviles**.

   ![](assets/image2015-4-22-11-3a10-3a14.png)

1. Haga clic en **Administrar el menú de navegación móvil**.

   ![](assets/image2015-4-22-11-3a13-3a10.png)

1. Select **Marketo** y **Agregar** a la **Seleccionado** elementos de menú.

   ![](assets/image2015-4-22-14-3a55-3a37.png)

1. Select **Marketo**, muévalo **Up** a un área deseada y haga clic en **Guardar**.

   ![](assets/image2015-4-22-17-3a20-3a56.png)

## Ocultar objeto personalizado de Marketo obsoleto {#hide-outdated-marketo-custom-object}

1. Haga clic en **Configuración**.

   ![](assets/image2015-4-22-15-3a13-3a48.png)

1. Select **Administrar usuarios**.

   ![](assets/image2015-5-5-11-3a13-3a45.png)

1. Select **Perfiles**.

   ![](assets/image2015-5-5-11-3a15-3a21.png)

1. Haga clic en **editar** cualquier perfil deseado.

   ![](assets/image2015-5-5-13-3a51-3a36.png)

1. En **Configuración de pestañas**, seleccione _first_ **Marketo**.

   ![](assets/image2015-5-5-13-3a55-3a36.png)

1. Select **Tabulación oculta**.

   ![](assets/image2015-5-5-14-3a2-3a29.png)

   >[!NOTE]
   >
   >Asegúrese de ocultar la pestaña Marketo para todos los perfiles deseados.

## Personalizar fichas {#customize-tabs}

1. Haga clic **+**.

   ![](assets/image2015-4-22-17-3a14-3a49.png)

1. Haga clic en **Personalizar mis fichas**.

   ![](assets/image2015-4-22-17-3a16-3a22.png)

1. Select **Marketo** y **Agregar** hasta las fichas seleccionadas.

   ![](assets/image2015-4-22-17-3a17-3a15.png)

1. Select **Marketo**, muévalo **Up** a un área deseada y haga clic en **Guardar**.

   ![](assets/image2015-4-22-18-3a29-3a47.png)

## Personalizar diseños de página {#customize-page-layouts}

1. Haga clic en **Configuración**.

   ![](assets/image2015-4-22-17-3a26-3a56.png)

1. Haga clic en **Configuración**, tipo **Diseños de página** y haga clic en **Diseños de página** en Posibles clientes.

   >[!NOTE]
   >
   >Repita los pasos para cada diseño de página que utilice su organización (marketing, ventas, etc.) para objetos Contacto, Cuenta y Oportunidad.

   ![](assets/image2015-4-22-17-3a34-3a33.png)

1. Haga clic en **Editar** para realizar cambios en el diseño de posible cliente.

   ![](assets/image2015-4-22-17-3a44-3a0.png)

1. Haga clic en **Páginas de VisualForce** y, a continuación, arrastre **Móvil de posible cliente** a la sección Tarjetas móviles .

   ![](assets/image2015-4-22-17-3a49-3a37.png)

1. Cambie Height a 66 y haga clic en **OK**.

   ![](assets/image2015-4-22-17-3a52-3a15.png)

1. Haga clic en **Campos** y arrastre **Añadir a Marketo Campaign** a **Perspectiva de ventas de Marketo** para obtener más información.

   ![](assets/configure-step-6.png)

   >[!TIP]
   >
   >Escriba &quot;Agregar a&quot; en la Búsqueda rápida para que Agregar a Marketo Campaign sea fácil de encontrar.

1. Haga clic en **Guardar**.

   ![](assets/image2015-4-22-18-3a1-3a56.png)

¡Uf! Por último, ha terminado de instalar Marketo Sales Insight para Salesforce1! Adelante, dale una palmada en la espalda.

>[!MORELIKETHIS]
>
>* [Mejores apuestas en Salesforce1](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/msi-for-mobile/best-bets-in-salesforce1.md)
>* [Momentos interesantes en Salesforce1](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/msi-for-mobile/interesting-moments-in-salesforce1.md)
>* [Enviar acciones de correo electrónico y de campaña y lista de observación de Marketo en Salesforce1](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/msi-for-mobile/send-marketo-email-and-campaign-and-watchlist-actions-in-salesforce1.md)

