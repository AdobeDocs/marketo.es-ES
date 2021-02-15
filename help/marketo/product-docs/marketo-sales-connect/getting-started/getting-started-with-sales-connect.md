---
unique-page-id: 13796466
description: Introducción a Sales Connect - Documentos de marketing - Documentación del producto
title: Introducción a Sales Connect
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '635'
ht-degree: 0%

---


# Introducción a Sales Connect {#getting-started-with-sales-connect}

Si prefiere ver estos pasos en lugar de leerlos, vaya directamente a las [Instrucciones de video a continuación](#video).

>[!AVAILABILITY]
>
>No todos los clientes han adquirido esta funcionalidad. Póngase en contacto con el administrador de éxito del cliente para obtener más información.

## Qué debe comenzar {#what-you-need-to-get-started}

* Suscripción de marketing
* Suscripción de conexión de ventas
* Suscripción de Salesforce (con llamadas de API y Clases de Apex activadas)

## ¿Quién necesita comenzar {#who-you-need-to-get-started}?

* Usuario administrador de marketing
* Administrador de Sales Connect
* Administrador de Salesforce
* Usuarios de Sales Connect

## Administradores de Sales Connect {#sales-connect-admins}

Recibirá un correo electrónico de Marketing con un vínculo para restablecer su contraseña. Después de crear una contraseña nueva, inicie sesión en Sales Connect.

Para completar la configuración, debe hacer lo siguiente:

* [Connect Sales Connect y Salesforce](#sfdc)
* [Adquirir credenciales antes de conectar la conexión de ventas con Marketing](#acquire)
* [Connect Sales Connect con Marketing](#mkto)
* [Invitar o aprovisionar usuarios](#IPU)

Opcionalmente, también puede:

* [Probar Sales Connect en el Simulador para pruebas](#sandbox)

## Conectar la cuenta de Sales Connect con Salesforce {#connect-your-sales-connect-account-to-salesforce}

Para conectar su cuenta de Sales Connect a su cuenta de Salesforce, como administrador o como no administrador, siga los pasos descritos en [este artículo](https://docs.marketo.com/x/JwDb).

>[!NOTE]
>
>La instancia de Salesforce a la que se conecta debe ser la misma instancia que está (o estará) conectada a Marketing.

## Adquirir credenciales antes de conectar Sales Connect con Marketing {#acquiring-credentials-prior-to-connecting-sales-connect-with-marketo}

Tendrá que obtener un conjunto de credenciales desde Marketing. Estas credenciales serán utilizadas posteriormente por el administrador de Sales Connect para conectar Marketing con Sales Connect.

1. En Marketing, haga clic en **Administración**.

   ![](assets/one.png)

1. En el árbol, haga clic en **Conexión de ventas**.

   ![](assets/two.png)

1. Seleccione y envíe las siguientes credenciales de Marketing a su administrador de Sales Connect: ID de Munchkin, ID de cliente, Secreto de cliente.

   ![](assets/3.jpg)

   >[!NOTE]
   >
   >Cuando copie y pegue la información anterior, asegúrese de que no se agreguen espacios.

## Conectar ventas con marketing {#connect-sales-connect-to-marketo}

1. En Sales Connect, haga clic en el icono de engranaje y seleccione **Configuración**.

   ![](assets/four.png)

1. En Configuración de administración, seleccione **Comercializar**.

   ![](assets/eight.png)

1. Introduzca las credenciales de marketing proporcionadas por el administrador de marketing y haga clic en **Conectar**.

   ![](assets/credentials.png)

## Invitar/Aprovisionar usuarios {#invite-provision-users}

Si algún usuario ya existe en su cuenta (anteriormente desde ToutApp), aparecerá en la ficha **Acceso al equipo** de la sección Comercialización de Sales Connect.

Desde esta página puede aprovisionar su equipo como usuario de conexión de marketing para ventas. Si nunca ha utilizado ToutApp o aún no ha invitado a usuarios, siga los pasos de [este artículo](https://docs.marketo.com/display/TOUT/Invite+Team+Members).

>[!CAUTION]
>
>Espere diez minutos después de conectar Sales Connect con Marketing para realizar estos pasos.

1. Seleccione uno o varios usuarios y haga clic en **Conectar**.

   >[!NOTE]
   >
   >La asignación de espacio de trabajo solo se puede realizar una vez al invitar a usuarios. Una vez configurada, deberá desconectar al usuario para cambiarla.

   ![](assets/users.png)

1. Si la suscripción de marketing tiene habilitadas las áreas de trabajo, podrá asignar espacios de trabajo a cada usuario o conjunto de usuarios de forma masiva. Si no hay espacios de trabajo seleccionados, los asignaremos al espacio de trabajo de marketing predeterminado.

   ![](assets/nine.jpg)

1. Haga clic en la lista desplegable Espacio de trabajo, seleccione los espacios de trabajo que desee y haga clic en **Conectar**.

   ![](assets/ten.png)

   >[!NOTE]
   >
   >Si desea agregar usuarios nuevos, vaya a la sección Administración de equipos de Configuración de administración y haga clic en el botón **Invitar a usuarios**.

Puede agregar usuarios desde la página Administración de equipos y seguir los pasos anteriores para conectarlos.

## Probar Sales Connect en el Simulador para pruebas {#test-sales-connect-in-your-sandbox}

Para los equipos que deseen probar Marketingto Sales Connect con su Simulador para pruebas de marketing, se puede aprovisionar una cuenta adicional de Sales Connect si se solicita. Esto es solo para clientes que han comprado un Simulador para pruebas de marketing o para aquellos que lo tienen como parte de su paquete de marketing. Si está interesado en adquirir un Simulador para pruebas, póngase en contacto con el administrador de cuentas de Marketing to.

>[!NOTE]
>
>No se puede aprovisionar una cuenta de Sales Connect con el mismo ID de correo electrónico en varias instancias. Esto significa que si desea tener una cuenta adicional de Sales Connect para probarla con la instancia de MarketingTo Sandbox, deberá utilizar un ID de correo electrónico diferente en cada una de las cuentas.
