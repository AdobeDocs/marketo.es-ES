---
unique-page-id: 14352600
description: Cómo configurar el servidor SMTP de Outlook365 con Sales Connect - Documentos de marketing - Documentación del producto
title: Cómo configurar el servidor SMTP de Outlook365 con Sales Connect
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '252'
ht-degree: 0%

---


# Cómo configurar el servidor SMTP de Outlook365 con Sales Connect {#how-to-set-up-your-outlook-smtp-server-with-sales-connect}

>[!NOTE]
>
>Si su organización utiliza Outlook y está intentando configurar un canal de envío de correo electrónico con Marketing a Sales Connect, le recomendamos que se conecte a su servidor de Exchange [mediante la función](http://docs.marketo.com/x/Z4AOAQ)de conexión de correo electrónico.

Para configurar un servidor [SMTP](http://docs.marketo.com/x/zYTS) personalizado como canal de envío alternativo, ToutApp requiere que utilice algún tipo de autenticación por motivos de seguridad. Puede configurar cualquier servidor SMTP en la página [de configuración](http://toutapp.com/next#settings/email-servers/smtp/configure)SMTP. Para configurar un servidor SMTP de Office365, Microsoft recomienda la siguiente configuración:\
**Servidor** SMTP: smtp.office365.com\
**Puerto** del servidor: Puerto 587 - Seguro\
**Método** de autenticación: Inicio de sesión (SSL/TLS)\
**Nombre de usuario o inicio de sesión**: su dirección de correo electrónico de Office365\
**Contraseña**: su contraseña de correo electrónico de Office365\
**Su dominio**: el dominio de su compañía

Si sigue teniendo problemas al configurar el servidor SMTP, asocie con el administrador de Exchange para asegurarse de que se utilizan las credenciales correctas.

>[!NOTE]
>
>Al enviar a través de su SMTP de Office365, Microsoft impone un `limit of 30 messages sent per minute`límite de 10.000 destinatarios por día. Además, `each member` el equipo que desee enviar correos electrónicos a través de su servidor SMTP de Office365 deberá configurarlos con su propia dirección de correo electrónico y contraseña en la configuración de Sales Connect. Marque la casilla de la opción &quot; `Make this deliverability channel to all my team members` `" will not work` para esta configuración, de acuerdo con las directivas de cuenta de Office365 de Microsoft.

