---
unique-page-id: 14352602
description: Obtenga ayuda cuando los campos dinámicos no se rellenen en Sales Connect. Solucione el problema de por qué los campos de combinación muestran datos en blanco o incorrectos.
title: Mis campos dinámicos no se están rellenando
exl-id: fb3e8b56-506a-41f8-a84f-41370381c058
feature: Marketo Sales Connect
TQID: https://experienceleague.adobe.com/sbjcM4m5C5yVDq1nPOO3lt-uSUWO3q9DguMS2Dn23Fc
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: f82558ea-6af5-44eb-a424-5b3389abb0a3
topic_v2: id: c1579802-ddd4-4214-8a91-97b2066abe11
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 302
ht-degree: 3%

---

# Mis campos dinámicos no se están rellenando {#my-dynamic-fields-arent-filling-out}

Los campos dinámicos solo funcionarán cuando utilice una plantilla. Los correos electrónicos únicos individuales que escriba no los rellenarán.

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
