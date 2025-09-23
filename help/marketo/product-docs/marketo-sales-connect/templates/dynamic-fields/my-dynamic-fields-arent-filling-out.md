---
unique-page-id: 14352602
description: 'Mis campos dinámicos no se rellenan. Documentos de Marketo: documentación del producto'
title: Mis campos dinámicos no se están rellenando
exl-id: fb3e8b56-506a-41f8-a84f-41370381c058
feature: Marketo Sales Connect
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '278'
ht-degree: 4%

---

# Mis campos dinámicos no se están rellenando {#my-dynamic-fields-arent-filling-out}

Los campos dinámicos solo funcionarán cuando se utilice una plantilla. Los correos electrónicos únicos individuales que escriba no los rellenarán.

## Qué comprobar {#what-to-check}

Existen tres tipos de campos dinámicos en [!DNL Sales Connect]: Básico, Personalizado y [!DNL Salesforce]. Tanto básica como personalizada buscan extraer información de la [aplicación web](https://toutapp.com/login). Si la información no existe en la aplicación web, los campos están en blanco. [!DNL Salesforce] campos obtienen información de [Salesforce.com](https://salesforce.com).

**Solucionar problemas de [!DNL Salesforce] campos**

[!DNL Salesforce] campos: p. ej. `{{sfdc_account_name}}`

* Asegúrese de que esté correctamente conectado con [!DNL Sales Connect]. Vaya a la página [Configuración](https://toutapp.com/login) y haga clic en **[!UICONTROL Administrar]** junto a su CRM.

**Solucionar problemas de campos básicos y personalizados**

Campos básicos de información: p. ej. `{{company}}`

Campos personalizados de información: p. ej. `{{custom_field_favorite_movie}}`

* El campo correspondiente debe guardarse para el contacto en la [página Personas](https://toutapp.com/next#relationships) para que nuestro campo dinámico haga referencia a él. Por ejemplo, si envía un correo electrónico a Mary y utiliza el campo `{{company}}`, pero su registro de contacto no indica una compañía, no podremos rellenarlo.

## ¿Por Qué Se Envió El Correo Electrónico Sin Rellenar Todos Los Campos Dinámicos? {#why-did-my-email-send-without-populating-all-dynamic-fields}

[!DNL Sales Connect] evitará que se envíen sus correos electrónicos si no podemos rellenar todos los campos dinámicos en el correo electrónico. **Sin embargo**, existen algunas excepciones a esta regla. Algunos campos enviarán en blanco o rellenarán automáticamente un valor si podemos encontrar uno. A continuación, se enumeran estos campos y cómo reaccionarán si no pueden rellenarlos.

`{{first_name}}` = EN BLANCO

`{{last_name}}` =EN BLANCO

`{{title}}` = EN BLANCO

`{{company}}` = &quot;su empresa&quot;

`{{friendly_company}}` = &quot;su empresa&quot;

>[!NOTE]
>
>El campo `{{first_name}}` buscará tanto en [!DNL Sales Connect] como en [!DNL Salesforce] para intentar extraer información. Todos los demás campos de esta lista solo buscan [!DNL Sales Connect] para rellenar el campo.
