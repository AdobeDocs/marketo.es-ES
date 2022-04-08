---
unique-page-id: 37357050
description: 'Actualización del paquete MSI: Documentos de Marketo: Documentación del producto'
title: Actualización del paquete MSI
exl-id: 45004990-8452-4824-a9b2-89cd8302fe43
source-git-commit: 5c4bce6ab6801b861f70722b6782df34f96fed10
workflow-type: tm+mt
source-wordcount: '222'
ht-degree: 0%

---

# Actualización del paquete MSI {#upgrading-your-msi-package}

1. Vaya a [esta página en appexchange](https://appexchange.salesforce.com/listingDetail?listingId=a0N30000001SVZmEAO){target=&quot;_blank&quot;}.

1. Inicie sesión en la instancia de Salesforce (la que está conectada a su instancia de Marketo, puede ser simulador de pruebas o producción) desde la esquina superior derecha de la página desde el paso uno. Debe tener privilegios de administrador para instalar o actualizar un paquete administrado en Salesforce.

1. Haga clic en el **Get It Now** botón. Se le pedirá que elija dónde desea instalar. Se le dará la opción de actualizar porque ya tiene una versión anterior de MSI. Elija una opción basada en la cuenta en la que inició sesión durante el paso uno.

   >[!TIP]
   >
   >Se recomienda probarlo en la instancia de entorno limitado antes de actualizar la instancia de producción.

1. Puede actualizar el paquete eligiendo &quot;Instalar solo para administradores&quot; (y proporcionar acceso MSI a perfiles específicos más adelante), &quot;Instalar para todos los usuarios&quot; o &quot;Instalar para perfiles específicos&quot;. En este ejemplo elegimos Solo administradores. Cuando haya realizado la selección, haga clic en **Actualización**.

   ![](assets/four.png)

>[!NOTE]
>
>Se recomienda actualizar el paquete solo para administradores y, a continuación, [proporcionar acceso a usuarios específicos](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/add-sales-insight-access-to-profiles.md){target=&quot;_blank&quot;} en función del número de asientos MSI comprados. Como alternativa, puede crear un perfil específico de Salesforce para los usuarios de MSI e instalar o actualizar el paquete solo para esos usuarios.
