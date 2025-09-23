---
unique-page-id: 14746470
description: 'Configuración de un canal de entrega personalizado: documentos de Marketo, documentación del producto'
title: Configuración de un canal de entrega personalizado
exl-id: a31f7bfd-a4ee-4948-9bdc-b49d47054d40
feature: Marketo Sales Connect
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '386'
ht-degree: 4%

---

# Configuración de un canal de entrega personalizado {#setting-up-a-custom-delivery-channel}

[!DNL Marketo Sales Connect] le permite integrar con un servidor SMTP personalizado para el envío de sus correos electrónicos. Esta es una excelente opción para aquellos que no desean enviar correos electrónicos masivos fuera de su canal de entrega de Gmail o [!DNL Exchange].

Los usuarios pueden configurar un servidor SMTP personalizado para su propio uso individual, o los administradores pueden configurar un SMTP de equipo para compartirlo entre todos los usuarios de [!DNL Sales Connect] de su instancia.

>[!NOTE]
>
>* Además de configurar su servidor SMTP, su [identidad de correo electrónico debe verificarse](/help/marketo/product-docs/marketo-sales-connect/getting-started/email-settings/verify-your-email.md) para poder enviar correos electrónicos.
>* Se recomienda trabajar con su equipo de TI o con el proveedor de servidores SMTP para obtener las credenciales de servidor adecuadas para su servidor SMTP.
>* No puede conectar su servidor Gmail y [!DNL Exchange] con las credenciales del servidor SMTP. Utilice nuestro servicio de conexión de correo electrónico para integrarse con estos proveedores.

## SMTP personalizado {#custom-smtp}

1. Inicie sesión en la [aplicación web](https://toutapp.com/login), haga clic en el icono de engranaje en la parte superior derecha y elija **[!UICONTROL Configuración]**.

   ![](assets/setting-up-a-custom-delivery-channel-1.png)

1. En [!UICONTROL Mi cuenta], haga clic en **[!UICONTROL Configuración de correo electrónico]**.

   ![](assets/setting-up-a-custom-delivery-channel-2.png)

1. Haga clic en **[!UICONTROL Canal de entrega personalizado]**.

   ![](assets/setting-up-a-custom-delivery-channel-3.png)

1. Escriba sus credenciales de [!UICONTROL SMTP Server] y haga clic en **[!UICONTROL Conectar]**.

   ![](assets/setting-up-a-custom-delivery-channel-4.png)

   >[!NOTE]
   >
   >Si este es su único canal de envío, se asigna automáticamente a todas las identidades de correo electrónico y ha terminado aquí. Si este no es el único canal de envío, siga con el paso 5.

1. Mientras sigue en [!UICONTROL Configuración de correo electrónico], haga clic en **[!UICONTROL Dirección y firma]**.

   ![](assets/setting-up-a-custom-delivery-channel-5.png)

1. Busque la identidad de correo electrónico para la que desea elegir un canal de entrega y haga clic en **[!UICONTROL Elegir canal de entrega]**.

   ![](assets/setting-up-a-custom-delivery-channel-6.png)

1. En la tarjeta [!UICONTROL Deliverability], haga clic en **[!UICONTROL Editar]**.

   ![](assets/setting-up-a-custom-delivery-channel-7.png)

1. Haga clic en el menú desplegable [!UICONTROL Canal] y elija el canal de entrega personalizado que acaba de agregar. Haga clic en **[!UICONTROL Guardar]**.

   ![](assets/setting-up-a-custom-delivery-channel-8.png)

   >[!NOTE]
   >
   >Si el administrador del equipo configura el servidor SMTP de equipo, se aplicará automáticamente solo a su identidad de correo electrónico predeterminada y estará disponible como opción para el resto de identidades de correo electrónico.

## Servidor SMTP del equipo {#team-smtp-server}

>[!NOTE]
>
>**Se requieren permisos de administración**

1. Inicie sesión en la [aplicación web](https://toutapp.com/login), haga clic en el icono de engranaje en la parte superior derecha y elija **[!UICONTROL Configuración]**.

   ![](assets/setting-up-a-custom-delivery-channel-9.png)

1. En [!UICONTROL Configuración de administración], haga clic en **[!UICONTROL General]**.

   ![](assets/setting-up-a-custom-delivery-channel-10.png)

1. Haga clic en **[!UICONTROL Canal de envío de equipo]**.

   ![](assets/setting-up-a-custom-delivery-channel-11.png)

1. Escriba sus credenciales de [!UICONTROL SMTP Server] y haga clic en **[!UICONTROL Conectar]**.

   ![](assets/setting-up-a-custom-delivery-channel-12.png)

   >[!NOTE]
   >
   >El servidor SMTP de equipo será el canal de entrega predeterminado de la identidad de correo electrónico predeterminada para todos los integrantes del equipo. Además, estará disponible como opción de canal de envío para todas las demás identidades de correo electrónico.

   >[!MORELIKETHIS]
   >
   >* [Conexión de correo electrónico para usuarios de Gmail](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md)
   >
   >* [Conexión de correo electrónico para [!DNL Outlook] Usuarios](/help/marketo/product-docs/marketo-sales-connect/email-plugins/msc-for-outlook/email-connection-for-outlook-users.md)
