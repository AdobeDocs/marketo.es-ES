---
unique-page-id: 2949711
description: Instale el complemento de correo electrónico de Marketo para  [!DNL Outlook] con un código de registro - Documentos de Marketo - Documentación del producto
title: Instale el complemento de correo electrónico de Marketo para  [!DNL Outlook]  con un código de registro
exl-id: d7a877c2-f71e-44da-b323-04f6cdb44eb0
feature: Marketo Sales Insights
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '536'
ht-degree: 3%

---

# Instale el complemento de correo electrónico de Marketo para [!DNL Outlook] con un código de registro {#install-the-marketo-email-add-in-for-outlook-with-a-registration-code}

Si los usuarios pueden acceder a la configuración de administración de sus portátiles, puede enviarles directamente un código de registro.

Si no ha recibido un correo electrónico de invitación, pídale al administrador de Marketo que le invite.

>[!PREREQUISITES]
>
>Se le debe [emitir una licencia de complemento de correo electrónico de Marketo](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/issue-a-marketo-email-add-in-license.md).

>[!IMPORTANT]
>
>La instalación no es compatible con equipos en los que la carpeta Usuario de Windows contenga caracteres que no sean ingleses. Windows genera automáticamente esta carpeta en `<System Root>\Users\` según el nombre de usuario de Windows y puede contener caracteres que no sean ingleses si el nombre de usuario de Windows no es inglés. Trabaje con su equipo de TI para comprobar si tiene problemas de instalación.

>[!NOTE]
>
>Las funciones de acciones de Sales Insight, como Enviar correo electrónico de ventas, Agregar a la campaña de ventas y Tareas, no están disponibles en los complementos de correo electrónico de Sales Insight para Gmail y Outlook. En este momento, los usuarios solo pueden enviar un correo electrónico rastreable con o sin una plantilla de correo electrónico de Marketo desde su cliente de correo electrónico al utilizar los complementos de correo electrónico de Sales Insight.

## Descargar instalador {#download-installer}

1. Identifique su [versión de Microsoft Outlook](https://support.office.com/en-us/article/what-version-of-outlook-do-i-have-b3a9568c-edb5-42b9-9825-d48d82b2257c){target="_blank"}.

1. En la tabla siguiente, haga clic en el vínculo para descargar el archivo .ZIP correspondiente a su versión de Microsoft Outlook.

1. Descomprima el archivo para acceder al archivo .MSI necesario y continúe con la instalación.

   >[!NOTE]
   >
   >En este momento, los vínculos siguientes solamente funcionan en [!DNL Microsoft Edge], o haciendo clic con el botón secundario en [!DNL Chrome]. Sentimos cualquier inconveniente.

<table><thead>
  <tr>
    <th>Versión de Outlook</th>
    <th>Outlook de 32 bits</th>
    <th>Outlook de 64 bits</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Outlook 2000</td>
    <td>No compatible</td>
    <td>N/A</td>
  </tr>
  <tr>
    <td>Outlook 2003</td>
    <td><a href="https://munchkin.marketo.net/MarketoAddInSetup32.zip">Descargar</a></td>
    <td>N/A</td>
  </tr>
  <tr>
    <td>Outlook 2007</td>
    <td><a href="https://munchkin.marketo.net/MarketoAddInSetup32.zip">Descargar</a></td>
    <td>N/A</td>
  </tr>
  <tr>
    <td>Outlook 2010</td>
    <td><a href="https://munchkin.marketo.net/MarketoAddInSetup32.zip">Descargar</a></td>
    <td><a href="https://munchkin.marketo.net/MarketoAddInSetup64.zip">Descargar</a></td>
  </tr>
  <tr>
    <td>Outlook 2013</td>
    <td><a href="https://munchkin.marketo.net/MarketoAddInSetup32.zip">Descargar</a></td>
    <td><a href="https://munchkin.marketo.net/MarketoAddInSetup64.zip">Descargar</a></td>
  </tr>
  <tr>
    <td>Outlook 2016</td>
    <td><a href="https://munchkin.marketo.net/MarketoAddInSetup32.zip">Descargar</a></td>
    <td><a href="https://munchkin.marketo.net/MarketoAddInSetup64.zip">Descargar</a></td>
  </tr>
  <tr>
    <td>Outlook 2019</td>
    <td><a href="https://munchkin.marketo.net/MarketoAddInSetup32.zip">Descargar</a></td>
    <td><a href="https://munchkin.marketo.net/MarketoAddInSetup64.zip">Descargar</a></td>
  </tr>
  <tr>
    <td>Outlook para Mac</td>
    <td>No compatible</td>
    <td>No compatible</td>
  </tr>
  <tr>
    <td>Outlook Web App</td>
    <td>No compatible</td>
    <td>No compatible</td>
  </tr>
  <tr>
    <td>Office 365*</td>
    <td><a href="https://munchkin.marketo.net/MarketoAddInSetup32.zip">Descargar</a></td>
    <td><a href="https://munchkin.marketo.net/MarketoAddInSetup64.zip">Descargar</a></td>
  </tr>
</tbody></table>

*[!DNL Office] versión 365: [!DNL Windows] solo cliente (en [!DNL Windows] 10, [!DNL Enterprise] o [!DNL Pro]).

>[!IMPORTANT]
>
>Microsoft ha lanzado [una nueva versión de Outlook para Windows](https://techcommunity.microsoft.com/t5/outlook-blog/new-outlook-for-windows-now-available/ba-p/3932068){target="_blank"}. Esta nueva versión no admite el complemento MSI Outlook existente. El complemento MSI Outlook seguirá funcionando para escritorios de Windows que ejecuten la versión clásica de Outlook. Para obtener más información acerca del nuevo Outlook para Windows para organizaciones, [haga clic aquí](https://techcommunity.microsoft.com/t5/outlook-blog/the-new-outlook-for-windows-for-organization-admins/ba-p/3929169){target="_blank"}.

## Copiar el código de registro {#copy-your-registration-code}

1. Copie el código de registro del correo electrónico de invitación que ha recibido.

   ![](assets/image2016-7-22-10-3a45-3a10.png)

1. Cerrar [!DNL Microsoft Outlook].

   ![](assets/ent-key-close-outlook-hand.png)

## Instalar {#install}

1. Ejecute el instalador.

   ![](assets/image2016-7-25-10-3a23-3a33.png)

   >[!NOTE]
   >
   >Si recibe una advertencia de seguridad, no se preocupe. Simplemente haga clic en **Ejecutar**.

1. Haga clic en **[!UICONTROL Siguiente]**.

   ![](assets/welcome-to-the-setup-wizard-hand.png)

1. Rellene **[!UICONTROL Nombre]**, **[!UICONTROL Apellido]**, **[!UICONTROL Dirección de correo electrónico]**, luego copie y pegue el **[!UICONTROL código de registro]** del correo electrónico en el formulario y haga clic en **[!UICONTROL Siguiente]**.

   ![](assets/enter-your-information-hands.png)

   >[!TIP]
   >
   >Si la instalación falla, consulte con su departamento de TI para asegurarse de que el tráfico HTTPS no esté bloqueado. El instalador requiere que el tráfico HTTPS esté abierto.

1. Haga clic en **[!UICONTROL Siguiente]** para instalarlo en la ubicación predeterminada.

   ![](assets/select-installation-folder-hand.png)

1. Haga clic en **[!UICONTROL Siguiente]**.

   ![](assets/confirm-installation-hand.png)

   >[!NOTE]
   >
   >Si recibe una solicitud de seguridad acerca de un editor desconocido, haga clic en **[!UICONTROL Sí]**.

1. La instalación ha finalizado, haga clic en **[!UICONTROL Cerrar]**.

   ![](assets/image2014-9-23-15-3a52-3a11.png)

1. Ahora abra [!DNL Microsoft Outlook] y vea los botones de Marketo.

   ![](assets/image2016-8-24-15-3a47-3a38.png)

   ¡Excelente! Ahora los botones de Marketo están en un lugar mejor.

Obtenga más información sobre el uso de las acciones Mensaje de Marketo y Registrar con Marketo.

>[!MORELIKETHIS]
>
>* [Enviar y rastrear un correo electrónico con el complemento de correo electrónico de Marketo para Outlook](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/send-and-track-an-email-with-the-email-add-in-for-outlook.md){target="_blank"}
>* [Enviar y rastrear desde Outlook usando una plantilla de Marketo](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/send-and-track-from-outlook-using-a-marketo-template.md){target="_blank"}
