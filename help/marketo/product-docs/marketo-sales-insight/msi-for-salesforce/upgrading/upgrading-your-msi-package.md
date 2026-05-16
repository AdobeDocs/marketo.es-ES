---
unique-page-id: 37357050
description: Obtenga información sobre cómo actualizar el paquete de Marketo Sales Insight en Salesforce. Obtenga la versión más reciente y aplique la actualización.
title: Actualizando el paquete MSI
exl-id: 45004990-8452-4824-a9b2-89cd8302fe43
feature: Marketo Sales Insights
TQID: https://experienceleague.adobe.com/wOriEL9vVh3fEb7SdMYiT2OmbrWJmEJ7yoraRr3Ogss
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: b3b8a63f-51fc-40f6-a7d2-a31c5d49fb45
topic_v2:
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 276
ht-degree: 2%

---

# Actualizando el paquete MSI {#upgrading-your-msi-package}

>[!IMPORTANT]
>
>Debido a las mejoras de seguridad realizadas por Salesforce, el paquete Sales Insight ya no puede conceder permisos a objetos estándar. En adelante, el perfil de Salesforce de los usuarios de Sales Insight necesitará tener acceso de lectura a los siguientes objetos estándar: posible cliente, contacto, cuenta y oportunidad. [Aprenda a configurarlo aquí](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md#grant-sales-insight-users-profile-access){target="_blank"}.

1. Vaya a [esta página en appexchange](https://appexchange.salesforce.com/listingDetail?listingId=a0N30000001SVZmEAO){target="_blank"}.

1. Inicie sesión en la instancia de [!DNL Salesforce] (la que está conectada a la instancia de Marketo, puede ser de zona protegida o producción) desde la esquina superior derecha de la página desde el paso uno. Debe tener privilegios de administrador para instalar o actualizar un paquete administrado en [!DNL Salesforce].

1. Haga clic en el botón **Obtenerlo ahora**. Se le pedirá que elija dónde desea instalar. Se le dará la opción de actualizar dado que ya tiene una versión anterior de MSI. Elija una opción basada en la cuenta en la que inició sesión durante el paso uno.

   >[!TIP]
   >
   >Le recomendamos que pruebe esto en la instancia de zona protegida antes de actualizar la instancia de producción.

1. Puede actualizar el paquete eligiendo &quot;Instalar solo para administradores&quot; (y proporcionar acceso MSI a perfiles específicos más adelante), &quot;Instalar para todos los usuarios&quot; o &quot;Instalar para perfiles específicos&quot;. En este ejemplo, se elige Solo administradores. Cuando hayas hecho tu selección, haz clic en **Actualizar**.

   ![](assets/four.png)

>[!NOTE]
>
>Se recomienda actualizar el paquete solo para administradores y luego [proporcionar acceso a usuarios específicos](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/add-sales-insight-access-to-profiles.md){target="_blank"} según el número de puestos de MSI adquiridos. También puede crear un perfil de Salesforce específico para usuarios MSI e instalar o actualizar el paquete solo para esos usuarios.
