---
unique-page-id: 37357050
description: 'Actualización del paquete MSI: Marketo Docs: Documentación del producto'
title: Actualización del paquete MSI
translation-type: tm+mt
source-git-commit: ed9399396c82a3b2fb93c83ffdaa1dc7b0827306
workflow-type: tm+mt
source-wordcount: '218'
ht-degree: 0%

---


# Actualización del paquete MSI {#upgrading-your-msi-package}

1. Vaya a [esta página en appexchange](https://appexchange.salesforce.com/listingDetail?listingId=a0N30000001SVZmEAO).

1. Inicie sesión en la instancia de Salesforce (la que está conectada a la instancia de Marketo, puede ser simulador de pruebas o producción) desde la esquina superior derecha de la página desde el paso uno. Debe tener privilegios de administrador para instalar o actualizar un paquete administrado en Salesforce.

1. Haga clic en el botón **Get It Now**. Se le pedirá que elija dónde desea instalar. Se le dará la opción de actualizar porque ya tiene una versión anterior de MSI. Elija una opción basada en la cuenta en la que inició sesión durante el paso uno.

   >[!TIP]
   >
   >Se recomienda probarlo en la instancia de entorno limitado antes de actualizar la instancia de producción.

1. Puede actualizar el paquete eligiendo &quot;Instalar solo para administradores&quot; (y proporcionar acceso MSI a perfiles específicos más adelante), &quot;Instalar para todos los usuarios&quot; o &quot;Instalar para perfiles específicos&quot;. En este ejemplo elegimos Solo administradores. Cuando haya realizado la selección, haga clic en **Actualizar**.

   ![](assets/four.png)

>[!NOTE]
>
>Se recomienda actualizar el paquete solo para administradores y, a continuación, [proporcionar acceso a usuarios específicos](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/setting-up-sales-insight-for-your-team.md) en función del número de asientos MSI adquiridos. Como alternativa, puede crear un perfil específico de Salesforce para los usuarios de MSI e instalar o actualizar el paquete solo para esos usuarios.
