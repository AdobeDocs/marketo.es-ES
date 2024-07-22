---
unique-page-id: 2359422
description: 'Personalización de un correo electrónico: documentos de Marketo, documentación del producto'
title: Personalización de un correo electrónico
exl-id: 1562796e-da47-4305-b950-3bed1d36d339
feature: Getting Started
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '338'
ht-degree: 0%

---

# Personalización de un correo electrónico {#personalize-an-email}

## Misión: Personalice sus correos electrónicos añadiendo tokens de datos {#mission-make-your-emails-personal-by-adding-data-tokens}

>[!PREREQUISITES]
>
>* [Configurar y agregar una persona](/help/marketo/getting-started/quick-wins/get-set-up-and-add-a-person.md){target="_blank"}
>* [Enviar una ráfaga por correo electrónico](/help/marketo/getting-started/quick-wins/send-an-email.md){target="_blank"}
>* [Goteo, Goteo, Nutrición](/help/marketo/getting-started/quick-wins/drip-drip-nurture.md){target="_blank"}

## Paso 1: Seleccionar un correo electrónico para personalizar {#step-select-an-email-to-personalize}

1. Seleccione uno de los correos electrónicos creados en la [victoria rápida anterior](/help/marketo/getting-started/quick-wins/drip-drip-nurture.md){target="_blank"} y haga clic en **[!UICONTROL Crear borrador]**.

   ![](assets/personalize-an-email-1.png)

   >[!NOTE]
   >
   >Esto crea una copia del correo electrónico como borrador. Recuerde aprobar el borrador para que los cambios se activen.

Si no ha habilitado un bloqueador de ventanas emergentes, el editor de correo electrónico se abrirá en una nueva pestaña o ventana. De lo contrario, haga clic dos veces en **[!UICONTROL Crear borrador]**.

## Paso 2: Hacer que el vendedor sea el remitente {#step-make-the-salesperson-the-sender}

1. Seleccione el campo **[!UICONTROL De]**, resalte y **elimine** el nombre actual.

   ![](assets/personalize-an-email-2.png)

1. Haga clic en el icono **Token** a la derecha del campo **[!UICONTROL Desde]**.

   ![](assets/personalize-an-email-3.png)

1. Busque y seleccione el token **`{{lead.Lead Owner First Name}}`**.

   ![](assets/personalize-an-email-4.png)

1. Escriba el nombre de su empresa y un guión para el **Valor predeterminado** para asegurarse de que se muestre algo en caso de que el nombre del representante de ventas no esté disponible. Haga clic en **Insertar**.

   ![](assets/personalize-an-email-5.png)

1. Pulse la barra espaciadora en el campo **[!UICONTROL Desde]**, asegurándose de que el cursor parpadee un espacio después del token que acaba de insertar. A continuación, haga clic de nuevo en el icono **Token**.

   ![](assets/personalize-an-email-6.png)

1. Busque y seleccione el token **`{{lead.Lead Owner Last Name}}`**.

   ![](assets/personalize-an-email-7.png)

1. Escriba &quot;Ventas&quot; para el **Valor predeterminado** y haga clic en **Insertar**.

   ![](assets/personalize-an-email-8.png)

## Paso 3: Añadir el nombre del posible cliente al correo electrónico {#step-add-the-leads-name-to-the-email}

1. Seleccione la sección editable superior, haga clic en el icono de engranaje y seleccione **[!UICONTROL Editar]**.

   ![](assets/personalize-an-email-9.png)

1. Agregue un espacio después de &quot;Hola&quot; y coloque el cursor delante de la coma; a continuación, haga clic en el icono **Insertar token**.

   ![](assets/personalize-an-email-10.png)

1. Busque y seleccione el token **`{{lead.First Name}}`**.

   ![](assets/personalize-an-email-11.png)

1. Escriba &quot;Amigo&quot; (o cualquier etiqueta que desee) en el campo **[!UICONTROL Valor predeterminado]** y haga clic en **[!UICONTROL Insertar]**.

   ![](assets/personalize-an-email-12.png)

   >[!TIP]
   >
   >Incluya siempre un valor predeterminado para los tokens; esto garantiza que el valor predeterminado se muestre en el correo electrónico si falta alguna parte de la información personal.

1. Haga clic en **[!UICONTROL Guardar]**.

   ![](assets/personalize-an-email-13.png)

1. En **[!UICONTROL Acciones de correo electrónico]** y seleccione **[!UICONTROL Aprobar y cerrar]**.

   ![](assets/personalize-an-email-14.png)

>[!TIP]
>
>¿Necesita un repaso rápido sobre cómo enviarse el correo electrónico? Ver [Enviar una ráfaga por correo electrónico](/help/marketo/getting-started/quick-wins/send-an-email.md){target="_blank"}.

### Misión finalizada {#mission-complete}

¡Felicidades, ha personalizado su correo electrónico!

<br> 

[◄ Misión 6: Goteo, Goteo, Nutrición](/help/marketo/getting-started/quick-wins/drip-drip-nurture.md)

[Misión 8: Alerta al representante de ventas ►](/help/marketo/getting-started/quick-wins/alert-the-sales-rep.md)
