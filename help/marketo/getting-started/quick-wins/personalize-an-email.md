---
unique-page-id: 2359422
description: 'Personalización de un correo electrónico: documentos de Marketo: documentación del producto'
title: Personalización de un correo electrónico
exl-id: 1562796e-da47-4305-b950-3bed1d36d339
source-git-commit: 8aa2f3069c0168f57ac00dfc7270484a9045584c
workflow-type: tm+mt
source-wordcount: '341'
ht-degree: 0%

---

# Personalización de un correo electrónico {#personalize-an-email}

## Misión: Conversión de correos electrónicos en personales añadiendo tokens de datos {#mission-make-your-emails-personal-by-adding-data-tokens}

>[!PREREQUISITES]
>
>* [Configurar y agregar una persona](/help/marketo/getting-started/quick-wins/get-set-up-and-add-a-person.md){target=&quot;_blank&quot;}
>* [Enviar una explosión de correo electrónico](/help/marketo/getting-started/quick-wins/send-an-email.md){target=&quot;_blank&quot;}
>* [Perforación, Perforación](/help/marketo/getting-started/quick-wins/drip-drip-nurture.md){target=&quot;_blank&quot;}


## Paso 1: Seleccionar un correo electrónico para personalizar {#step-select-an-email-to-personalize}

1. Seleccione uno de los correos electrónicos de formación creados en la [victoria rápida anterior](/help/marketo/getting-started/quick-wins/drip-drip-nurture.md){target=&quot;_blank&quot;} y haga clic en **Crear borrador**.

   ![](assets/personalize-an-email-1.png)

   >[!NOTE]
   >
   >Esto crea una copia del correo electrónico como borrador. Recuerde aprobar el borrador para que los cambios se activen.

Si no ha habilitado un bloqueador de ventanas emergentes, el editor de correo electrónico se abrirá en una nueva pestaña o ventana. De lo contrario, haga clic en **Crear borrador** dos veces.

## Paso 2: Convertir al vendedor en el remitente {#step-make-the-salesperson-the-sender}

1. Seleccione el **De** campo, resaltado y **delete** el nombre actual.

   ![](assets/personalize-an-email-2.png)

1. Haga clic en el **Token** a la derecha del **De** campo .

   ![](assets/personalize-an-email-3.png)

1. Busque y seleccione el **`{{lead.Lead Owner First Name}}`** token.

   ![](assets/personalize-an-email-4.png)

1. Escriba el nombre de su empresa y un guión para la **Valor predeterminado** para garantizar que se muestre algo en caso de que el nombre del representante de venta no esté disponible. Haga clic en **Insertar**.

   ![](assets/personalize-an-email-5.png)

1. Pulse la barra espaciadora de la **De** , asegúrese de que el cursor parpadea un espacio después del token que acaba de insertar. A continuación, haga clic en el **Token** de nuevo.

   ![](assets/personalize-an-email-6.png)

1. Busque y seleccione el **`{{lead.Lead Owner Last Name}}`** token.

   ![](assets/personalize-an-email-7.png)

1. Escriba &quot;Ventas&quot; para la variable **Valor predeterminado** y haga clic en **Insertar**.

   ![](assets/personalize-an-email-8.png)

## Paso 3: Añadir el nombre del posible cliente al correo electrónico {#step-add-the-leads-name-to-the-email}

1. Seleccione la sección editable superior, haga clic en el icono de engranaje y seleccione **Editar**.

   ![](assets/personalize-an-email-9.png)

1. Añada un espacio después de &quot;Hello&quot; y coloque el cursor delante de la coma y, a continuación, haga clic en el botón **Insertar token** icono.

   ![](assets/personalize-an-email-10.png)

1. Busque y seleccione el **`{{lead.First Name}}`** token.

   ![](assets/personalize-an-email-11.png)

1. Escriba &quot;Amigo&quot; (o cualquier etiqueta que desee) en el **Valor predeterminado** y haga clic en **Insertar**.

   ![](assets/personalize-an-email-12.png)

   >[!TIP]
   >
   >Incluya siempre un valor predeterminado para los tokens; esto garantiza que el valor predeterminado se muestre en el correo electrónico si falta alguna parte de la información personal.

1. Haga clic en **Guardar**.

   ![](assets/personalize-an-email-13.png)

1. En **Acciones de correo electrónico** y seleccione **Aprobar y cerrar**.

   ![](assets/personalize-an-email-14.png)

>[!TIP]
>
>¿Necesita un repaso rápido sobre cómo enviarse el correo electrónico? Consulte [Enviar una explosión de correo electrónico](/help/marketo/getting-started/quick-wins/send-an-email.md){target=&quot;_blank&quot;}.

### Misión finalizada {#mission-complete}

¡Felicidades, has personalizado tu correo electrónico!

<br> 

[◄ Misión 6: Perforación, Perforación](/help/marketo/getting-started/quick-wins/drip-drip-nurture.md)

[Misión 8: Alerta al representante de ventas ►](/help/marketo/getting-started/quick-wins/alert-the-sales-rep.md)
