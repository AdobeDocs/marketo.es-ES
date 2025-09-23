---
unique-page-id: 4719291
description: Establecer apellidos y nombre de empresa de la persona predeterminada - Documentos de Marketo - Documentación del producto
title: Establecer apellidos de persona y nombre de empresa predeterminados
exl-id: 0216fb41-adf0-4ccf-be22-c064e90be65a
feature: Salesforce Integration
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '139'
ht-degree: 11%

---

# Establecer apellidos de persona y nombre de empresa predeterminados {#set-default-person-last-name-and-company-name}

[!DNL Salesforce] requiere (como mínimo) apellidos y nombre de compañía para sus posibles clientes y contactos. Los registros incompletos no se sincronizarán con [!DNL Salesforce]. Si desea sincronizar registros parciales, debe establecer los valores predeterminados que Marketo usará con [!DNL Salesforce].

1. Vaya a **[!UICONTROL Admin]** y haga clic en **[!DNL Salesforce]**.

   ![](assets/image2014-12-9-13-3a41-3a58.png)

1. Haga clic en **[!UICONTROL Editar opciones de sincronización]**.

   ![](assets/image2014-12-9-13-3a42-3a6.png)

1. Escriba **[!UICONTROL apellidos de persona predeterminada]** y **[!UICONTROL compañía de persona predeterminada]**; a continuación, haga clic en **[!UICONTROL Guardar]**.

   ![](assets/sync-options-hands.png)

   >[!NOTE]
   >
   >Marketo Engage solo asigna un valor predeterminado cuando el registro se sincroniza inicialmente con Salesforce y solo si alguno de los campos obligatorios está vacío.

¡Y eso es todo! Cada vez que a una persona le falta un apellido o un nombre de empresa, Marketo agrega el valor predeterminado a medida que sincroniza el registro.
