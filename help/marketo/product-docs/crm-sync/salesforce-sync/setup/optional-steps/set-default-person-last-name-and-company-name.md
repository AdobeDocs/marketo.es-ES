---
unique-page-id: 4719291
description: Obtenga información sobre cómo establecer los apellidos de la persona y el nombre de la empresa predeterminados para la sincronización de Salesforce. Utilice las Opciones de administración y sincronización para que los registros parciales se sincronicen con los valores predeterminados.
title: Establecer apellidos de persona y nombre de empresa predeterminados
exl-id: 0216fb41-adf0-4ccf-be22-c064e90be65a
feature: Salesforce Integration
TQID: https://experienceleague.adobe.com/pq4XPfiwO1UemSmg3edhJgWWmvR-mx4Q3udff9xzWt0
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 149
ht-degree: 10%

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

Cada vez que a una persona le falta un apellido o un nombre de empresa, Marketo agregará el valor predeterminado a medida que sincroniza el registro.
