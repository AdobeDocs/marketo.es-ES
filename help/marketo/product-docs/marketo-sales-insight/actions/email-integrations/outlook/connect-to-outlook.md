---
description: 'Conectar con Outlook: documentos de Marketo: documentación del producto'
title: Conectar con Outlook
source-git-commit: 2538bd5973eb3372352c3ddbada6521911f9fc33
workflow-type: tm+mt
source-wordcount: '521'
ht-degree: 0%

---

# Conectar con Outlook {#connect-to-outlook}

Obtenga información sobre cómo conectar su cuenta de acciones de información de ventas con Outlook.

>[!NOTE]
>
>Cada usuario debe conectarse a Outlook desde su cuenta de ventas de Marketo.

## Conectarse a Outlook Online {#connecting-to-outlook-online}

La conexión a Outlook significa que recibirá seguimiento de respuestas, acceso al canal de entrega de Outlook, la capacidad de programar correos electrónicos en Outlook y enviar conformidad.

1. En Marketo Sales, haga clic en el icono de engranaje y seleccione **Configuración**.

   ![](assets/connect-to-outlook-1.png)

1. En Mi cuenta, seleccione **Configuración de correo electrónico**.

   ![](assets/connect-to-outlook-2.png)

1. Haga clic en **Conexión de correo electrónico** pestaña.

   ![](assets/connect-to-outlook-3.png)

1. Clic **Primeros pasos**.

   ![](assets/connect-to-outlook-4.png)

1. Seleccionar **Uso Outlook para enviar correos electrónicos** y haga clic en **Siguiente**.

   ![](assets/connect-to-outlook-5.png)

1. Seleccione la versión de Outlook que está utilizando y haga clic en **Siguiente**. En este ejemplo elegimos Outlook en línea.

   ![](assets/connect-to-outlook-6.png)

   <table> 
    <tbody>
     <tr>
      <td><strong>Outlook Online</strong></td> 
      <td>También conocido como Exchange Online</td> 
     </tr>
     <tr>
      <td><strong>Exchange On-Premise</strong></td> 
      <td>Incluye Exchange 2013 y 2016</td> 
     </tr>
    </tbody>
   </table>

   >[!NOTE]
   >
   >Marketo no admite cuentas híbridas de Exchange en este momento.

1. Clic **OK**.

   ![](assets/connect-to-outlook-7.png)

1. Si no ha iniciado sesión en Outlook, escriba la información de inicio de sesión y haga clic en **Siguiente**. Si lo está, elija la cuenta a la que desee conectarse y haga clic en **Siguiente**. En este ejemplo, ya hemos iniciado sesión.

   ![](assets/connect-to-outlook-8.png)

1. Clic **Aceptar**.

   ![](assets/connect-to-outlook-9.png)

   Puede utilizar esta conexión para rastrear correos electrónicos y también como canal de envío.

   >[!NOTE]
   >
   >Outlook Online (Office365) aplica sus propios límites de envío. [Obtenga más información aquí](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/email-connection-throttling.md#email-provider-limits).

## Conectarse a Exchange local {#connecting-to-exchange-on-premise}

La conexión a Exchange local significa que recibirá seguimiento de respuestas, acceso al canal de entrega de Outlook, la capacidad de programar correos electrónicos en Outlook y enviar conformidad.

1. En Marketo Sales, haga clic en el icono de engranaje y seleccione **Configuración**.

   ![](assets/connect-to-outlook-10.png)

1. En Mi cuenta, seleccione **Configuración de correo electrónico**.

   ![](assets/connect-to-outlook-11.png)

1. Haga clic en **Conexión de correo electrónico** pestaña.

   ![](assets/connect-to-outlook-12.png)

1. Clic **Primeros pasos**.

   ![](assets/connect-to-outlook-13.png)

1. Seleccionar **Uso Outlook para enviar correos electrónicos** y haga clic en **Siguiente**.

   ![](assets/connect-to-outlook-14.png)

1. Seleccione la versión de Outlook que está utilizando y haga clic en **Siguiente**. En este ejemplo elegimos Exchange On-Premise.

   ![](assets/connect-to-outlook-15.png)

   <table> 
    <tbody>
     <tr>
      <td><strong>Outlook Online</strong></td> 
      <td>También conocido como Exchange Online</td> 
     </tr>
     <tr>
      <td><strong>Exchange On-Premise</strong></td> 
      <td>Incluye Exchange 2013 y 2016</td> 
     </tr>
    </tbody>
   </table>

1. Introduzca sus credenciales de y haga clic en **Connect**.

   ![](assets/connect-to-outlook-16.png)

   >[!NOTE]
   >
   >Si desactiva Detección automática en la lista desplegable Versión de Exchange, tendrá que solicitar a su departamento de TI la URL de Exchange.

   Puede utilizar esta conexión para rastrear correos electrónicos y también como canal de envío.

   >[!NOTE]
   >
   >Al utilizar Exchange local, su equipo de TI establecerá el límite de envío de correo electrónico.

## Obtener permiso para conectarse a Outlook Online {#getting-permission-to-connect-to-outlook-online}

Es posible que tenga que trabajar con su equipo de TI para obtener permiso para permitir que Marketo Sales se conecte a su cuenta de Outlook Online (Microsoft 365).

>[!NOTE]
>
>Informe al equipo de TI que administra su cuenta de Microsoft 365 de que la aplicación a la que necesita acceder es &quot;Marketo Sales Connect&quot;.

En función de las preferencias de su equipo informático y de la configuración actual, es mejor consultar con él sobre cómo conceder acceso. A continuación se muestran algunos artículos que pueden ayudar a guiar la conversación.

* Consentimiento global: [Aplicaciones integradas y Azure AD para administradores de Microsoft 365](https://learn.microsoft.com/en-us/microsoft-365/enterprise/integrated-apps-and-azure-ads?view=o365-worldwide){target="_blank"}
* Consentimiento del usuario: [Configurar el consentimiento de los usuarios a las aplicaciones](https://learn.microsoft.com/en-us/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal&amp;pivots=portal){target="_blank"}
* Consentimiento de administrador: [Configuración del flujo de trabajo de consentimiento de administrador](https://learn.microsoft.com/en-us/microsoft-365/admin/misc/user-consent?source=recommendations&amp;view=o365-worldwide){target="_blank"}
* Activar o desactivar el consentimiento del usuario: [Administración del consentimiento del usuario a las aplicaciones en Microsoft 365](https://learn.microsoft.com/en-us/microsoft-365/admin/misc/user-consent?source=recommendations&amp;view=o365-worldwide){target="_blank"}
* Administración con Microsoft Defender: [Administrar aplicaciones de OAuth](https://learn.microsoft.com/en-us/defender-cloud-apps/manage-app-permissions){target="_blank"}
