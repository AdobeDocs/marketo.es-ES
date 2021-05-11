---
unique-page-id: 13796466
description: Introducción a Sales Connect - Documentos de Marketo - Documentación del producto
title: Introducción a Sales Connect
exl-id: 8c5b1f65-449c-4304-b904-fc6442a47e5a
translation-type: tm+mt
source-git-commit: 20ccc6ba2b26b869776ed88ed6fe76a67f74400a
workflow-type: tm+mt
source-wordcount: '624'
ht-degree: 0%

---

# Introducción a Sales Connect {#getting-started-with-sales-connect}

Si prefiere ver estos pasos en lugar de leerlos, vaya directamente a las [Instrucciones de vídeo a continuación](#video).

>[!AVAILABILITY]
>
>No todos los clientes han adquirido esta funcionalidad. Para obtener más información, póngase en contacto con el administrador de éxito del cliente.

## Lo que debe comenzar {#what-you-need-to-get-started}

* suscripción a Marketo
* Suscripción a Conexión de ventas
* Suscripción a Salesforce (con llamadas API y clases Apex habilitadas)

## A quién debe empezar {#who-you-need-to-get-started}

* Usuario administrador de Marketo
* Usuario administrador de Sales Connect
* Administrador de Salesforce
* Usuarios de Sales Connect

## Administradores de conexión de ventas {#sales-connect-admins}

Recibirá un correo electrónico de Marketo con un vínculo para restablecer su contraseña. Después de crear una contraseña nueva, inicie sesión en Conexión de ventas.

Para completar la configuración, debe hacer lo siguiente:

* [Conectar Sales Connect y Salesforce](#connect-your-sales-connect-account-to-salesforce)
* [Adquirir credenciales antes de conectar ventas y conectar con Marketo](#acquiring-credentials-prior-to-connecting-sales-connect-with-marketo)
* [Conectar ventas con Marketo](#connect-sales-connect-to-marketo)
* [Invitar/aprovisionar usuarios](#invite-provision-users)

Opcionalmente, también puede:

* [Probar conexión de ventas en el Simulador para pruebas](#test-sales-connect-in-your-sandbox)

## Conecte su cuenta de conexión de ventas a Salesforce {#connect-your-sales-connect-account-to-salesforce}

Para conectar su cuenta de Conexión de ventas a su cuenta de Salesforce, como administrador o no administrador, siga los pasos de [este artículo](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-integration/connect-your-sales-connect-account-to-salesforce.md).

>[!NOTE]
>
>La instancia de Salesforce a la que se conecte debe ser la misma instancia que esté (o que vaya a estar) conectada a Marketo.

## Adquirir credenciales antes de conectar ventas y conectar con Marketo {#acquiring-credentials-prior-to-connecting-sales-connect-with-marketo}

Tendrá que obtener un conjunto de credenciales desde Marketo. Más adelante, el administrador de conexión de ventas utilizará estas credenciales para conectar Marketo con Conexión de ventas.

1. En Marketo, haga clic en **Admin**.

   ![](assets/one.png)

1. En el árbol, haga clic en **Conexión de ventas**.

   ![](assets/two.png)

1. Seleccione y envíe las siguientes credenciales de Marketo a su administrador de conexión de ventas: Munchkin ID, Client ID, Client Secret.

   ![](assets/3.jpg)

   >[!NOTE]
   >
   >Cuando copie y pegue la información anterior, asegúrese de que no se agreguen espacios.

## Conectar ventas con Marketo {#connect-sales-connect-to-marketo}

1. En Conexión de ventas, haga clic en el icono del engranaje y seleccione **Configuración**.

   ![](assets/four.png)

1. En Configuración de administración, seleccione **Marketo**.

   ![](assets/eight.png)

1. Introduzca las credenciales de Marketo proporcionadas por el administrador de Marketo y haga clic en **Connect**.

   ![](assets/credentials.png)

## Invitar/aprovisionar usuarios {#invite-provision-users}

Si algún usuario ya existe en su cuenta (anteriormente desde ToutApp), se mostrará en la pestaña **Acceso al equipo** de la sección Marketo de Conexión de ventas.

Puede aprovisionar su equipo como usuario de Marketo Sales Connect desde esta página. Si nunca ha utilizado ToutApp, o aún no ha invitado a usuarios, siga los pasos de [este artículo](/help/marketo/product-docs/marketo-sales-connect/admin/invite-users.md).

>[!CAUTION]
>
>Espere diez minutos después de conectar Conexión de ventas con Marketo antes de realizar estos pasos.

1. Seleccione uno o varios usuarios y haga clic en **Conectar**.

   >[!NOTE]
   >
   >La asignación de espacio de trabajo solo se puede realizar una vez en el momento de invitar a los usuarios. Una vez configurado, tendrá que desconectar al usuario para cambiarlo.

   ![](assets/users.png)

1. Si la suscripción a Marketo tiene habilitados los espacios de trabajo, podrá asignar espacios de trabajo a cada usuario o conjunto de usuarios de forma masiva. Si no se seleccionan espacios de trabajo, se asignarán al espacio de trabajo predeterminado de Marketo.

   ![](assets/nine.jpg)

1. Haga clic en la lista desplegable Workspace , seleccione los espacios de trabajo que desee y haga clic en **Connect**.

   ![](assets/ten.png)

   >[!NOTE]
   >
   >Si desea agregar nuevos usuarios, vaya a la sección Administración de equipos de Configuración de administración y haga clic en el botón **Invitar usuarios**.

Puede agregar usuarios adicionales desde la página Administración de equipos y seguir los pasos anteriores para conectarlos.

## Probar conexión de ventas en su Sandbox {#test-sales-connect-in-your-sandbox}

Para los equipos que deseen probar Marketo Sales Connect con su Sandbox de Marketo, se puede aprovisionar una cuenta adicional de Sales Connect bajo petición. Esto solo es para clientes que han comprado un Simulador para pruebas de Marketo o que lo tienen como parte de su paquete de Marketo. Si está interesado en adquirir un Simulador para pruebas, póngase en contacto con su administrador de cuentas de Marketo.

>[!NOTE]
>
>No se puede aprovisionar una cuenta de Conexión de ventas con el mismo ID de correo electrónico para varias instancias. Esto significa que si desea tener una cuenta adicional de conexión de ventas para probarla con la instancia de Marketo Sandbox, deberá utilizar un ID de correo electrónico diferente en cada una de las cuentas.
