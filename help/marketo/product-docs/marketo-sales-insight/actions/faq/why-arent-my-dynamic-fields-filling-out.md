---
description: '¿Por qué no se rellenan mis campos dinámicos: documentos de Marketo: documentación del producto?'
title: ¿Por qué no se rellenan mis campos dinámicos?
hide: true
hidefromtoc: true
source-git-commit: 8e31c2da9351d784e97d3d2bfe0d3d07dfab8961
workflow-type: tm+mt
source-wordcount: '309'
ht-degree: 0%

---

# ¿Por qué no se rellenan mis campos dinámicos? {#why-arent-my-dynamic-fields-filling-out}

Los campos dinámicos solo funcionarán cuando utilice una plantilla. Los correos electrónicos individuales individuales que escribas no los rellenarán.

## Qué comprobar {#what-to-check}

Existen tres tipos de campos dinámicos en las acciones de perspectiva de ventas: Básico, Personalizado y Salesforce. Básico y Personalizado ambos buscan extraer información de la variable [aplicación web](https://toutapp.com/login). Si la información no existe en la aplicación web, los campos estarán en blanco. Los campos de Salesforce extraen información de [Salesforce.com](https://salesforce.com).

**Solución de problemas de los campos de Salesforce**

Campos de Salesforce: p. ej. `{{sfdc_account_name}}`

* Asegúrese de que esté correctamente conectado con las acciones de perspectivas de ventas. Vaya a la [Configuración](https://toutapp.com/login) página y haga clic en **Administrar** junto a su CRM.

**Solución de problemas de campos básicos y personalizados**

Campos Básicos De Tout: p. ej. `{{company}}`

Tout Campos Personalizados: p. ej. `{{custom_field_favorite_movie}}`

* El campo correspondiente debe guardarse para su contacto en la sección [Página Personas](https://toutapp.com/next#relationships) para que haga referencia a nuestro campo dinámico. Por ejemplo, si está enviando un correo electrónico a Mary y usa la variable `{{company}}` , pero su registro de contacto no enumera una empresa, no podremos rellenarlo.

## ¿Por Qué Se Envió Mi Correo Electrónico Sin Rellenar Todos Los Campos Dinámicos? {#why-did-my-email-send-without-populating-all-dynamic-fields}

Las acciones de perspectiva de ventas evitarán que se envíen sus correos electrónicos si no podemos rellenar todos sus campos dinámicos en el correo electrónico. **Sin embargo**, hay algunas excepciones a esta regla. Algunos campos se envían en blanco o se rellena automáticamente un valor si se encuentra uno. Estos campos y cómo reaccionarán si no pueden rellenar el campo se enumeran a continuación.

`{{first_name}}` = EN BLANCO

`{{last_name}}` =EN BLANCO

`{{title}}` = EN BLANCO

`{{company}}` = &quot;su empresa&quot;

`{{friendly_company}}` = &quot;su empresa&quot;

>[!NOTE]
>
>La variable `{{first_name}}` para intentar extraer información, el campo buscará tanto en las acciones de perspectivas de ventas como en Salesforce. Todos los demás campos de esta lista solo buscan en Acciones de perspectiva de ventas para rellenar el campo.
