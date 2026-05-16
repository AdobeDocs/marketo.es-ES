---
unique-page-id: 10098433
description: Restrinja el acceso de la API a direcciones IP o rangos específicos mediante las restricciones IP de los servicios web de administración.
title: Creación de una Lista de permitidos para el acceso a API basado en IP
exl-id: 1a2f2216-07ee-4d37-b883-458ea39fc452
feature: Administration
TQID: https://experienceleague.adobe.com/MIuDfjHpqBC2Z-hMEgtk0BvK-W2DEL25M-j6GNQK9zI
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: b13bd2ad-8e65-49e5-9691-2a0d31067b35
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 175
ht-degree: 12%

---

# Creación de una Lista de permitidos para el acceso a API basado en IP {#create-an-allowlist-for-ip-based-api-access}

A veces, desea conceder acceso a la API solo a una dirección IP específica o a un intervalo de direcciones. Para ello, primero debe habilitar las restricciones y luego especificar las direcciones IP permitidas para utilizar las API.

>[!NOTE]
>
>**Se requieren permisos de administrador**

>[!CAUTION]
>
>Si habilita esta característica, no podrá obtener acceso a [Marketo MCP Server](https://experienceleague.adobe.com/es/docs/marketo-developer/marketo/mcp-server){target="_blank"} en este momento. Se espera que esto se resuelva en una próxima versión.

1. Vaya al área de **[!UICONTROL Admin]**.

   ![](assets/create-an-allowlist-for-ip-based-api-access-1.png)

1. Haga clic en **[!UICONTROL Servicios web]**.

   ![](assets/create-an-allowlist-for-ip-based-api-access-2.png)

1. En el área **[!UICONTROL Restricciones de IP]**, haga clic en **[!UICONTROL Editar],** o en **[!UICONTROL Editar restricciones de IP]** en la esquina superior izquierda.

   ![](assets/create-an-allowlist-for-ip-based-api-access-3.png)

1. Marque la casilla **[!UICONTROL Habilitar restricciones de IP]** e introduzca las direcciones IP que desea Lista de permitidos.

   ![](assets/create-an-allowlist-for-ip-based-api-access-4.png)

   >[!NOTE]
   >
   >Puede introducir una sola dirección IP o un intervalo de ellas, o utilizar un comodín.

1. Haga clic en **[!UICONTROL Agregar]** para abrir campos adicionales e introducir más direcciones IP.

   ![](assets/create-an-allowlist-for-ip-based-api-access-5.png)

1. Haga clic en **[!UICONTROL Guardar]**.

   ![](assets/create-an-allowlist-for-ip-based-api-access-6.png)
