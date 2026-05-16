---
unique-page-id: 1147114
description: Obtenga información acerca de los tokens de campo personalizado de miembros de programa. Utilice tokens para insertar datos de miembros en correos electrónicos y páginas de aterrizaje.
title: Tókenes de campo personalizado para miembros del programa
exl-id: 3046dec8-b885-4b08-baa9-896bcf3594b2
feature: Tokens
TQID: https://experienceleague.adobe.com/B2oY6BKJdd92AAsMPHZV8Ffyc-9jKGRpATqles6TUos
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: e64968b2-4ee5-47f9-8cae-0588f184b9eb
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 445
ht-degree: 5%

---

# Tókenes de campo personalizado para miembros del programa {#program-member-custom-field-tokens}

## Compatibilidad de tokens para campos personalizados de miembros del programa {#token-support-for-program-member-custom-fields}

En la parte posterior de las funciones Campos personalizados de miembro de programa, se está ampliando la compatibilidad con los Campos personalizados de miembro de programa en los marcos de tokens.

Los tokens de PMCF serán compatibles con el dominio miembro de la familia de tokens.

Los tokens de miembro se utilizan para campos dentro del ámbito de Miembro de programa. A partir del estado actual, los tokens de miembro también se utilizan para insertar valores únicos de socios de servicios integrados. El token `{{member.webinar url}}` resuelve automáticamente la URL de confirmación única de la persona generada por el proveedor de servicios. `{{member.registration code}}` resuelve el código de registro proporcionado por el proveedor de servicios.

>[!NOTE]
>
>* Los campos personalizados de miembros de programa solo se pueden utilizar en el contexto de un programa.
>* Los tokens de campos personalizados de miembros de programa no se pueden usar en: encabezado previo de correo electrónico, tokens de fecha en pasos de espera o fragmentos de código.
>* El estado de miembro del programa no es compatible con los tokens de miembro.

## Uso de tokens de campo personalizado de miembro de programa en Assets {#using-program-member-custom-field-tokens-in-assets}

Puede insertar tokens de campos personalizados de miembros del programa en correos electrónicos, páginas de aterrizaje, SMS, notificaciones push y webhooks.

**Correos electrónicos**

1. Seleccione el correo electrónico que desee y haga clic en **[!UICONTROL Editar borrador]**.

   ![](assets/program-member-custom-field-tokens-1.png)

1. Haga clic en el icono Insertar token.

   ![](assets/program-member-custom-field-tokens-2.png)

1. Busque y seleccione el token de campo personalizado de miembro de programa deseado, introduzca un valor predeterminado y haga clic en **[!UICONTROL Insertar]**.

   ![](assets/program-member-custom-field-tokens-3.png)

1. Haga clic en **[!UICONTROL Guardar]**.

   ![](assets/program-member-custom-field-tokens-4.png)

>[!NOTE]
>
>Recuerde aprobar el correo electrónico.

**Páginas de destino**

1. Seleccione su página de aterrizaje y haga clic en **[!UICONTROL Editar borrador]**.

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

1. Escriba un valor predeterminado y haga clic en **[!UICONTROL Insertar]**.

   ![](assets/program-member-custom-field-tokens-9.png)

1. Haga clic en **[!UICONTROL Guardar]**.

   ![](assets/program-member-custom-field-tokens-10.png)

**SMS**

1. Seleccione el SMS deseado y haga clic en **[!UICONTROL Editar borrador]**.

   ![](assets/program-member-custom-field-tokens-11.png)

1. Haga clic en el botón **`{{ Token`**.

   ![](assets/program-member-custom-field-tokens-12.png)

1. Busque y seleccione el token de campo personalizado del miembro del programa que desee. Escriba un [!UICONTROL valor predeterminado] y haga clic en **[!UICONTROL Insertar]**.

   ![](assets/program-member-custom-field-tokens-13.png)

1. Haga clic en el menú desplegable Acciones de SMS y seleccione **[!UICONTROL Aprobar y cerrar]**.

   ![](assets/program-member-custom-field-tokens-14.png)

**Notificaciones Push**

1. Seleccione la notificación push que desee y haga clic en **[!UICONTROL Editar borrador]**.

   ![](assets/program-member-custom-field-tokens-15.png)

1. Haga clic en **[!UICONTROL Notificación push]**.

   ![](assets/program-member-custom-field-tokens-16.png)

1. Haga clic en el mensaje en el editor y haga clic en el botón `{{` para obtener el selector de tokens.

   ![](assets/program-member-custom-field-tokens-17.png)

1. Busque y seleccione el token de campo personalizado del miembro del programa que desee. Escriba un valor predeterminado y haga clic en **[!UICONTROL Insertar]**.

   ![](assets/program-member-custom-field-tokens-18.png)

1. Haga clic en **[!UICONTROL Finalizar]** para guardar y salir (o en **[!UICONTROL Siguiente]** para revisar primero).

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
