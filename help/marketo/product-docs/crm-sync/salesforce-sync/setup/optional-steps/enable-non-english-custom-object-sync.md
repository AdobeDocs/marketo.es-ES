---
unique-page-id: 4719302
description: Habilitar la sincronización de objetos personalizados que no estén en inglés - Documentos de Marketo - Documentación del producto
title: Habilitar sincronización de objetos personalizados que no esté en inglés
exl-id: 5d1c5b52-5323-4f68-847b-7d24e6acd6c4
feature: Salesforce Integration
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '155'
ht-degree: 9%

---

# Habilitar sincronización de objetos personalizados que no esté en inglés {#enable-non-english-custom-object-sync}

Si el usuario de sincronización de Marketo está configurado en un idioma distinto del inglés, puede producirse un error al intentar habilitar una sincronización de objetos personalizada.

## El error {#the-error}

![](assets/image2014-12-10-13-3a17-3a51.png)

## Dar la vuelta {#getting-around-it}

1. Inicie sesión en [!DNL Salesforce] con el usuario de marketo sync.

   ![](assets/image2014-12-10-13-3a18-3a1.png)

1. Bajo el nombre de usuario, vaya a **[!UICONTROL Configuración]**.

   ![](assets/image2014-12-10-13-3a18-3a11.png)

1. En **[!UICONTROL Información personal]**, haga clic en **[!UICONTROL Mi información personal]**.

   ![](assets/image2014-12-10-13-3a18-3a22.png)

1. Haga clic en **[!UICONTROL Editar]**.

   ![](assets/image2014-12-10-13-3a18-3a32.png)

1. Cambiar **[!UICONTROL idioma]** a **[!UICONTROL inglés]**.

   ![](assets/image2014-12-10-13-3a18-3a45.png)

1. Haga clic en **[!UICONTROL Guardar]**.

   ![](assets/image2014-12-10-13-3a18-3a55.png)

1. En Marketo, en **[!UICONTROL Administración]** > **[!UICONTROL Salesforce]** > **[!UICONTROL Objetos]**, haga clic en **[!UICONTROL Actualizar esquema]**.

   ![](assets/image2014-12-10-13-3a19-3a6.png)

1. Esto extraerá la lista de objetos en inglés. Seleccione el objeto que desee y haga clic en **[!UICONTROL Habilitar sincronización]**.

   ![](assets/image2014-12-10-13-3a19-3a16.png)

1. Observe que el objeto personalizado ahora está habilitado y sincronizándose.

   ![](assets/image2014-12-10-13-3a19-3a26.png)

1. Ahora, vuelva a [!DNL Salesforce] y siga los pasos anteriores para volver a cambiar el usuario de sincronización a su idioma preferido.

>[!NOTE]
>
>No olvide actualizar el esquema por última vez para extraer los objetos en su idioma.
