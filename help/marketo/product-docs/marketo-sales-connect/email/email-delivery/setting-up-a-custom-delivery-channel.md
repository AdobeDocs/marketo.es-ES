---
unique-page-id: 14746470
description: 'Configuración de un canal de entrega personalizado: documentos de Marketo, documentación del producto'
title: Configuración de un canal de entrega personalizado
exl-id: a31f7bfd-a4ee-4948-9bdc-b49d47054d40
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '397'
ht-degree: 0%

---

# Configuración de un canal de entrega personalizado {#setting-up-a-custom-delivery-channel}

Marketo Sales Connect le permite integrarse con un servidor SMTP personalizado para el envío de sus correos electrónicos. Esta es una buena opción para aquellos que no desean enviar correos electrónicos masivos fuera de su canal de entrega de Gmail o Exchange.

Los usuarios pueden configurar un servidor SMTP personalizado para su uso individual, o los administradores pueden configurar un SMTP de equipo para compartirlo entre todos los usuarios de Sales Connect de su instancia.

>[!NOTE]
>
>* Además de configurar el servidor SMTP, su [debe verificarse la identidad del correo electrónico](/help/marketo/product-docs/marketo-sales-connect/getting-started/email-settings/verify-your-email.md) antes de poder enviar correos electrónicos.
>* Se recomienda trabajar con su equipo de TI o con el proveedor de servidores SMTP para obtener las credenciales de servidor adecuadas para su servidor SMTP.
>* No puede conectar el servidor de Gmail y Exchange con las credenciales del servidor SMTP. Utilice nuestro servicio de conexión de correo electrónico para integrarse con estos proveedores.

## SMTP personalizado {#custom-smtp}

1. Inicie sesión en [aplicación web](https://toutapp.com/login), haga clic en el icono de engranaje en la parte superior derecha y seleccione **Configuración**.

   ![](assets/setting-up-a-custom-delivery-channel-1.png)

1. En Mi cuenta, haga clic en **Configuración de correo electrónico**.

   ![](assets/setting-up-a-custom-delivery-channel-2.png)

1. Clic **Canal de envío personalizado**.

   ![](assets/setting-up-a-custom-delivery-channel-3.png)

1. Introduzca las credenciales del servidor SMTP y haga clic en **Connect**.

   ![](assets/setting-up-a-custom-delivery-channel-4.png)

   >[!NOTE]
   >
   >Si este es su único canal de envío, se asigna automáticamente a todas las identidades de correo electrónico y ha terminado aquí. Si este no es el único canal de envío, siga con el paso 5.

1. Mientras sigue en Configuración de correo electrónico, haga clic en **Dirección y firma**.

   ![](assets/setting-up-a-custom-delivery-channel-5.png)

1. Busque la identidad de correo electrónico para la que desea elegir un canal de envío y haga clic en **Elegir canal de entrega**.

   ![](assets/setting-up-a-custom-delivery-channel-6.png)

1. En la tarjeta de envío, haga clic en **Editar**.

   ![](assets/setting-up-a-custom-delivery-channel-7.png)

1. Haga clic en el menú desplegable Canal y elija el canal de entrega personalizado que acaba de añadir. Clic **Guardar**.

   ![](assets/setting-up-a-custom-delivery-channel-8.png)

   >[!NOTE]
   >
   >Si el administrador del equipo configura el servidor SMTP de equipo, se aplicará automáticamente solo a su identidad de correo electrónico predeterminada y estará disponible como opción para el resto de identidades de correo electrónico.

## Servidor SMTP del equipo {#team-smtp-server}

>[!NOTE]
>
>**Permisos de administración necesarios**

1. Inicie sesión en [aplicación web](https://toutapp.com/login), haga clic en el icono de engranaje en la parte superior derecha y seleccione **Configuración**.

   ![](assets/setting-up-a-custom-delivery-channel-9.png)

1. En Configuración de administración, haga clic en **General**.

   ![](assets/setting-up-a-custom-delivery-channel-10.png)

1. Clic **Canal de envío de equipo**.

   ![](assets/setting-up-a-custom-delivery-channel-11.png)

1. Introduzca las credenciales del servidor SMTP y haga clic en **Connect**.

   ![](assets/setting-up-a-custom-delivery-channel-12.png)

   >[!NOTE]
   >
   >El servidor SMTP de equipo será el canal de entrega predeterminado de la identidad de correo electrónico predeterminada para todos los integrantes del equipo. Además, estará disponible como opción de canal de envío para todas las demás identidades de correo electrónico.

   >[!MORELIKETHIS]
   >
   >* [Conexión de correo electrónico para usuarios de Gmail](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md)
   >
   >* [Conexión de correo electrónico para usuarios de Outlook](/help/marketo/product-docs/marketo-sales-connect/email-plugins/msc-for-outlook/email-connection-for-outlook-users.md)
