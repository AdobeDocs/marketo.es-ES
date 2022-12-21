---
unique-page-id: 14352484
description: 'Corrección de "No hemos podido autenticar su solicitud" al conectarse a Salesforce: Documentos de Marketo: Documentación del producto'
title: Corrección de "No se pudo autenticar la solicitud" al conectarse a Salesforce
exl-id: ddd49064-f584-4490-8d45-29cf61ed3ebe
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '186'
ht-degree: 0%

---

# Corrección de &quot;No se pudo autenticar la solicitud&quot; al conectarse a Salesforce {#how-to-fix-we-were-unable-to-authenticate-your-request-when-connecting-to-salesforce}

Si recibe el mensaje de error &quot;No hemos podido autenticar su solicitud&quot; al intentar conectar Sales Connect a Salesforce, puede haber una restricción en su acceso a la API de Salesforce. Consulte a su administrador de Salesforce para asegurarse de que se han realizado las siguientes acciones.

## Habilitar API en permisos de usuario {#enable-api-in-user-permissions}

1. Inicie sesión con un administrador de Salesforce en SFDC.
1. Select **Configuración**.
1. Select **Administrar usuarios**.
1. Select **Perfiles**.
1. Busque el perfil en el que se encuentran los usuarios de ToutApp y haga clic en **Editar**.
1. Desplácese hacia abajo hasta **Permisos administrativos** y asegúrese de **API habilitada** está activada.

## Comprobar si Salesforce bloquea la conexión de ventas {#check-if-salesforce-is-blocking-sales-connect-from-connecting}

1. Pida a un administrador de Salesforce que inicie sesión en SFDC.
1. Select **Configuración**.
1. Select **Administrar aplicaciones**.
1. Select **Uso de aplicaciones conectadas auth**.
1. Asegúrese de que Sales Connect muestra el &quot;Bloque&quot; junto a él. Si ve &quot;Desbloquear&quot;, haga clic en el botón para desbloquear el acceso de Sales Connect a Salesforce.
