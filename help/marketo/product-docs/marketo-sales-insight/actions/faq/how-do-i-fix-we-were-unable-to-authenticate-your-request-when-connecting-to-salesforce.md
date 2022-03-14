---
description: ¿Cómo puedo corregir "No hemos podido autenticar su solicitud" al conectarse a Salesforce - Marketo Docs - Documentación del producto
title: ¿Cómo puedo corregir "No hemos podido autenticar su solicitud" al conectarme a Salesforce?
hide: true
hidefromtoc: true
source-git-commit: c398aff77e09f4a63db5d51af55178aa663ec98e
workflow-type: tm+mt
source-wordcount: '193'
ht-degree: 0%

---

# ¿Cómo puedo corregir &quot;No hemos podido autenticar su solicitud&quot; al conectarme a Salesforce? {#how-do-i-fix-we-were-unable-to-authenticate-your-request-when-connecting-to-salesforce}

Si recibe el mensaje de error &quot;No hemos podido autenticar su solicitud&quot; al intentar conectar acciones de perspectiva de ventas a Salesforce, puede haber una restricción en su acceso a la API de Salesforce. Consulte a su administrador de Salesforce para asegurarse de que se han realizado las siguientes acciones.

## Habilitar API en permisos de usuario {#enable-api-in-user-permissions}

1. Inicie sesión con un administrador de Salesforce en SFDC.
1. Select **Configuración**.
1. Select **Administrar usuarios**.
1. Select **Perfiles**.
1. Busque el perfil en el que se encuentran los usuarios de ToutApp y haga clic en **Editar**.
1. Desplácese hacia abajo hasta **Permisos administrativos** y asegúrese de **API habilitada** está activada.

## Comprobar si Salesforce bloquea las acciones de perspectiva de ventas al conectarse {#check-if-salesforce-is-blocking-sales-insight-actions-from-connecting}

1. Pida a un administrador de Salesforce que inicie sesión en SFDC.
1. Select **Configuración**.
1. Select **Administrar aplicaciones**.
1. Select **Uso de aplicaciones conectadas auth**.
1. Asegúrese de que las Acciones de perspectivas de ventas muestran el &quot;bloque&quot; junto a él. Si ve &quot;Desbloquear&quot;, haga clic en el botón para desbloquear el acceso de las acciones de Insight de Ventas a Salesforce.
