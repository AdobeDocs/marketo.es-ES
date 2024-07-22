---
unique-page-id: 14352602
description: 'Mis campos dinámicos no se rellenan. Documentos de Marketo: documentación del producto'
title: Mis campos dinámicos no se están rellenando
exl-id: fb3e8b56-506a-41f8-a84f-41370381c058
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '293'
ht-degree: 0%

---

# Mis campos dinámicos no se están rellenando {#my-dynamic-fields-arent-filling-out}

Los campos dinámicos solo funcionarán cuando se utilice una plantilla. Los correos electrónicos únicos individuales que escriba no los rellenarán.

## Qué comprobar {#what-to-check}

Existen tres tipos de campos dinámicos en Sales Connect: Básico, Personalizado y Salesforce. Tanto básica como personalizada buscan extraer información de la [aplicación web](https://toutapp.com/login). Si la información no existe en la aplicación web, los campos están en blanco. Los campos de Salesforce extraen información de [Salesforce.com](https://salesforce.com).

**Solucionar problemas de campos de Salesforce**

Campos de Salesforce: p. ej. `{{sfdc_account_name}}`

* Asegúrese de que está correctamente conectado con Sales Connect. Vaya a la página [Configuración](https://toutapp.com/login) y haga clic en **Administrar** junto a su CRM.

**Solucionar problemas de campos básicos y personalizados**

Campos básicos de información: p. ej. `{{company}}`

Campos personalizados de información: p. ej. `{{custom_field_favorite_movie}}`

* El campo correspondiente debe guardarse para el contacto en la [página Personas](https://toutapp.com/next#relationships) para que nuestro campo dinámico haga referencia a él. Por ejemplo, si envía un correo electrónico a Mary y utiliza el campo `{{company}}`, pero su registro de contacto no indica una compañía, no podremos rellenarlo.

## ¿Por Qué Se Envió El Correo Electrónico Sin Rellenar Todos Los Campos Dinámicos? {#why-did-my-email-send-without-populating-all-dynamic-fields}

Sales Connect evitará que se envíen mensajes de correo electrónico si no podemos rellenar todos los campos dinámicos en el mensaje. **Sin embargo**, existen algunas excepciones a esta regla. Algunos campos enviarán en blanco o rellenarán automáticamente un valor si podemos encontrar uno. A continuación, se enumeran estos campos y cómo reaccionarán si no pueden rellenarlos.

`{{first_name}}` = EN BLANCO

`{{last_name}}` =EN BLANCO

`{{title}}` = EN BLANCO

`{{company}}` = &quot;su empresa&quot;

`{{friendly_company}}` = &quot;su empresa&quot;

>[!NOTE]
>
>El campo `{{first_name}}` buscará tanto en Sales Connect como en Salesforce para intentar extraer información. Todos los demás campos de esta lista solo buscan en Sales Connect para rellenar el campo.
