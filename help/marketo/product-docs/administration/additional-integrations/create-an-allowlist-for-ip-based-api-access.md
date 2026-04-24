---
unique-page-id: 10098433
description: Restrict API access to specific IP addresses or ranges via Admin Web Services IP Restrictions.
title: Creación de una Lista de permitidos para el acceso a API basado en IP
exl-id: 1a2f2216-07ee-4d37-b883-458ea39fc452
feature: Administration
source-git-commit: d0c8f8d5dda0747a83e4a76004863c650998c75f
workflow-type: tm+mt
source-wordcount: '173'
ht-degree: 12%

---

# Creación de una Lista de permitidos para el acceso a API basado en IP {#create-an-allowlist-for-ip-based-api-access}

Sometimes, you want to give API access only to a specific IP address or a range of addresses. To do this, you first enable restrictions, then specify the IP addresses that are allowed to use the APIs.

>[!NOTE]
>
>**Se requieren permisos de administrador**

>[!CAUTION]
>
>Enabling this feature prevents you from being able to access the [Marketo MCP Server](https://experienceleague.adobe.com/es/docs/marketo-developer/marketo/mcp-server){target="_blank"} at this time. This will be fixed in an upcoming release.

1. Go to the **[!UICONTROL Admin]** area.

   ![](assets/create-an-allowlist-for-ip-based-api-access-1.png)

1. Click **[!UICONTROL Web Services]**.

   ![](assets/create-an-allowlist-for-ip-based-api-access-2.png)

1. In the **[!UICONTROL IP Restrictions]** area, click **[!UICONTROL Edit],** or click **[!UICONTROL Edit IP Restrictions]** in the upper left.

   ![](assets/create-an-allowlist-for-ip-based-api-access-3.png)

1. Check the **[!UICONTROL Enable IP Restrictions]** box and enter the IP addresses you want to Allowlist.

   ![](assets/create-an-allowlist-for-ip-based-api-access-4.png)

   >[!NOTE]
   >
   >You can enter a single IP address or a range of them, or use a wildcard.

1. Click **[!UICONTROL Add]** to open additional fields to enter more IP addresses.

   ![](assets/create-an-allowlist-for-ip-based-api-access-5.png)

1. Haga clic en **[!UICONTROL Guardar]**.

   ![](assets/create-an-allowlist-for-ip-based-api-access-6.png)
