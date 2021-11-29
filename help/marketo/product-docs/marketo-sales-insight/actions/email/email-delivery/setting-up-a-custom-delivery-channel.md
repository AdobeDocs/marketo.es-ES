---
description: 'Configuración de un canal de entrega personalizado: documentos de Marketo: documentación del producto'
title: Configuración de un canal de envío personalizado
hide: true
hidefromtoc: true
source-git-commit: 55afdc537d0a5d0b6114f478c4dd2ded09c84e34
workflow-type: tm+mt
source-wordcount: '409'
ht-degree: 0%

---

# Configuración de un canal de envío personalizado {#setting-up-a-custom-delivery-channel}

Marketo Sales Connect le permite integrarse con un servidor SMTP personalizado para el envío de sus correos electrónicos. Esta es una buena opción para aquellos que no desean enviar correos electrónicos masivos desde su canal de entrega de Gmail o Exchange.

Los usuarios pueden configurar un servidor SMTP personalizado para su propio uso individual, o los administradores pueden configurar un SMTP de equipo para compartirlo entre todos los usuarios de Conexión de ventas de su instancia.

>[!NOTE]
>
>* Además de configurar el servidor SMTP, su [la identidad de correo electrónico debe verificarse](/help/marketo/product-docs/marketo-sales-connect/getting-started/email-settings/verify-your-email.md) antes de poder enviar correos electrónicos.
>* Le recomendamos que trabaje con su equipo de TI o con el proveedor de servidores SMTP para obtener las credenciales de servidor correctas para su servidor SMTP.
>* No puede conectar el servidor de Gmail y Exchange con las credenciales del servidor SMTP. Utilice nuestro servicio de conexión de correo electrónico para integrarlo con estos proveedores.


## SMTP personalizado {#custom-smtp}

1. Inicie sesión en la [aplicación web](https://toutapp.com/login), haga clic en el icono del engranaje en la parte superior derecha y seleccione **Configuración**.

PICC

1. En Mi cuenta, haga clic en **Configuración de correo electrónico**.

PICC

1. Haga clic en **Canal de envío personalizado**.

PICC

1. Introduzca las credenciales del servidor SMTP y haga clic en **Connect**.

PICC

>[!NOTE]
>
>Si este es su único canal de envío, se asigna automáticamente a todas sus identidades de correo electrónico y ya ha terminado aquí. Si este no es el único canal de envío, continúe con el paso 5.

1. Mientras sigue en Configuración de correo electrónico, haga clic en **Dirección y firma**.

PICC

1. Busque la identidad de correo electrónico para la que desea elegir un canal de envío y haga clic en **Elegir canal de entrega**.

PICC

1. En la tarjeta de entrega, haga clic en **Editar**.

PICC

1. Haga clic en la lista desplegable Canal y seleccione el canal de envío personalizado que acaba de añadir. Haga clic en **Guardar**.

PICC

>[!NOTE]
>
>Si el administrador del equipo configura el servidor SMTP del equipo, se aplicará automáticamente solo a su identidad de correo electrónico predeterminada y estará disponible como opción para el resto de identidades de correo electrónico.

## Servidor SMTP de equipo {#team-smtp-server}

>[!NOTE]
>
>**Se requieren permisos de administrador**

1. Inicie sesión en la [aplicación web](https://toutapp.com/login), haga clic en el icono del engranaje en la parte superior derecha y seleccione **Configuración**.

PICC

1. En Configuración de administración, haga clic en **General**.

PICC

1. Haga clic en **Canal de entrega de equipo**.

PICC

1. Introduzca las credenciales del servidor SMTP y haga clic en **Connect**.

PICC

>[!NOTE]
>
>Team SMTP Server será el canal de envío predeterminado de la identidad de correo electrónico predeterminada para todos los integrantes del equipo. Además, estará disponible como opción de canal de envío para todas las demás identidades de correo electrónico.

>[!MORELIKETHIS]
>
>* [Conexión de correo electrónico para usuarios de Gmail](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md)
>* [Conexión de correo electrónico para usuarios de Outlook](/help/marketo/product-docs/marketo-sales-connect/email-plugins/msc-for-outlook/email-connection-for-outlook-users.md)

