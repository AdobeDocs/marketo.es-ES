---
unique-page-id: 2949711
description: 'Instalación del complemento de correo electrónico de Marketo para Outlook con un código de registro: documentos de Marketo, documentación del producto'
title: Instalación del complemento de correo electrónico de Marketo para Outlook con un código de registro
exl-id: d7a877c2-f71e-44da-b323-04f6cdb44eb0
source-git-commit: 8b9b2b83f5dc8908f9794d1ee387299edaae31b3
workflow-type: tm+mt
source-wordcount: '516'
ht-degree: 3%

---

# Instalación del complemento de correo electrónico de Marketo para Outlook con un código de registro {#install-the-marketo-email-add-in-for-outlook-with-a-registration-code}

Si los usuarios pueden acceder a la configuración de administración de sus portátiles, puede enviarles directamente un código de registro.

Si no ha recibido un correo electrónico de invitación, pídale al administrador de Marketo que le invite.

>[!PREREQUISITES]
>
>Debes ser... [ha emitido una licencia de complemento de correo electrónico de Marketo](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/issue-a-marketo-email-add-in-license.md).

>[!IMPORTANT]
>
>La instalación no es compatible con equipos en los que la carpeta Usuario de Windows contenga caracteres que no sean ingleses. Windows genera automáticamente esta carpeta en `<System Root>\Users\` se basa en el nombre de usuario de Windows y puede contener caracteres que no sean ingleses si el nombre de usuario de Windows no es inglés. Trabaje con su equipo de TI para comprobar si tiene problemas de instalación.

>[!NOTE]
>
>Las funciones de acciones de perspectiva de ventas, como Enviar correo electrónico de ventas, Agregar a la campaña de ventas y Tareas, no están disponibles en los complementos de correo electrónico de perspectiva de ventas para Gmail y Outlook. En este momento, los usuarios solo tienen la capacidad de enviar un correo electrónico rastreable con o sin una plantilla de correo electrónico de Marketo desde su cliente de correo electrónico al utilizar los complementos de correo electrónico de Sales Insight.

## Descargar instalador {#download-installer}

1. Identifique su [Versión de Microsoft Outlook](https://support.office.com/en-us/article/what-version-of-outlook-do-i-have-b3a9568c-edb5-42b9-9825-d48d82b2257c){target="_blank"}

1. Haga clic en el vínculo para descargar el programa de instalación adecuado para su versión de Microsoft Outlook.

   >[!NOTE]
   >
   >En este momento, los vínculos siguientes solo funcionan en Microsoft Edge o haciendo clic con el botón derecho en Chrome. Sentimos cualquier inconveniente.

   | Versión de Outlook | Outlook de 32 bits | Outlook de 64 bits |
   |---|---|---|
   | Outlook 2000 | No compatible | N/A |
   | Outlook 2003 | [Descargar](https://munchkin.marketo.net/MarketoAddInSetup32.msi) | N/A |
   | Outlook 2007 | [Descargar](https://munchkin.marketo.net/MarketoAddInSetup32.msi) | N/A |
   | Outlook 2010 | [Descargar](https://munchkin.marketo.net/MarketoAddInSetup32.msi) | [Descargar](https://munchkin.marketo.net/MarketoAddInSetup64.msi) |
   | Outlook 2013 | [Descargar](https://munchkin.marketo.net/MarketoAddInSetup32.msi) | [Descargar](https://munchkin.marketo.net/MarketoAddInSetup64.msi) |
   | Outlook 2016 | [Descargar](https://munchkin.marketo.net/MarketoAddInSetup32.msi) | [Descargar](https://munchkin.marketo.net/MarketoAddInSetup64.msi) |
   | Outlook 2019 | [Descargar](https://munchkin.marketo.net/MarketoAddInSetup32.msi) | [Descargar](https://munchkin.marketo.net/MarketoAddInSetup64.msi) |
   | Outlook para Mac | No compatible | No compatible |
   | Outlook Web App | No compatible | No compatible |
   | Office 365* | [Descargar](https://munchkin.marketo.net/MarketoAddInSetup32.msi) | [Descargar](https://munchkin.marketo.net/MarketoAddInSetup64.msi) |

   *Versión de Office 365: solo cliente de Windows (en Windows 10, Enterprise o Pro).

## Copiar el código de registro {#copy-your-registration-code}

1. Copie el código de registro del correo electrónico de invitación que ha recibido.

   ![](assets/image2016-7-22-10-3a45-3a10.png)

1. Cierre Microsoft Outlook.

   ![](assets/ent-key-close-outlook-hand.png)

## Instalar {#install}

1. Ejecute el instalador.

   ![](assets/image2016-7-25-10-3a23-3a33.png)

   >[!NOTE]
   >
   >Si recibe una advertencia de seguridad, no se preocupe. Solo haga clic en **Ejecutar**.

1. Clic **Siguiente**.

   ![](assets/welcome-to-the-setup-wizard-hand.png)

1. Completar en **Nombre**, **Apellidos**, **Correo electrónico**, luego copie y pegue el **Código de registro** del correo electrónico al formulario y haga clic en **Siguiente**.

   ![](assets/enter-your-information-hands.png)

   >[!TIP]
   >
   >Si la instalación falla, consulte con su departamento de TI para asegurarse de que el tráfico HTTPS no esté bloqueado. El instalador requiere que el tráfico HTTPS esté abierto.

1. Clic **Siguiente** para instalar en la ubicación predeterminada.

   ![](assets/select-installation-folder-hand.png)

1. Clic **Siguiente**.

   ![](assets/confirm-installation-hand.png)

   >[!NOTE]
   >
   >Si aparece un mensaje de seguridad acerca de un editor desconocido, haga clic en **Sí**.

1. La instalación ha finalizado y haga clic en **Cerrar**.

   ![](assets/image2014-9-23-15-3a52-3a11.png)

1. Ahora abra Microsoft Outlook y vea los botones de Marketo.

   ![](assets/image2016-8-24-15-3a47-3a38.png)

   ¡Excelente! Ahora los botones de Marketo están en un lugar mejor.

Obtenga más información sobre el uso de las acciones Mensaje de Marketo y Registrar con Marketo.

>[!MORELIKETHIS]
>
>* [Envío y seguimiento de un correo electrónico con el complemento de correo electrónico de Marketo para Outlook](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/send-and-track-an-email-with-the-email-add-in-for-outlook.md){target="_blank"}
>* [Envío y seguimiento desde Outlook mediante una plantilla de Marketo](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/send-and-track-from-outlook-using-a-marketo-template.md){target="_blank"}
