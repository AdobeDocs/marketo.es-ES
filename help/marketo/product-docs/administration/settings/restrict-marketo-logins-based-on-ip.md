---
unique-page-id: 2360297
description: 'Restringir los inicios de sesión de Marketo basados en IP: documentos de Marketo: documentación del producto'
title: Restringir inicios de sesión de Marketo según la dirección IP
exl-id: 5d9d0b88-b4bc-4e1b-b70c-2c2e7b4269f5
feature: Administration
source-git-commit: 3595cdc76a0f92da10dc5ddaac64c4cf83056e88
workflow-type: tm+mt
source-wordcount: '236'
ht-degree: 5%

---

# Restringir inicios de sesión de Marketo según la dirección IP {#restrict-marketo-logins-based-on-ip}

Puede restringir o permitir que los usuarios accedan a Marketo en función de sus direcciones IP. Así es cómo se hace.

>[!NOTE]
>
>**Se requieren permisos de administración**

>[!IMPORTANT]
>
>Adobe Admin Console (AAC) admite [control de acceso basado en IP](https://helpx.adobe.com/enterprise/using/ip-based-access.html){target="_blank"}. Para garantizar una transición sin problemas, las restricciones de IP de Marketo Engage existentes estarán activas, incluidos los usuarios de Adobe ID hasta el primer trimestre de 2026 en las suscripciones en las que esta función esté habilitada.
>
>* Puede configurar el acceso basado en IP de AAC en cualquier momento.
>* Las restricciones de AAC y Marketo Engage se pueden ejecutar simultáneamente. Utilice la misma lista de permitidos IP para la compatibilidad.
>
>A partir del primer trimestre de 2026, se eliminarán las restricciones de IP de Marketo Engage. El acceso basado en IP se administrará exclusivamente mediante AAC y debe configurarse para aplicar restricciones de inicio de sesión. Más adelante se anunciará una fecha final de transición.

1. Vaya al área de **[!UICONTROL Admin]**.

   ![](assets/restrict-marketo-logins-based-on-ip-1.png)

1. Haga clic en **[!UICONTROL Configuración de inicio de sesión]**.

   ![](assets/restrict-marketo-logins-based-on-ip-2.png)

1. Haga clic en **[!UICONTROL Editar restricciones de IP]**.

   ![](assets/restrict-marketo-logins-based-on-ip-3.png)

1. Elija si quiere **permitir** o **bloquear** direcciones específicas, ingrese las direcciones y luego haga clic en **[!UICONTROL Guardar]**.

   >[!NOTE]
   >
   >**Definición**
   >
   >* **[!UICONTROL Direcciones IP permitidas]**: La adición de direcciones IP permitidas es inclusiva. Incluirá todas las direcciones IP especificadas y excluirá todo lo demás.
   >* **[!UICONTROL Bloquear direcciones IP]**: impide que determinadas direcciones IP tengan acceso a Marketo.
   >* **[!UICONTROL Deshabilitar restricciones de IP]**: si se activa esta opción, se impedirá que funcionen todas las reglas de restricción. Utilícelo para realizar pruebas.

   >[!NOTE]
   >
   >Puede añadir varias restricciones, pero solo se pueden permitir TODAS o bloquear TODAS. No puede combinar los elementos permitidos y bloqueados.

   ![](assets/restrict-marketo-logins-based-on-ip-4.png)
