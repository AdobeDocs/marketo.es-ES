---
unique-page-id: 4719302
description: Obtenga información sobre cómo habilitar la sincronización de objetos personalizada cuando el usuario de sincronización de Marketo utiliza un idioma que no sea el inglés. Establezca el idioma del usuario de sincronización en inglés en Salesforce y actualice el esquema.
title: Habilitar sincronización de objetos personalizados que no esté en inglés
exl-id: 5d1c5b52-5323-4f68-847b-7d24e6acd6c4
feature: Salesforce Integration
TQID: https://experienceleague.adobe.com/kPzDEdjDnDAvuJmCtPj0I2Lfl63Lset00t-LwB8DDhI
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
source-git-commit: 67c57a9162946c4b9c424ab3fd445b70e90b530a
workflow-type: tm+mt
source-wordcount: 195
ht-degree: 9%

---

# Habilitar sincronización de objetos personalizados que no esté en inglés {#enable-non-english-custom-object-sync}

Si el usuario de sincronización de Marketo está configurado en un idioma distinto del inglés, puede producirse un error al intentar habilitar una sincronización de objetos personalizada.

![](assets/image2014-12-10-13-3a17-3a51.png)

## Cómo solucionarlo {#how-to-fix}

1. Inicie sesión en [!DNL Salesforce] con el usuario de marketo sync.

   ![](assets/image2014-12-10-13-3a18-3a1.png)

1. Haga clic en el menú desplegable de nombre de usuario y seleccione **[!UICONTROL Configuración]**.

   ![](assets/image2014-12-10-13-3a18-3a11.png)

1. En **[!UICONTROL Información personal]**, haga clic en **[!UICONTROL Mi información personal]**.

   ![](assets/image2014-12-10-13-3a18-3a22.png)

1. Haga clic en **[!UICONTROL Editar]**.

   ![](assets/image2014-12-10-13-3a18-3a32.png)

1. Cambiar **[!UICONTROL idioma]** a **[!UICONTROL inglés]**.

   ![](assets/image2014-12-10-13-3a18-3a45.png)

1. Haga clic en **[!UICONTROL Guardar]**.

   ![](assets/image2014-12-10-13-3a18-3a55.png)

1. En tu [perfil de cuenta de Adobe](https://account.adobe.com/profile){target="_blank"}, desplázate hacia abajo hasta **[!UICONTROL Idiomas preferidos]** y asegúrate de que tu primer idioma esté configurado en inglés.

   ![](assets/enable-non-english-custom-object-sync-step-6.5.png)

1. En Marketo Engage, vaya a **[!UICONTROL Administración]** > **[!UICONTROL Salesforce]** > **[!UICONTROL Objetos]**. Haga clic en **[!UICONTROL Actualizar esquema]**.

   ![](assets/image2014-12-10-13-3a19-3a6.png)

1. Esto extrae la lista de objetos en inglés. Seleccione el objeto que desee y haga clic en **[!UICONTROL Habilitar sincronización]**.

   ![](assets/image2014-12-10-13-3a19-3a16.png)

1. El objeto personalizado está ahora habilitado y sincronizándose.

   ![](assets/image2014-12-10-13-3a19-3a26.png)

1. Vuelva a [!DNL Salesforce] y siga los pasos anteriores para cambiar el usuario de sincronización de nuevo a su idioma preferido.

>[!NOTE]
>
>Actualice el esquema una última vez para extraer los objetos de nuevo en su idioma.
