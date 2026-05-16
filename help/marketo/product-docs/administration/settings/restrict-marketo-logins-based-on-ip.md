---
unique-page-id: 2360297
description: Obtenga información sobre cómo permitir o bloquear inicios de sesión de Marketo por dirección IP.
title: Restringir inicios de sesión de Marketo según la dirección IP
exl-id: 5d9d0b88-b4bc-4e1b-b70c-2c2e7b4269f5
feature: Administration
TQID: https://experienceleague.adobe.com/05hhFeXOdOg2zw9ioSV3kVI9DbDscpjx-s9SKYVDzv0
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 249
ht-degree: 6%

---

# Restringir inicios de sesión de Marketo según la dirección IP {#restrict-marketo-logins-based-on-ip}

Puede restringir o permitir que los usuarios accedan a Marketo en función de sus direcciones IP. Siga los pasos a continuación.

>[!NOTE]
>
>**Se requieren permisos de administrador**

>[!IMPORTANT]
>
>Adobe Admin Console (AAC) admite [control de acceso basado en IP](https://helpx.adobe.com/es/enterprise/using/ip-based-access.html){target="_blank"}. Para garantizar una transición sin problemas, las restricciones de IP de Marketo Engage existentes estarán activas, incluidos los usuarios de Adobe ID hasta el primer trimestre de 2027 en las suscripciones en las que esta función esté habilitada.
>
>* Puede configurar el acceso basado en IP de AAC en cualquier momento.
>* Las restricciones de AAC y Marketo Engage se pueden ejecutar simultáneamente. Utilice la misma lista de permitidos IP para la compatibilidad.
>
>A partir del primer trimestre de 2027, se eliminarán las restricciones de IP de Marketo Engage. El acceso basado en IP se administrará exclusivamente mediante AAC y debe configurarse para aplicar restricciones de inicio de sesión. Más adelante se anunciará una fecha final de transición.

1. Vaya al área de **[!UICONTROL Admin]**.

   ![](assets/restrict-marketo-logins-based-on-ip-1.png)

1. Haga clic en **[!UICONTROL Configuración de inicio de sesión]**.

   ![](assets/restrict-marketo-logins-based-on-ip-2.png)

1. Haga clic en **[!UICONTROL Editar restricciones de IP]**.

   ![](assets/restrict-marketo-logins-based-on-ip-3.png)

1. Elija si desea **permitir** o **bloquear** direcciones específicas, ingrese una o más direcciones y luego haga clic en **[!UICONTROL Guardar]**.

   >[!NOTE]
   >
   >**Definición**
   >
   >* **[!UICONTROL Direcciones IP permitidas]**: La adición de direcciones IP permitidas es inclusiva. Incluirá todas las direcciones IP especificadas y excluirá todo lo demás.
   >* **[!UICONTROL Bloquear direcciones IP]**: impide que determinadas direcciones IP tengan acceso a Marketo.
   >* **[!UICONTROL Deshabilitar restricciones de IP]**: si se activa esta opción, se impedirá que funcionen todas las reglas de restricción. Utilícelo para realizar pruebas.

   >[!NOTE]
   >
   >Puede añadir varias restricciones, pero solo se pueden permitir TODAS o bloquear TODAS. No puede combinar direcciones permitidas y bloqueadas.

   ![](assets/restrict-marketo-logins-based-on-ip-4.png)
