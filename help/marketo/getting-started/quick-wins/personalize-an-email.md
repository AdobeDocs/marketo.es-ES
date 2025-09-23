---
unique-page-id: 2359422
description: 'Personalizar un correo electrónico: documentos de Marketo, documentación del producto'
title: Personalizar un correo electrónico
exl-id: 1562796e-da47-4305-b950-3bed1d36d339
feature: Getting Started
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '336'
ht-degree: 100%

---

# Personalizar un correo electrónico {#personalize-an-email}

## Misión: Personalice sus correos electrónicos añadiendo tókenes de datos {#mission-make-your-emails-personal-by-adding-data-tokens}

>[!PREREQUISITES]
>
>* [Configurar y añadir una persona](/help/marketo/getting-started/quick-wins/get-set-up-and-add-a-person.md){target="_blank"}
>* [Enviar correos electrónicos de forma masiva](/help/marketo/getting-started/quick-wins/send-an-email.md){target="_blank"}
>* [Sistema de goteo y nutrición](/help/marketo/getting-started/quick-wins/drip-drip-nurture.md){target="_blank"}

## Paso 1: Seleccionar un correo electrónico para su personalización {#step-select-an-email-to-personalize}

1. Seleccione uno de los correos electrónicos de nutrición creados en la [ganancia rápida anterior](/help/marketo/getting-started/quick-wins/drip-drip-nurture.md){target="_blank"} y haga clic en **[!UICONTROL Crear borrador]**.

   ![](assets/personalize-an-email-1.png)

   >[!NOTE]
   >
   >Esto crea una copia del correo electrónico como borrador. Recuerde aprobar el borrador para que los cambios se activen.

Si no ha habilitado un bloqueador de ventanas emergentes, el editor de correo electrónico se abre en una nueva pestaña o ventana. De lo contrario, haga clic dos veces en **[!UICONTROL Crear borrador]**.

## Paso 2: Hacer que el vendedor sea el remitente {#step-make-the-salesperson-the-sender}

1. Seleccione el campo **[!UICONTROL De]**, resalte y **eliminar** el nombre actual.

   ![](assets/personalize-an-email-2.png)

1. Haga clic en el icono **Token** a la derecha del campo **[!UICONTROL De]**.

   ![](assets/personalize-an-email-3.png)

1. Busque y seleccione el token **`{{lead.Lead Owner First Name}}`**.

   ![](assets/personalize-an-email-4.png)

1. Escriba el nombre de su empresa y un guion en el **valor predeterminado** para asegurarse de que se muestre algo en caso de que el nombre del representante de ventas no esté disponible. Haga clic en **Insertar**.

   ![](assets/personalize-an-email-5.png)

1. Pulse la barra espaciadora en el campo **[!UICONTROL De]**, asegurándose de que el cursor parpadee un espacio después del token que acaba de insertar. A continuación, haga clic de nuevo en el icono **Token**.

   ![](assets/personalize-an-email-6.png)

1. Busque y seleccione el token **`{{lead.Lead Owner Last Name}}`**.

   ![](assets/personalize-an-email-7.png)

1. Escriba “Ventas” en el **Valor predeterminado** y haga clic en **Insertar**.

   ![](assets/personalize-an-email-8.png)

## Paso 3: Añadir el nombre del posible cliente al correo electrónico {#step-add-the-leads-name-to-the-email}

1. Seleccione la sección editable superior, haga clic en el icono de engranaje y seleccione **[!UICONTROL Editar]**.

   ![](assets/personalize-an-email-9.png)

1. Añada un espacio después de “Hola” y coloque el cursor delante de la coma; a continuación, haga clic en el icono **Insertar token**.

   ![](assets/personalize-an-email-10.png)

1. Busque y seleccione el token **`{{lead.First Name}}`**.

   ![](assets/personalize-an-email-11.png)

1. Escriba “Amigo” (o cualquier etiqueta que desee) en el campo **[!UICONTROL Valor predeterminado]** y haga clic en **[!UICONTROL Insertar]**.

   ![](assets/personalize-an-email-12.png)

   >[!TIP]
   >
   >Incluya siempre un valor predeterminado para los tókenes; esto garantiza que el valor predeterminado se muestre en el correo electrónico si falta alguna parte de la información personal.

1. Haga clic en **[!UICONTROL Guardar]**.

   ![](assets/personalize-an-email-13.png)

1. En **[!UICONTROL Acciones de correo electrónico]**, seleccione **[!UICONTROL Aprobar y cerrar]**.

   ![](assets/personalize-an-email-14.png)

>[!TIP]
>
>¿Necesita un repaso rápido sobre cómo enviarse el correo electrónico? Vea [Enviar correos electrónicos de forma masiva](/help/marketo/getting-started/quick-wins/send-an-email.md){target="_blank"}.

### Misión completada {#mission-complete}

Enhorabuena, ha personalizado su correo electrónico.

<br> 

[◄ Misión 6: Sistema de goteo y nutrición](/help/marketo/getting-started/quick-wins/drip-drip-nurture.md)

[Misión 8: Alertar al representante de ventas ►](/help/marketo/getting-started/quick-wins/alert-the-sales-rep.md)
