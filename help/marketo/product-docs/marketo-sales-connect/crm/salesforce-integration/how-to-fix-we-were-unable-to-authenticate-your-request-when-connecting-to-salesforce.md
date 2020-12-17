---
unique-page-id: 14352484
description: Cómo corregir "No hemos podido autenticar su solicitud" al conectarse a Salesforce - Documentos de marketing - Documentación del producto
title: Cómo corregir "No hemos podido autenticar su solicitud" al conectarse a Salesforce
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '186'
ht-degree: 0%

---


# Cómo corregir &quot;No hemos podido autenticar su solicitud&quot; al conectarse a Salesforce {#how-to-fix-we-were-unable-to-authenticate-your-request-when-connecting-to-salesforce}

Si recibe el mensaje de error &quot;No hemos podido autenticar su solicitud&quot; al intentar conectar Sales Connect con Salesforce, puede haber una restricción en su acceso a la API de Salesforce. Póngase en contacto con el administrador de Salesforce para asegurarse de que existen los siguientes elementos.

## Habilitar API en Permisos de usuario {#enable-api-in-user-permissions}

1. Tener un registro de administrador de Salesforce en SFDC.
1. Seleccione **Configuración**.
1. Seleccione **Administrar usuarios**.
1. Seleccione **Perfiles**.
1. Busque el Perfil en el que se encuentran los usuarios de ToutApp y haga clic en **Editar**.
1. Desplácese hacia abajo hasta **Permisos administrativos** y asegúrese de que **API habilitada** está marcada.

## Compruebe si Salesforce bloquea la conexión de Sales Connect {#check-if-salesforce-is-blocking-sales-connect-from-connecting}

1. Inicie sesión en SFDC con el administrador de Salesforce.
1. Seleccione **Configuración**.
1. Seleccione **Administrar aplicaciones**.
1. Seleccione **Uso de OAuth de aplicaciones conectadas**.
1. Asegúrese de que Sales Connect muestra &quot;Bloque&quot; junto a él. Si ve &quot;Desbloquear&quot;, haga clic en el botón para desbloquear el acceso de Sales Connect a Salesforce.

