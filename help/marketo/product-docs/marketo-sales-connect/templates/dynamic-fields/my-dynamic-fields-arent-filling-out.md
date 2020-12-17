---
unique-page-id: 14352602
description: Mis campos dinámicos no se rellenan - Documentos de marketing - Documentación del producto
title: Mis campos dinámicos no se rellenan
translation-type: tm+mt
source-git-commit: 5c9683c6b00ccbf9e9d606fd4513432c9872ad00
workflow-type: tm+mt
source-wordcount: '290'
ht-degree: 0%

---


# Mis campos dinámicos no se rellenan {#my-dynamic-fields-arent-filling-out}

Los campos dinámicos solo funcionarán cuando se utilice una plantilla. Los correos electrónicos individuales que se escriban no los completarán.

## Qué comprobar {#what-to-check}

Hay tres tipos de campos dinámicos en Sales Connect: Básico, Personalizado y Salesforce. Tanto Basic como Custom buscan extraer información de la [aplicación Web](http://toutapp.com/login). Si la información no existe en la aplicación web, los campos estarán en blanco. Los campos de Salesforce extraen información de [Salesforce.com](http://salesforce.com).

`**Troubleshooting Salesforce Fields**`

Campos de Salesforce: p. ej. `{{sfdc_account_name}}`

* Asegúrese de que está correctamente conectado con Sales Connect. Vaya a la página [Configuración](http://toutapp.com/next#settings) y haga clic en **Administrar** al lado de su CRM.

**Resolución de problemas de campos básicos y personalizados**

Campos básicos de Tout: p. ej. `{{company}}`

Campos personalizados de Tout: p. ej. `{{custom_field_favorite_movie}}`

* T `he corresponding field needs to be saved for your contact` en la [página Personas](http://toutapp.com/next#relationships) para que nuestro campo dinámico haga referencia. Por ejemplo: si envía un correo electrónico a Mary y utiliza el campo `{{company}}`, pero su registro de contacto no lista una compañía, no podremos cumplimentar eso.

## ¿Por Qué Se Envió Mi Correo Electrónico Sin Rellenar Todos Los Campos Dinámicos? {#why-did-my-email-send-without-populating-all-dynamic-fields}

Sales Connect impedirá que se envíen sus correos electrónicos si no podemos rellenar todos sus campos dinámicos en el correo electrónico. **Sin embargo**, hay algunas excepciones a esta regla. Algunos campos se enviarán en blanco o se rellenará automáticamente un valor si se encuentra uno. Estos campos y cómo reaccionarán si no pueden rellenar el campo se enumeran a continuación.

`{{first_name}}` = BLANCO

`{{last_name}}` =EN BLANCO

`{{title}}` = BLANCO

`{{company}}` = &quot;su compañía&quot;

`{{friendly_company}}` = &quot;su compañía&quot;

>[!NOTE]
>
>El campo `{{first_name}}` buscará información tanto en Sales Connect como en Salesforce. Todos los demás campos de esta lista solo buscan en Sales Connect para rellenar el campo.

