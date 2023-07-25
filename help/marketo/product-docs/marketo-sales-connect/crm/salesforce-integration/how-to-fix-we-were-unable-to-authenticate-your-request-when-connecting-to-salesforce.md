---
unique-page-id: 14352484
description: Corrección del error "No se pudo autenticar la solicitud" al conectar con Salesforce - Documentos de Marketo - Documentación del producto
title: Cómo corregir "No se pudo autenticar su solicitud" al conectarse a Salesforce
exl-id: ddd49064-f584-4490-8d45-29cf61ed3ebe
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '186'
ht-degree: 0%

---

# Cómo corregir &quot;No se pudo autenticar su solicitud&quot; al conectarse a Salesforce {#how-to-fix-we-were-unable-to-authenticate-your-request-when-connecting-to-salesforce}

Si recibe el mensaje de error &quot;No hemos podido autenticar su solicitud&quot; al intentar conectar Sales Connect a Salesforce, podría haber una restricción en su acceso a la API de Salesforce. Consulte con su administrador de Salesforce para asegurarse de que se cumplan los siguientes requisitos.

## Habilitar API en permisos de usuario {#enable-api-in-user-permissions}

1. Haga que un administrador de Salesforce inicie sesión en SFDC.
1. Seleccionar **Configurar**.
1. Seleccionar **Administrar usuarios**.
1. Seleccionar **Perfiles**.
1. Busque el perfil en el que se encuentran los usuarios de ToutApp y haga clic en **Editar**.
1. Desplácese hacia abajo hasta **Permisos administrativos** y asegúrese de que **API habilitada** está marcada.

## Comprobar si Salesforce bloquea la conexión de Sales Connect {#check-if-salesforce-is-blocking-sales-connect-from-connecting}

1. Haga que un administrador de Salesforce inicie sesión en SFDC.
1. Seleccionar **Configurar**.
1. Seleccionar **Administrar aplicaciones**.
1. Seleccionar **Uso de OAuth para aplicaciones conectadas**.
1. Asegúrese de que Sales Connect muestra &quot;Bloquear&quot; junto a ella. Si ve &quot;Desbloquear&quot;, haga clic en el botón para desbloquear el acceso de Sales Connect a Salesforce.
