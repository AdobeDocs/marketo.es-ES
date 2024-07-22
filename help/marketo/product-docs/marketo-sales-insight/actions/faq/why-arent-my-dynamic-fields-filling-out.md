---
description: ¿Por qué no se rellenan mis campos dinámicos? - Documentos de Marketo - Documentación del producto
title: ¿Por qué no se rellenan mis campos dinámicos?
exl-id: 4e1d133f-8314-4e64-b50b-f3e824c3bef4
feature: Sales Insight Actions
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '307'
ht-degree: 0%

---

# ¿Por qué no se rellenan mis campos dinámicos? {#why-arent-my-dynamic-fields-filling-out}

Los campos dinámicos solo funcionarán cuando se utilice una plantilla. Los correos electrónicos únicos individuales que escriba no los rellenarán.

## Qué comprobar {#what-to-check}

Existen tres tipos de campos dinámicos en las acciones de información de ventas: Básico, Personalizado y Salesforce. Tanto básica como personalizada buscan extraer información de la [aplicación web](https://toutapp.com/login){target="_blank"}. Si la información no existe en la aplicación web, los campos están en blanco. Los campos de Salesforce extraen información de [Salesforce.com](https://salesforce.com){target="_blank"}.

**Solucionar problemas de campos de Salesforce**

Campos de Salesforce: p. ej. `{{sfdc_account_name}}`

* Asegúrese de que está correctamente conectado con las acciones de información de ventas. Vaya a la página [Configuración](https://toutapp.com/login{target="_blank"} y haga clic en **Administrar** junto a su CRM.

**Solucionar problemas de campos básicos y personalizados**

Campos básicos de acciones de información de ventas de Marketo: p. ej., `{{company}}`

Campos personalizados de acciones de Marketo Sales Insight: p. ej., `{{custom_field_favorite_movie}}`

* El campo correspondiente debe guardarse para el contacto en la [página Personas](https://toutapp.com/next#relationships){target="_blank"} para que nuestro campo dinámico haga referencia a él. Por ejemplo, si envía un correo electrónico a Mary y utiliza el campo `{{company}}`, pero su registro de contacto no indica una compañía, no podremos rellenarlo.

## ¿Por Qué Se Envió El Correo Electrónico Sin Rellenar Todos Los Campos Dinámicos? {#why-did-my-email-send-without-populating-all-dynamic-fields}

Las acciones de perspectiva de ventas evitarán que se envíen correos electrónicos si no podemos rellenar todos los campos dinámicos en el correo electrónico. **Sin embargo**, existen algunas excepciones a esta regla. Algunos campos enviarán en blanco o rellenarán automáticamente un valor si podemos encontrar uno. A continuación, se enumeran estos campos y cómo reaccionarán si no pueden rellenarlos.

`{{first_name}}` = EN BLANCO

`{{last_name}}` =EN BLANCO

`{{title}}` = EN BLANCO

`{{company}}` = &quot;su empresa&quot;

`{{friendly_company}}` = &quot;su empresa&quot;

>[!NOTE]
>
>El campo `{{first_name}}` buscará tanto en las acciones de perspectiva de ventas como en Salesforce para intentar extraer información. Todos los demás campos de esta lista solo buscan en las acciones de información de ventas para rellenar el campo.
