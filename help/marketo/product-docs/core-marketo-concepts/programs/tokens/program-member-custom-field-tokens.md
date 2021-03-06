---
unique-page-id: 1147114
description: Tokens de campo personalizados de miembro del programa - Marketo Docs - Documentación del producto
title: Tokens de campo personalizados de miembro del programa
translation-type: tm+mt
source-git-commit: 35e8b41574ebf8aafa27a59440c8ea9cb6413d50
workflow-type: tm+mt
source-wordcount: '439'
ht-degree: 0%

---


# Tokens de campo personalizados de miembro del programa {#program-member-custom-field-tokens}

## Compatibilidad con tokens para los campos personalizados de miembro del programa {#token-support-for-program-member-custom-fields}

En la parte posterior de las funciones Campos personalizados de miembros del programa , se está ampliando la compatibilidad con Campos personalizados de miembros del programa en los marcos de token.

Los tokens de PMCF serán compatibles con el dominio miembro de la familia de tokens.

Los tokens de miembro se utilizan para los campos comprendidos en el ámbito de los miembros del programa. A partir del estado actual, los tokens de miembro también se utilizan para insertar valores únicos de socios de servicios integrados. `{{member.webinar url}}` resuelve automáticamente la URL de confirmación única de la persona generada por el proveedor de servicios. {{member.registration code}} se resuelve en el código de registro proporcionado por el proveedor de servicios.

>[!NOTE]
>
>* Los campos personalizados de miembro del programa solo se pueden usar en el contexto de un programa.
>* Los tokens de campos personalizados de miembro del programa no se pueden usar en: secuencias de comandos de correo electrónico, encabezado previo de correo electrónico, tokens de fecha en pasos de espera o fragmentos.
>* El estado de miembro del programa no es compatible con los tokens de miembro.


## Uso de tokens de campo personalizados de miembro del programa en Assets {#using-program-member-custom-field-tokens-in-assets}

Puede insertar Tokens de campos personalizados de miembro del programa en correos electrónicos, páginas de aterrizaje, SMS, notificaciones push y Webhooks.

**Correos electrónicos**

1. Seleccione el correo electrónico deseado y haga clic en **Editar borrador**.

   ![](assets/program-member-custom-field-tokens-1.png)

1. Haga clic en el icono Insertar token .

   ![](assets/program-member-custom-field-tokens-2.png)

1. Busque y seleccione el Token de campo personalizado del miembro del programa que desee, introduzca un valor predeterminado y haga clic en **Insertar**.

   ![](assets/program-member-custom-field-tokens-3.png)

1. Haga clic en **Guardar**.

   ![](assets/program-member-custom-field-tokens-4.png)

>[!NOTE]
>
>No olvide aprobar su correo electrónico.

**Páginas de aterrizaje**

1. Seleccione la página de aterrizaje y haga clic en **Editar borrador**.

   ![](assets/program-member-custom-field-tokens-5.png)

   >[!NOTE]
   >
   >El diseñador de páginas de aterrizaje se abre en una nueva ventana.

1. Haga doble clic en el cuadro de texto enriquecido al que desee agregar el token.

   ![](assets/program-member-custom-field-tokens-6.png)

1. Haga clic donde desee que esté el token y, a continuación, haga clic en el icono Insertar token.

   ![](assets/program-member-custom-field-tokens-7.png)

1. Busque y seleccione el token deseado.

   ![](assets/program-member-custom-field-tokens-8.png)

1. Introduzca un valor predeterminado y haga clic en **Insert**.

   ![](assets/program-member-custom-field-tokens-9.png)

1. Haga clic en **Guardar**.

   ![](assets/program-member-custom-field-tokens-10.png)

**SMS**

1. Seleccione el SMS deseado y haga clic en **Editar borrador**.

   ![](assets/program-member-custom-field-tokens-11.png)

1. Haga clic en el botón **`{{ Token`**.

   ![](assets/program-member-custom-field-tokens-12.png)

1. Busque y seleccione el token de campo personalizado del miembro del programa que desee. Introduzca un valor predeterminado y haga clic en Insertar.

   ![](assets/program-member-custom-field-tokens-13.png)

1. Haga clic en la lista desplegable Acciones de SMS y seleccione **Aprobar y cerrar**.

   ![](assets/program-member-custom-field-tokens-14.png)

**Notificaciones push**

1. Seleccione la notificación push deseada y haga clic en **Editar borrador**.

   ![](assets/program-member-custom-field-tokens-15.png)

1. Haga clic en **Notificaciones push**.

   ![](assets/program-member-custom-field-tokens-16.png)

1. Haga clic en el mensaje en el editor y haga clic en el botón `{{` para obtener el selector de tokens.

   ![](assets/program-member-custom-field-tokens-17.png)

1. Busque y seleccione el token de campo personalizado del miembro del programa que desee. Introduzca un valor predeterminado y haga clic en **Insert**.

   ![](assets/program-member-custom-field-tokens-18.png)

1. Haga clic en **Finish** para guardar y salir (o **Next** para revisarlo primero).

   ![](assets/program-member-custom-field-tokens-19.png)

>[!NOTE]
>
>Si el campo personalizado miembro del programa de un miembro del programa no tiene valor, el token se sustituirá por el valor predeterminado si se ha proporcionado.

## Uso de tokens de campo personalizados de miembro del programa en campañas {#using-program-member-custom-field-tokens-in-campaigns}

Los tokens de campo personalizados de miembro del programa se pueden usar en:

* Crear tarea
* Crear tarea en Microsoft
* Momentos interesantes
* Cambiar acciones de flujo de valor de datos
* Enlaces web
