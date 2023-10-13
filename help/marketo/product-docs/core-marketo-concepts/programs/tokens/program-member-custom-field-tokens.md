---
unique-page-id: 1147114
description: Tokens de campo personalizado de miembro del programa - Documentos de Marketo - Documentación del producto
title: Tokens de campo personalizado de miembro de programa
exl-id: 3046dec8-b885-4b08-baa9-896bcf3594b2
feature: Tokens
source-git-commit: b21f955bf98063e11f8ed3fdc6f164134ee4f5aa
workflow-type: tm+mt
source-wordcount: '435'
ht-degree: 3%

---

# Tokens de campo personalizado de miembro de programa {#program-member-custom-field-tokens}

## Compatibilidad de tokens para campos personalizados de miembros del programa {#token-support-for-program-member-custom-fields}

En la parte posterior de las funciones Campos personalizados de miembro de programa, se está ampliando la compatibilidad con los Campos personalizados de miembro de programa en los marcos de tokens.

Los tokens de PMCF serán compatibles con el dominio miembro de la familia de tokens.

Los tokens de miembro se utilizan para campos dentro del ámbito de Miembro de programa. A partir del estado actual, los tokens de miembro también se utilizan para insertar valores únicos de socios de servicios integrados. `{{member.webinar url}}` resuelve automáticamente la URL de confirmación única de la persona generada por el proveedor de servicios. {{member.registration code}} resuelve en el código de registro proporcionado por el proveedor de servicios.

>[!NOTE]
>
>* Los campos personalizados de miembros de programa solo se pueden utilizar en el contexto de un programa.
>* Los tokens de campos personalizados de miembros de programa no se pueden usar en: encabezado previo de correo electrónico, tokens de fecha en pasos de espera o fragmentos de código.
>* El estado de miembro del programa no es compatible con los tokens de miembro.

## Uso de tokens de campo personalizado de miembro de programa en Assets {#using-program-member-custom-field-tokens-in-assets}

Puede insertar tokens de campos personalizados de miembros del programa en correos electrónicos, páginas de aterrizaje, SMS, notificaciones push y webhooks.

**Emails**

1. Seleccione el correo electrónico deseado y haga clic en **[!UICONTROL Editar borrador]**.

   ![](assets/program-member-custom-field-tokens-1.png)

1. Haga clic en el icono Insertar token.

   ![](assets/program-member-custom-field-tokens-2.png)

1. Busque y seleccione el token de campo personalizado de miembro de programa deseado, introduzca un valor predeterminado y haga clic en **[!UICONTROL Insertar]**.

   ![](assets/program-member-custom-field-tokens-3.png)

1. Haga clic en **[!UICONTROL Guardar]**.

   ![](assets/program-member-custom-field-tokens-4.png)

>[!NOTE]
>
>No olvide aprobar su correo electrónico.

**Páginas de destino**

1. Seleccione la página de aterrizaje y haga clic en **[!UICONTROL Editar borrador]**.

   ![](assets/program-member-custom-field-tokens-5.png)

   >[!NOTE]
   >
   >El diseñador de la página de aterrizaje se abre en una nueva ventana.

1. Haga doble clic en el cuadro de texto enriquecido al que desee agregar el token.

   ![](assets/program-member-custom-field-tokens-6.png)

1. Haga clic en el lugar donde desee que esté el token y, a continuación, haga clic en el icono Insertar token.

   ![](assets/program-member-custom-field-tokens-7.png)

1. Busque y seleccione el token deseado.

   ![](assets/program-member-custom-field-tokens-8.png)

1. Introduzca un valor predeterminado y haga clic en **[!UICONTROL Insertar]**.

   ![](assets/program-member-custom-field-tokens-9.png)

1. Haga clic en **[!UICONTROL Guardar]**.

   ![](assets/program-member-custom-field-tokens-10.png)

**SMS**

1. Seleccione el SMS deseado y haga clic en **[!UICONTROL Editar borrador]**.

   ![](assets/program-member-custom-field-tokens-11.png)

1. Haga clic en **`{{ Token`** botón.

   ![](assets/program-member-custom-field-tokens-12.png)

1. Busque y seleccione el token de campo personalizado del miembro del programa que desee. Introduzca un valor predeterminado y haga clic en Insert.

   ![](assets/program-member-custom-field-tokens-13.png)

1. Haga clic en el menú desplegable Acciones de SMS y seleccione **[!UICONTROL Aprobar y cerrar]**.

   ![](assets/program-member-custom-field-tokens-14.png)

**Insertar notificaciones**

1. Seleccione la notificación push que desee y haga clic en **[!UICONTROL Editar borrador]**.

   ![](assets/program-member-custom-field-tokens-15.png)

1. Clic **[!UICONTROL Notificación push]**.

   ![](assets/program-member-custom-field-tokens-16.png)

1. Haga clic en el mensaje en el editor y haga clic en `{{` para obtener el selector de token.

   ![](assets/program-member-custom-field-tokens-17.png)

1. Busque y seleccione el token de campo personalizado del miembro del programa que desee. Introduzca un valor predeterminado y haga clic en **[!UICONTROL Insertar]**.

   ![](assets/program-member-custom-field-tokens-18.png)

1. Clic **[!UICONTROL Finalizar]** para guardar y salir (o **[!UICONTROL Siguiente]** para revisarlo primero).

   ![](assets/program-member-custom-field-tokens-19.png)

>[!NOTE]
>
>Si el campo personalizado del miembro del programa para un miembro del programa no tiene valor, el token se sustituirá por el valor predeterminado si se ha proporcionado.

## Uso de tokens de campo personalizado de miembro de programa en campañas {#using-program-member-custom-field-tokens-in-campaigns}

Los tokens de campo personalizado de miembro de programa se pueden utilizar en:

* Crear tarea
* Crear tarea en Microsoft
* Momentos interesantes
* Cambiar acciones de flujo de valor de datos
* Webhooks
