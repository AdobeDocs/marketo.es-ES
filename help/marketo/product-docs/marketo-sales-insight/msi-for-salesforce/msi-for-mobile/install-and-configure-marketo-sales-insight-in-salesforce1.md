---
unique-page-id: 7511512
description: Instalación y configuración de la perspectiva de ventas de Marketo en Salesforce1 - Documentos de Marketo - Documentación del producto
title: Instalación y configuración de Marketo Sales Insight en Salesforce1
exl-id: 9f26e90b-3199-4ef8-92bc-95e8bd81f1c5
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '374'
ht-degree: 1%

---

# Instalación y configuración de Marketo Sales Insight en Salesforce1 {#install-and-configure-marketo-sales-insight-in-salesforce}

>[!NOTE]
>
>Clientes actuales, [Actualice su paquete MSI](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md) antes de continuar.

>[!PREREQUISITES]
>
>Si tiene Salesforce Enterprise/Unlimited:
>
>* [Paso 1 de 3: Agregar campos de Marketo a Salesforce (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited.md)
>* [Paso 2 de 3: Crear un usuario de Salesforce para Marketo (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md)
>* [Paso 3 de 3: conectar Marketo y Salesforce (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-3-of-3-connect-marketo-and-salesforce-enterprise-unlimited.md)
>* [Configuración de Marketo Sales Insight en Salesforce Enterprise/Unlimited](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md)
>
>Si tiene Salesforce Professional:
>
>* [Configurar Marketo Sales Insight en Salesforce Professional Edition](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md)
>

>[!NOTE]
>
>El conocimiento de ventas de Marketo en Salesforce1 incluye: resultados más probables, fuente de posibles clientes, momentos interesantes y agregar a Marketo Campaign.

## Habilitar la aplicación móvil Salesforce1 {#enable-the-salesforce1-mobile-app}

1. Haga clic en **Configuración** y luego en **Administración móvil**.

   ![](assets/image2015-4-21-15-3a29-3a22.png)

1. Haga clic en **Salesforce1**.

   ![](assets/image2015-4-21-15-3a30-3a51.png)

1. Haga clic en **Configuración de Salesforce1**.

   ![](assets/image2015-4-21-15-3a32-3a21.png)

1. Haga clic en **Habilitar la aplicación de navegador móvil Salesforce1**.

   ![](assets/image2015-4-21-15-3a34-3a27.png)

1. Haga clic en **Guardar**.

   ![](assets/image2015-4-21-15-3a42-3a48.png)

1. Seleccione **Administración móvil**.

   ![](assets/image2015-4-22-11-3a10-3a14.png)

1. Haga clic en **Administrar el menú de navegación móvil**.

   ![](assets/image2015-4-22-11-3a13-3a10.png)

1. Seleccione **Marketo** y **agréguelo** a los **elementos de menú seleccionados**.

   ![](assets/image2015-4-22-14-3a55-3a37.png)

1. Seleccione **Marketo**, muévalo **Arriba** a un área deseada y haga clic en **Guardar**.

   ![](assets/image2015-4-22-17-3a20-3a56.png)

## Ocultar objeto personalizado de Marketo obsoleto {#hide-outdated-marketo-custom-object}

1. Haga clic en **Configuración**.

   ![](assets/image2015-4-22-15-3a13-3a48.png)

1. Seleccione **Administrar usuarios**.

   ![](assets/image2015-5-5-11-3a13-3a45.png)

1. Seleccione **Perfiles**.

   ![](assets/image2015-5-5-11-3a15-3a21.png)

1. Haga clic para **editar** cualquier perfil deseado.

   ![](assets/image2015-5-5-13-3a51-3a36.png)

1. En **Configuración de ficha**, seleccione _primero_ **Marketo**.

   ![](assets/image2015-5-5-13-3a55-3a36.png)

1. Seleccione **Tabulación oculta**.

   ![](assets/image2015-5-5-14-3a2-3a29.png)

   >[!NOTE]
   >
   >Asegúrese de ocultar la pestaña Marketo para todos los perfiles deseados.

## Personalizar fichas {#customize-tabs}

1. Haga clic en **+**.

   ![](assets/image2015-4-22-17-3a14-3a49.png)

1. Haga clic en **Personalizar mis fichas**.

   ![](assets/image2015-4-22-17-3a16-3a22.png)

1. Seleccione **Marketo** y **agréguelo** a las fichas seleccionadas.

   ![](assets/image2015-4-22-17-3a17-3a15.png)

1. Seleccione **Marketo**, muévalo **Arriba** a un área deseada y haga clic en **Guardar**.

   ![](assets/image2015-4-22-18-3a29-3a47.png)

## Personalizar diseños de página {#customize-page-layouts}

1. Haga clic en **Configuración**.

   ![](assets/image2015-4-22-17-3a26-3a56.png)

1. Haga clic en **Configuración**, escriba **Diseños de página** y haga clic en **Diseños de página** en Posibles clientes.

   >[!NOTE]
   >
   >Repita los pasos para cada Diseño de página que utilice su organización (marketing, ventas, etc.) para los objetos Contact, Account y Opportunity.

   ![](assets/image2015-4-22-17-3a34-3a33.png)

1. Haga clic en **Editar** para realizar cambios en el diseño del posible cliente.

   ![](assets/image2015-4-22-17-3a44-3a0.png)

1. Haga clic en **Páginas de Visualforce** y, a continuación, arrastre **Móvil principal** a la sección Tarjetas móviles.

   ![](assets/image2015-4-22-17-3a49-3a37.png)

1. Cambie Height a 66 y haga clic en **OK**.

   ![](assets/image2015-4-22-17-3a52-3a15.png)

1. Haga clic en **Campos** y arrastre **Agregar a Marketo Campaign** a la sección **Perspectiva de ventas de Marketo**.

   ![](assets/configure-step-6.png)

   >[!TIP]
   >
   >Escriba &quot;Agregar a&quot; en la Búsqueda rápida para que sea más fácil encontrar esta opción en Marketo Campaign.

1. Haga clic en **Guardar**.

   ![](assets/image2015-4-22-18-3a1-3a56.png)

¡Uf! Por fin ha terminado de instalar Marketo Sales Insight para Salesforce1. Adelante, date una palmadita en la espalda.

>[!MORELIKETHIS]
>
>* [Lo mejor en Salesforce1](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/msi-for-mobile/best-bets-in-salesforce1.md)
>* [Momentos interesantes en Salesforce1](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/msi-for-mobile/interesting-moments-in-salesforce1.md)
>* [Enviar correo electrónico de Marketo y acciones de campañas y listas de observación en Salesforce1](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/msi-for-mobile/send-marketo-email-and-campaign-and-watchlist-actions-in-salesforce1.md)
