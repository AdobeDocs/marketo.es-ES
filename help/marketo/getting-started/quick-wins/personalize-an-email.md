---
unique-page-id: 2359422
description: 'Personalización de un correo electrónico: documentos de Marketo: documentación del producto'
title: Personalización de un correo electrónico
exl-id: 1562796e-da47-4305-b950-3bed1d36d339
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '335'
ht-degree: 0%

---

# Personalización de un correo electrónico {#personalize-an-email}

## Misión: Conversión de sus correos electrónicos en personales añadiendo tokens de datos {#mission-make-your-emails-personal-by-adding-data-tokens}

>[!PREREQUISITES]
>
>* [Configurar y agregar una persona](/help/marketo/getting-started/quick-wins/get-set-up-and-add-a-person.md)
>* [Enviar una explosión de correo electrónico](/help/marketo/getting-started/quick-wins/send-an-email.md)
>* [Perforación, Perforación](/help/marketo/getting-started/quick-wins/drip-drip-nurture.md)


## Paso 1: Seleccionar un correo electrónico para personalizar {#step-select-an-email-to-personalize}

1. Seleccione uno de los correos electrónicos de formación creados en la [victoria rápida anterior](/help/marketo/getting-started/quick-wins/drip-drip-nurture.md) y haga clic en **Editar borrador**.

   ![](assets/one-4.png)

   >[!NOTE]
   >
   >Esto crea una copia del correo electrónico como borrador. Debe aprobar el borrador para que los cambios se activen.

Si no ha habilitado un bloqueador de ventanas emergentes, el editor de correo electrónico se abrirá en una nueva pestaña o ventana. De lo contrario, haga clic en **Editar borrador** dos veces.

## Paso 2: Conversión del vendedor en el remitente {#step-make-the-salesperson-the-sender}

1. Seleccione el campo **From**, resalte y **elimine** el nombre actual.

   ![](assets/two-5.png)

1. Haga clic en el icono **Token** a la derecha del campo **From**.

   ![](assets/three-4.png)

1. Busque y seleccione el token **`{{lead.Lead Owner First Name}}`**.

   ![](assets/four-3.png)

1. Escriba el nombre de su empresa y un guión para el **Valor predeterminado** para asegurarse de que se muestre algo en caso de que el nombre del representante de venta no esté disponible. Haga clic en **Insert**.

   ![](assets/five-4.png)

1. Pulse la barra espaciadora en el campo **From**, asegurándose de que el cursor parpadea un espacio después del token que acaba de insertar. A continuación, haga clic de nuevo en el icono **Token**.

   ![](assets/six-4.png)

1. Busque y seleccione el token **`{{lead.Lead Owner Last Name}}`**.

   ![](assets/seven-5.png)

1. Escriba &quot;Ventas&quot; para el **Valor predeterminado** y haga clic en **Insertar**.

   ![](assets/eight-3.png)

## Paso 3: Agregue el nombre del posible cliente al correo electrónico {#step-add-the-leads-name-to-the-email}

1. Seleccione la sección editable superior, haga clic en el icono del engranaje y seleccione **Editar**.

   ![](assets/nine-2.png)

1. Añada un espacio después de &quot;Hello&quot; y coloque el cursor delante de la coma y, a continuación, haga clic en el icono **Insert Token**.

   ![](assets/ten-4.png)

1. Busque y seleccione el token **`{{lead.First Name}}`**.

   ![](assets/eleven-4.png)

1. Introduzca &quot;Amigo&quot; (o cualquier etiqueta que desee) en el campo **Valor predeterminado** y haga clic en **Insertar**.

   ![](assets/twelve-3.png)

   >[!TIP]
   >
   >Incluya siempre un valor predeterminado para los tokens; esto garantiza que el valor predeterminado se muestre en el correo electrónico si falta alguna parte de la información personal.

1. Haga clic en **Guardar**.

   ![](assets/thirteen-3.png)

1. Cierre la pestaña o ventana del editor de correo electrónico.

   ![](assets/fourteen-3.png)

1. En **Acciones de correo electrónico**, seleccione **Aprobar borrador**.

   ![](assets/fifteen-3.png)

>[!TIP]
>
>¿Necesita un repaso rápido sobre cómo enviarse el correo electrónico? Consulte [Enviar un mensaje de correo electrónico ](/help/marketo/getting-started/quick-wins/send-an-email.md).

### Misión completada {#mission-complete}

¡Felicidades, has personalizado tu correo electrónico!

<br> 

[◄ Misión 6: Perforación, Perforación](/help/marketo/getting-started/quick-wins/drip-drip-nurture.md)

[Misión 8: Alerta al representante de ventas ►](/help/marketo/getting-started/quick-wins/alert-the-sales-rep.md)
