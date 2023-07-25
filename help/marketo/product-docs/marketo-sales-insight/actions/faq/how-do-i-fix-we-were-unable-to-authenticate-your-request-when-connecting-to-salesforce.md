---
description: ¿Cómo soluciono "No hemos podido autenticar su solicitud" al conectar con Salesforce? - Documentos de Marketo - Documentación del producto
title: ¿Cómo soluciono "No hemos podido autenticar su solicitud" al conectar con Salesforce?
exl-id: ef876f0f-bd76-4ba5-bf48-885ee048ceae
feature: Sales Insight Actions
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '193'
ht-degree: 0%

---

# ¿Cómo soluciono &quot;No hemos podido autenticar su solicitud&quot; al conectar con Salesforce? {#how-do-i-fix-we-were-unable-to-authenticate-your-request-when-connecting-to-salesforce}

Si recibe el mensaje de error &quot;No hemos podido autenticar su solicitud&quot; al intentar conectar las acciones de Sales Insight a Salesforce, puede haber una restricción en su acceso a la API de Salesforce. Consulte con su administrador de Salesforce para asegurarse de que se cumplan los siguientes requisitos.

## Habilitar API en permisos de usuario {#enable-api-in-user-permissions}

1. Haga que un administrador de Salesforce inicie sesión en SFDC.
1. Seleccionar **Configurar**.
1. Seleccionar **Administrar usuarios**.
1. Seleccionar **Perfiles**.
1. Busque el perfil en el que se encuentran los usuarios de ToutApp y haga clic en **Editar**.
1. Desplácese hacia abajo hasta **Permisos administrativos** y asegúrese de que **API habilitada** está marcada.

## Comprobar si Salesforce impide que las acciones de perspectiva de ventas se conecten {#check-if-salesforce-is-blocking-sales-insight-actions-from-connecting}

1. Haga que un administrador de Salesforce inicie sesión en SFDC.
1. Seleccionar **Configurar**.
1. Seleccionar **Administrar aplicaciones**.
1. Seleccionar **Uso de OAuth para aplicaciones conectadas**.
1. Asegúrese de que Acciones de perspectiva de ventas muestra &quot;Bloquear&quot; junto a ella. Si ve &quot;Desbloquear&quot;, haga clic en el botón para desbloquear el acceso de las acciones de información de ventas a Salesforce.
